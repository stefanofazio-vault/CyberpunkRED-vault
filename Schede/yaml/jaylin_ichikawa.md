---
type: character
game: cyberpunk-red

identity:
  name: Jaylin Ichikawa
  handle: Jaylin
  
roles:
  - label: Corpo
    rank: 7
  - label: Solo
    rank: 4

stats:
  INT: 8
  RIF: 6
  DES: 7
  TEC: 5
  CAR: 8
  VOL: 5
  FOR: 3
  VEL: 7
  FIS: 12
  EMP: 5

hp:
  current: 0
  death_save_penalty: 0

derived:
  death_save_base: FIS

armor:
  head:
    name: Corazza leggera
    sp: 11
    ablation: 0
  body:
    name: Corazza leggera
    sp: 11
    ablation: 0

equipment:
  weapons:
    - name: Arasaka WAA AR
      type: Fucile d'assalto
      damage: 5d6
      rof: 1
      hands: 2
      quality: Standard
      notes: Dotato di connettore smartgun

skills:
  # ARTISTICHE
  recitare:
    label: Recitare
    stat: CAR
    value: 8
    category: Artistiche

  musica:
    label: Musica
    stat: EMP
    value: 0
    category: Artistiche

  # ATTENZIONE
  concentrazione:
    label: Concentrazione
    stat: VOL
    value: 7
    category: Attenzione

  percezione:
    label: Percezione
    stat: INT
    value: 7
    category: Attenzione

  seguire_tracce:
    label: Seguire Tracce
    stat: INT
    value: 0
    category: Attenzione

  nascondere_trovare_oggetti:
    label: Nascondere/Trovare Oggetti
    stat: INT
    value: 0
    category: Attenzione

  leggere_labbra:
    label: Leggere le Labbra
    stat: INT
    value: 0
    category: Attenzione

  # COMBATTIMENTO A DISTANZA
  tiro_arco:
    label: Tiro con l'Arco
    stat: RIF
    value: 0
    category: Combattimento a distanza

  fuoco_automatico:
    label: Fuoco Automatico
    stat: RIF
    value: 4
    category: Combattimento a distanza

  pistole:
    label: Pistole
    stat: RIF
    value: 4
    category: Combattimento a distanza

  armi_pesanti:
    label: Armi Pesanti
    stat: RIF
    value: 0
    category: Combattimento a distanza

  armi_spalla:
    label: Armi a Spalla
    stat: RIF
    value: 8
    category: Combattimento a distanza

  # COMBATTIMENTO RAVVICINATO
  rissa:
    label: Rissa
    stat: DES
    value: 0
    category: Combattimento ravvicinato

  elusione:
    label: Elusione
    stat: DES
    value: 6
    category: Combattimento ravvicinato

  armi_mischia:
    label: Armi da Mischia
    stat: DES
    value: 0
    category: Combattimento ravvicinato

  arti_marziali:
    label: Arti Marziali
    stat: DES
    value: 6
    category: Combattimento ravvicinato

  # CONTROLLO
  guidare:
    label: Guidare Veicoli Terrestri
    stat: RIF
    value: 0
    category: Controllo

  pilotare_aeromobili:
    label: Pilotare Aeromobili
    stat: RIF
    value: 0
    category: Controllo

  pilotare_imbarcazioni:
    label: Pilotare Imbarcazioni
    stat: RIF
    value: 0
    category: Controllo

  cavalcare:
    label: Cavalcare
    stat: RIF
    value: 0
    category: Controllo

  # FISICHE
  atletica:
    label: Atletica
    stat: DES
    value: 7
    category: Fisiche

  contorsionismo:
    label: Contorsionismo
    stat: DES
    value: 0
    category: Fisiche

  danza:
    label: Danza
    stat: DES
    value: 6
    category: Fisiche

  tempra:
    label: Tempra
    stat: VOL
    value: 5
    category: Fisiche

  resistere_tortura_droghe:
    label: Resistere a Tortura/Droghe
    stat: VOL
    value: 9
    category: Fisiche

  furtivita:
    label: Furtività
    stat: DES
    value: 5
    category: Fisiche

  # ISTRUZIONE
  contabilita:
    label: Contabilità
    stat: INT
    value: 8
    category: Istruzione

  allevamento:
    label: Allevamento
    stat: INT
    value: 0
    category: Istruzione

  burocrazia:
    label: Burocrazia
    stat: INT
    value: 0
    category: Istruzione

  business:
    label: Business
    stat: INT
    value: 8
    category: Istruzione

  comporre:
    label: Comporre
    stat: INT
    value: 0
    category: Istruzione

  criminologia:
    label: Criminologia
    stat: INT
    value: 8
    category: Istruzione

  crittografia:
    label: Crittografia
    stat: INT
    value: 8
    category: Istruzione

  deduzione:
    label: Deduzione
    stat: INT
    value: 3
    category: Istruzione

  gioco_azzardo:
    label: Gioco d’Azzardo
    stat: INT
    value: 0
    category: Istruzione

  linguaggio:
    label: Linguaggio
    stat: INT
    value: 0
    category: Istruzione

  archivistica:
    label: Archivistica
    stat: INT
    value: 0
    category: Istruzione

  conoscenza_zona:
    label: Conoscenza della zona
    stat: INT
    value: 0
    category: Istruzione

  scienza:
    label: Scienza
    stat: INT
    value: 0
    category: Istruzione

  tattica:
    label: Tattica
    stat: INT
    value: 0
    category: Istruzione

  survivalismo:
    label: Survivalismo
    stat: INT
    value: 0
    category: Istruzione

  istruzione:
    label: Istruzione
    stat: INT
    value: 5
    category: Istruzione

  # Sociali
  corrompere:
    label: Corrompere
    stat: CAR
    value: 6
    category: Sociali

  conversazione:
    label: Conversazione
    stat: EMP
    value: 10
    category: Sociali

  sensibilita:
    label: Sensibilità
    stat: EMP
    value: 6
    category: Sociali

  interrogatorio:
    label: Interrogatorio
    stat: CAR
    value: 8
    category: Sociali

  persuasione:
    label: Persuasione
    stat: CAR
    value: 4
    category: Sociali

  cura_persona:
    label: Cura della Persona
    stat: CAR
    value: 4
    category: Sociali

  scaltrezza:
    label: Scaltrezza
    stat: CAR
    value: 4
    category: Sociali

  commercio:
    label: Commercio
    stat: CAR
    value: 6
    category: Sociali

  guardaroba_stile:
    label: Guardaroba e Stile
    stat: CAR
    value: 6
    category: Sociali

  # TECNICHE
  tecnologia_base:
    label: Tecnologia di Base
    stat: TEC
    value: 0
    category: Tecniche

  cybertecnologia:
    label: Cybertecnologia
    stat: TEC
    value: 8
    category: Tecniche

  pronto_soccorso:
    label: Pronto Soccorso
    stat: TEC
    value: 0
    category: Tecniche

  tecnologia_aeromobili:
    label: Tecnologia degli Aeromobili
    stat: TEC
    value: 0
    category: Tecniche

  demolizioni:
    label: Demolizioni
    stat: TEC
    value: 0
    category: Tecniche

  elettronica_sicurezza:
    label: Elettronica e Sicurezza
    stat: TEC
    value: 0
    category: Tecniche

  falsificare:
    label: Falsificare
    stat: TEC
    value: 0
    category: Tecniche

  tecnologia_veicoli_terrestri:
    label: Tecnologia dei Veicoli Terrestri
    stat: TEC
    value: 0
    category: Tecniche

  belle_arti:
    label: Belle Arti
    stat: TEC
    value: 0
    category: Tecniche

  paramedico:
    label: Paramedico
    stat: TEC
    value: 0
    category: Tecniche

  fotografia:
    label: Fotografia
    stat: TEC
    value: 0
    category: Tecniche

  scassinare:
    label: Scassinare
    stat: TEC
    value: 0
    category: Tecniche

  borseggiare:
    label: Borseggio
    stat: TEC
    value: 0
    category: Tecniche

  tecnologia_imbarcazioni:
    label: Tecnologia delle Imbarcazioni
    stat: TEC
    value: 0
    category: Tecniche

  tecnologia_armi:
    label: Tecnologia delle Armi
    stat: TEC
    value: 0
    category: Tecniche


