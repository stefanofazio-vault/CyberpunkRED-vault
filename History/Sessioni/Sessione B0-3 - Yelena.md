### Premessa
Durante una sessione di gioco su Elflines Online, Yelena riceve un messaggio in chat privata da parte di un account nascosto. Il messaggio recita quanto segue:
"Buongiorno, Yelena. Ho un lavoro per te. Ho bisogno che tu installi un virus nell'architettura di rete del [[Watson Residence]]. Il virus deve concedermi l'accesso alle telecamere. La paga è buona. Qualunque file troverai nell'architettura potrebbe interessarmi e potrebbe portarti ad un bonus."
### Svolgimento
Il Watson Residence è un complesso abitativo di medio livello, consistente in tre piani con due appartamenti per piano. 

Il *residence* è situato all'angolo di un incrocio di due strade abbastanza importanti del distretto.

Offre, al piano terra, un atrio che può fungere da punto di ritrovo, munito di un piccolo bar e di una *lounge* dotata di divanetti di varie dimensioni. Varie persone (nell'ordine della dozzina) stanno frequentando l'atrio. 

Il *residence* è munito di una piccola squadra di sorveglianza privata (composta di due guardie) che pattuglia tutti i piani cercando elementi di disturbo. Le guardie cambiano piano ogni tre minuti circa. Salgono e scendono di continuo, senza usare l'ascensore.

---

![[Vigilanza privata - SB]]

---

Il *residence* è munito di telecamere interne ed esterne. Nessuno le sta attivamente monitorando (non c'è sufficiente sicurezza) ma se non vengono gestite sarà evidente l'intromissione di un intruso.

Una delle stanze è attualmente vuota ed è disponibile all'affitto. L'affitto per il mese costa 1000 €$. 
Ogni stanza è dotata di un *access point* connesso ad un *tablet* che permette di ordinare bevande dal bar al piano terra.

Il piano terra dispone di un *access point* scoperto che precedentemente era collegato ad un distributore di bevande che è stato disconnesso quando è stato aperto il bar. 

Il terzo piano dispone di un *access point* che permette di eseguire la diagnostica degli impianti dell'edificio. 

Inoltre, sempre al terzo piano, c'è un piccolo ufficio per l'amministratore di condominio che in questo momento è presente.

L'architettura di rete dell'edificio è la seguente:

| Livello | Contenuto                     |
| ------- | ----------------------------- |
| 1       | Password DV6                  |
| 2       | Password DV8                  |
| 3       | Asp                           |
| 4       | File DV6                      |
| 5       | Raven                         |
| 6       | Wisp                          |
| 7       | Control Node DV8 (telecamere) |
| 8       | File DV10                     |

La password del primo livello può essere trovata annotata al bar del piano terra. 
La password del secondo livello, invece, è annotata nell'ufficio dell'amministratore di condominio.
Il file del quarto livello contiene una lista dei residenti. 
Il file dell'ottavo livello, invece, contiene le registrazioni degli ultimi tre giorni delle telecamere.

### Conclusione
Quando Yelena uscirà dall'edificio, riceverà un messaggio dallo stesso utente che la ha contattata su Elflines. Questo messaggio chiederà di consegnare i dati in uno *shard* presso gli [[University Cubes]]. Qui, sarà presente la paga e la proposta di appuntamento.