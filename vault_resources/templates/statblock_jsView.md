---
type: npc
game: cyberpunk-red

identity:
  name: <NOME>
  role: <ROLE>
  threat: <LEVEL>

combat:
  combat_number: <VAL>
  initiative: <VAL>
  mi: <VAL>
  dr: <VAL>

health:
  hp: <VAL>

armor:
  head: <VAL>
  body: <VAL>

weapons:
  - name: <NAME>
    damage: "Xd6"
    rof: <VAL>
    hands: <VAL>
    ammo: <VAL>

  - name: <NAME>
    damage: "Xd6"
    rof: <VAL>
    hands: <VAL>

cyberware:
  - <NAME>
  - <NAME>
  - <NAME>

---

```dataviewjs
const page = dv.current();

// -------------------------
// Helpers
// -------------------------
const block = (label, value) =>
  value !== undefined && value !== null
    ? `**${label}:** ${value}`
    : null;

const join = (...items) =>
  items.filter(Boolean).join(" | ");

// -------------------------
// Identity
// -------------------------
const id = page.identity ?? {};
const name = id.name ?? "Unknown NPC";
const role = id.role ? `— ${id.role}` : "";
const tier = page.tier ? `(Tier ${page.tier})` : "";

dv.header(2, `${name} ${role} ${tier}`);

// -------------------------
// Combat Overview
// -------------------------
const combat = page.combat ?? {};
const health = page.health ?? {};
const armor = page.armor ?? {};

dv.paragraph(
  join(
    block("CN", combat.combat_number ?? combat.cn),
    block("Init", combat.initiative ?? combat.init),
    block("MI", combat.mi),
    block("DR", combat.dr)
  )
);

dv.paragraph(
  join(
    block("HP", health.hp),
    armor.head !== undefined || armor.body !== undefined
      ? `**Armor:** Head ${armor.head ?? 0} | Body ${armor.body ?? 0}`
      : null
  )
);

// -------------------------
// Weapons
// -------------------------
if (Array.isArray(page.weapons) && page.weapons.length) {
  dv.header(3, "Weapons");

  page.weapons.forEach(w => {
    const line = [
      `**${w.name}**`,
      w.damage ? `— ${w.damage}` : null,
      w.rof ? `- ROF ${w.rof}` : null,
      w.hands ? `- Mani: ${w.hands}` : null,
	  w.ammo ? `- Colpi: ${w.ammo}` : null,
      w.notes ? `(${w.notes})` : null
    ].filter(Boolean).join(" ");

    dv.paragraph(`• ${line}`);
  });
}

// -------------------------
// Cyberware
// -------------------------
if (Array.isArray(page.cyberware) && page.cyberware.length) {
  dv.header(3, "Cyberware");

  page.cyberware.forEach(cw => {
    dv.paragraph(`• ${cw}`);
  });
}
```