cyberware:
  neural:
    - name: Collegamento neurale
      hl: 7
      options:
        - name: Coprocessore di riflessi
          hl: 7
          notes: Permette di schivare proiettili senza RIF 8
        - name: Alveolo
          hl: 7
          notes: Permette di utilizzare chip
        - name: Antidolorifico
          hl: 7
          notes: Ignora i malus di Ferito Gravemente
        - name: Sandevistan
          hl: 14
          notes: +3 Iniziativa per 20 Round

  cyberarm_dx:
    - name: Cyberbraccio
      hl: 7
      options:
        - name: Presa sottocutanea
          hl: 3
          notes: Collegamento Smartgun

  cyberoptics_dx:
    - name: Cyberocchio
      hl: 3
      options:
        - name: Bassa Luminosità / Infrarosso / UV
          hl: 7

  cyberoptics_sx:
    - name: Cyberocchio
      hl: 3
      options:
        - name: Bassa Luminosità / Infrarosso / UV
          hl: 7

  internal:
    - name: Telaio Lineare Sigma
      hl: 14
      notes: Porta FIS a 12
    - name: Filtro Antitossine
      hl: 3
      notes: +2 Resistere Tortura/Droghe
    - name: Biomonitor
      hl: 3
      notes: Monitora stato di salute
---
