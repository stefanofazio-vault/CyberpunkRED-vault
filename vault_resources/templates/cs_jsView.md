```dataviewjs
// ===============================
// CONFIG
// ===============================
const characterPath = "Schede/yaml/<nomePG_cognomePG>";

// ===============================
// LOAD CHARACTER
// ===============================
const page = dv.page(characterPath);
let valid = true;

if (!page) {
  dv.paragraph("❌ Personaggio non trovato");
  valid = false;
}

if (valid)
{
// ===============================
// IDENTITY
// ===============================
const id = page.identity ?? {};
const roles = page.roles ?? [];

dv.header(1, `${id.name ?? "Unknown"} ${id.handle ? `(${id.handle})` : ""}`);

if (roles.length > 0) {
  dv.header(3, "Roles");
  dv.list(
    roles.map(r =>
      `${r.label}${r.rank != null ? ` — Rank ${r.rank}` : ""}`
    )
  );
}

if (id.bundle) dv.paragraph(`**Background:** ${id.bundle}`);

// ===============================
// STATS
// ===============================
const stats = page.stats ?? {};

dv.header(2, "Stats");
dv.table(
  ["Stat", "Valore"],
  Object.entries(stats).map(([k, v]) => [k, v])
);

// ===============================
// HP & DEATH SAVE
// ===============================
const hp = page.hp ?? {};
const derived = page.derived ?? {};

const body = stats.FIS ?? 0;
const hpMax = 10 + body * 5;

const deathSaveStat = derived.death_save_base ?? "FIS";
const deathSaveBase = stats[deathSaveStat] ?? 0;
const deathSavePenalty = hp.death_save_penalty ?? 0;
const deathSave = deathSaveBase - deathSavePenalty;

dv.header(2, "HP & Death Save");
dv.paragraph(`❤️ **HP:** ${hp.current ?? 0} / ${hpMax}`);
dv.paragraph(`☠️ **Death Save:** ${deathSave}`);

// ===============================
// ARMOR
// ===============================
const armor = page.armor ?? {};

if (Object.keys(armor).length) {
  dv.header(2, "Armor");
  dv.table(
    ["Slot", "Nome", "SP", "Ablation", "SP Attuale"],
    Object.entries(armor).map(([slot, a]) => [
      slot,
      a.name ?? "-",
      a.sp ?? 0,
      a.ablation ?? 0,
      (a.sp ?? 0) - (a.ablation ?? 0),
    ])
  );
}

// ===============================
// SKILLS
// ===============================
const skills = page.skills ?? {};
const skillCategories = {};

for (let key in skills) {
  const s = skills[key];
  const statValue = stats[s.stat] ?? 0;
  const skillValue = s.value ?? 0;
  const total = statValue + skillValue;

  if (!skillCategories[s.category]) {
    skillCategories[s.category] = [];
  }

  skillCategories[s.category].push([
    s.label,
    s.stat,
    statValue,
    skillValue,
    total,
  ]);
}

dv.header(2, "Skills");

for (let cat in skillCategories) {
  dv.header(3, cat.toUpperCase());
  dv.table(
    ["Skill", "Stat", "Stat", "Skill", "Totale"],
    skillCategories[cat]
  );
}

// ===============================
// EQUIPMENT
// ===============================
const eq = page.equipment ?? {};

if (eq.weapons?.length) {
  dv.header(2, "Weapons");
  dv.table(
    ["Nome", "Tipo", "Danno", "ROF", "Mani", "Qualità"],
    eq.weapons.map(w => [
      w.name,
      w.type ?? "-",
      w.damage ?? "-",
      w.rof ?? "-",
      w.hands ?? "-",
      w.quality ?? "-",
    ])
  );
}

if (eq.gear?.length) {
  dv.header(2, "Gear");
  dv.table(
    ["Nome", "Descrizione"],
    eq.gear.map(g => [
      g.name,
      g.description ?? "",
    ])
  );
}

// ===============================
// CYBERWARE
// ===============================
const cyber = page.cyberware ?? {};
let totalHL = 0;

if (Object.keys(cyber).length) {
  dv.header(2, "Cyberware");

  for (let slot in cyber) {
    dv.header(3, slot.toUpperCase());

    cyber[slot].forEach(c => {
      totalHL += c.hl ?? 0;
      dv.paragraph(`**${c.name}** (HL ${c.hl ?? 0})`);

      if (c.options?.length) {
        c.options.forEach(o => {
          totalHL += o.hl ?? 0;
          dv.paragraph(`↳ ${o.name} (HL ${o.hl ?? 0})`);
        });
      }
    });
  }

  dv.paragraph(`🧠 **Humanity Loss Totale:** ${totalHL}`);
}
}

```

