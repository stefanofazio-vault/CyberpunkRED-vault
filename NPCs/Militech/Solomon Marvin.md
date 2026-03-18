---
type: npc
game: cyberpunk-red
identity:
  name: Solomon Marvin
  role: Bodyguard
  threat: Alta
combat:
  combat_number: 14
  initiative: 10
  mi: 23
  dr: 1
health:
  hp: 45
armor:
  head: 7
  body: 7
weapons:
  - name: Pistola a Doppio Funzionamento Militech Fox
    damage: 4d6
    rof: 1
    hands: 1
    ammo: 10 + 10
  - name: Mascella da combattimento
    damage: 4d6
    rof: 1
    hands: 0
  - name: Nocche blindate
    damage: 2d6
    rof: 2
    hands: 1
  - name: Piede artigliato
    damage: 2d6
    rof: 2
    hands: 0
cyberware:
  - Mascella da combattimento
  - Piede artigliato (x2)
  - Nocche blindate (x2)
  - Filtri nasali
  - Filtri antitossine
  - Skin Weave
  - Cyberbraccio (x2)
  - Cybergamba (x2)
  - Innesto cambio rapido
---
[[#Background]]
[[#Personalità]]
[[#Ai giorni nostri]]
[[#Scheda personaggio]]

---
#### Background
Solomon è una guardia del corpo dipendente di [[Militech]] e assegnata alla protezione di [[Aiden|Aiden]] nel 2045. 
Solomon convive con Aiden in un appartamento a Little Europe pagato da Militech, provvedendo protezione h24. 

---
#### Personalità
Solomon è una guardia del corpo efficiente e brutale. Difficilmente si lascia andare a commenti che non abbiano risvolto pratico e si dimostra senza scrupoli quando ha a che fare con delle minacce per la sicurezza dell'assistito.

---
#### Ai giorni nostri
##### 2045
Il 14 gennaio 2045 la crew tende un'imboscata all'appartamento di Aiden a Little Europe. Nel processo, Solomon viene ucciso cercando di proteggere l'assistito. Aiden verrà conseguentemente rapito. 

---
#### Scheda personaggio

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
