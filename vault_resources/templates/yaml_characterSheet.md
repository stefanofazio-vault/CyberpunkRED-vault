---
type: character
game: cyberpunk-red

identity:
  name: <NOME PG>
  handle: <HANDLE PG>
  role: <RUOLO PG>

stats:
  INT: 6
  RIF: 6
  DEX: 6
  TEC: 6
  CAR: 6
  VOL: 6
  FOR: 6
  VEL: 6
  FIS: 6
  EMP: 6

hp:
  current: 0
  death_save_penalty: 0

derived:
  death_save_base: FIS
  
equipment:
  weapons:
    - name: <NOME ARMA>
      type: <TIPO ARMA>
      damage: <Xd6>
      rof: <VAL>
      hands: <VAL>
      quality: <QUALITY>
      notes: ""

  armor:
    head:
      name: <NAME>
      sp: <VAL>
      penalty: <VAL>
    body:
      name: <NAME>
      sp: <VAL>
      penalty: <VAL>

  gear:
    - name: <NAME>
      description: <DESC>


skills:
  athletics:
    label: Athletics
    stat: DEX
    value: 6
    category: body
  brawling:
    label: Brawling
    stat: DEX
    value: 4
    category: fighting
  evasion:
    label: Evasion
    stat: DEX
    value: 8
    category: fighting
  handguns:
    label: Handgun
    stat: REF
    value: 10
    category: fighting
  melee:
    label: Melee Weapon
    stat: DEX
    value: 6
    category: fighting
  perception:
    label: Perception
    stat: INT
    value: 8
    category: awareness
  stealth:
    label: Stealth
    stat: DEX
    value: 7
    category: awareness

  
cyberware:
  neural:
    - name: <NAME>
      hl: <VAL>
      notes: <DESC>
    - name: <NAME>
      hl: <VAL>
      notes: <DESC>
    - name: <NAME>
      hl: <VAL>
      notes: <DESC>
    - name: <NAME>
      hl: <VAL>
      notes: <DESC>
    - name: <NAME>
      hl: <VAL>
      notes: <DESC>

  cyberarm_dx:
    - name: <NAME>
      hl: <VAL>
      options:
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>

  cyberarm_sx:
    - name: <NAME>
      hl: <VAL>
      options:
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>

  cyberoptics_dx:
    - name: <NAME>
      hl: <VAL>
      options:
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>

  cyberoptics_sx:
    - name: <NAME>
      hl: <VAL>
      options:
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>

  cyberaudio:
    - name: <NAME>
      hl: <VAL>
      options:
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>

  cyberleg_dx:
    - name: <NAME>
      hl: <VAL>
      options:
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>

  cyberleg_sx:
    - name: <NAME>
      hl: <VAL>
      options:
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>
        - name: <NAME>
          hl: <VAL>
          notes: <DESC>

  internal:
    - name: <NAME>
      hl: <VAL>

  external:
    - name: <NAME>
      hl: <VAL>

  fashion:
    - name: <NAME>
      hl: <VAL>

  borgware:
    - name: <NAME>
      hl: <VAL>
---
