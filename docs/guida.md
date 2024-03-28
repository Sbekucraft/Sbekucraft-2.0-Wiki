# Guida al server

Il server è basato sulla **versione di Minecraft 1.20.4** è accessibile sia tramite Java che tramite Bedrock tramite i seguenti IP:

- **Java**: server.sbekucraft.it:25565
- **Bedrock**: server.sbekucraft.it:19132

## Primo accesso al server 
Per avere accesso al server è necessario **essere abbonati a Twitch (anche Prime), Patreon (qualsiasi tier) o YouTube** ed effettuare il login dal sito di [whitelist](https://whitelist.sbekucraft.it). 
Se sei un abbonato di YouTube non è ancora presente il sistema di whitelist automatico tramite il sito, ti invitiamo a scrivere ai moderatori tramite il [gruppo Telegram](https://t.me/sbekucraft).

## Mappa del server
Tramite la mod [pl3xmap](https://modrinth.com/plugin/pl3xmap) è possibile visualizzare tramite web una [mappa del server](https://map.sbekucraft.it) completa di tutti i chunk attualmente esplorati.
Questo perché mentre i giocatori della Java edition possono usare mod come journeymap, xaero's map , etc.. per avere una mappa locale, i giocatori bedrock non possono installare mod.
Questa mappa cerca di bilanciare la situazione.

Di default la mappa mostra la posizione degli altri giocatori nella mappa, ma è possibile utilizzare il comando `/map hide` per nascondersi, e `/map show` per essere nuovamente visibili.

## Economia
Con il passaggio a paper, nel server è stato introdotto il framework economico [xConomy](https://www.spigotmc.org/resources/xconomy.75669/) che introduce due valute, la *Lore* (al plurale sempre *Lore*) e lo *sbeuro* (al plurale *sbeuri*). Queste valute cercano di standardizzare le transazioni tra giocatori e dare un senso di progressione ai claim. La valuta principale è la lore, per cui le transazioni con il server dovranno essere effettuate in lore, mentre per le transazioni tra giocatori sarà possibile usare qualunque valuta si voglia.

I comandi principali da conoscere sono `/lore` per controllare il proprio bilancio in lore e `/lore send <utente>` per inviare soldi ad un altro utente. Questi comandi esistono anche per gli sbeuri, con il corrispettivo `/sbeuro`. Inoltre per cambiare soldi da lore a sbeuri basta usare `/lore exchange sbeuro <quantità>`, viceversa per cambiare da sbeuri a lore, ricordando che i tassi di cambio sono di 20 sbeuri = 1 lore.

Ogni 24 ore verranno accreditati a tutti i giocatori registrati 400 lore fino ad un tetto massimo di 250k lore, indipendentemente dall'attività sul server.

## Skill Passive
Per permettere agli utenti passivi di guadagnare più soldi ed avere un'esperienza più dinamica, abbiamo introdotto un sistema di skill passive, ognuna con il proprio livello, obbiettivi e reward.

Ai giocatori verrà attribito un reward in sbeuri ogni volta che avviene un level-up ed ogni volta che viene completato un obbiettivo.

Attualmente le skill disponibili sono **caccia**, **estrazione** e **coltivazione**.

## Claim
In seguito al rework del server, per creare dei claim è necessario disporre di una certa quantità di Lore.
Il costo dell'area è di 1.5 lore per blocco, e quando proverai a rivendicare un'area che non puoi permetterti verrà esplicitata la quantità di lore necessaria.

Per creare un claim devi prima definire l'area da rivendicare. Per farlo, ti consigliamo di usare della lana, o dei blocchi facilmente riconoscibili per definire gli estremi del claim (in quanto non sarà possibile vedere i limiti dell'area successivamente), poi puoi proseguire in due modi:

- Mettiti sopra al primo vertice dell'area da rivendicare e usa `//pos1`, poi usa `//pos2` sul vertice opposto.
- Prendi in mano un bastone e usa il tasto *rompi blocco* (click sinistro) sul primo vertice dell'area da rivendicare, poi, sempre col bastone in mano usa il tasto *interazione* (click destro) sul vertice opposto.
 
Una volta selezionata l'area, puoi creare un claim tramite il comando `/lc claim <Nome dell'area>`. L'area rivendicata si estenderà lungo tutto l'asse verticale, dalla bedrock fino al limite di altezza.

Puoi aprire un'interfaccia contentenente tutto ciò che riguarda i claim con `/lc`, tramite cui sarà possibile aggiungere giocatori al tuo claim, modificare i permessi del tuo claim e ridimensionarne l'area.

Per ridimensionare un'area rivendicata, basta usare gli stessi metodi già descritti per selezionare l'area ampliata e poi andare nell'apposita sezione in `/lc`, selezionando l'area da modificare e poi la voce "Ridimensiona Area". Il server calcolerà automaticamente la differenza di prezzo tra le due aree.

**Nota I: L'area rivendicata non è necessariamente quadrata, è possibile rivendicare un'area rettangolare fino a un rapporto di 9:1. Tuttavia, una singola regione non può eccedere un'area di 160801 blocchi, ovvero circa 628 chunk.**

**Nota II: se utilizzi il modpack potrai notare l'area che viene mostrata dinamicamente. Una volta finito di rivendicare, per deselezionare l'area puoi usare** `//desel` **.**

**Nota III: attualmente è possibile ridimensionare soltanto le regioni, non i plot.**

## PvP
Il PvP nel server è disattivato di base. Per attivarlo basta usare il comando `/pvp on`, e per disattivarlo `/pvp off`.
Due giocatori possono entrare in combattimento quando entrambi hanno il pvp attivato e, se sono in un claim, soltanto se il claim ha il pvp attivo.

## Funzionalità aggiuntive
Alcune funzionalità aggiuntive, esterne all'esperienza vanilla, si interfacciano con il sistema economico, e vengono considerate come "sfizi" per i giocatori più ricchi. Queste includono:

- ImageFrame, importa delle immagini nella tua base. Questa funzionalità è disponibile tramite il comando `/imageframe <nome immagine> <link> <larghezza> <altezza> combined`. Questo comando spawnerà una mappa nell'inventario del giocatore, e cliccando nell'angolo in alto a sinistra dei frame, questi verranno automaticamente riempiti. Larghezza ed altezza, si riferiscono al numero di frame da riempire.

NB: Nel caso in cui venga utilizzata una sinstassi incorretta nel comando, per limitazioni di integrazione non è possibile stornarne il costo. Assicurati di utilizzare la sintassi corretta.

## Cross Platform Compatibility
Il server è aperto sia a giocatori della versione Java che a giocatori della versione bedrock grazie al plugin [GeyserMC](https://geysermc.org/).
Puoi capire se un giocatore sta usando la versione bedrock grazie al prefisso `.` prima del nome. Quindi `.Username`, è un username bedrock.
Tutte le mod indicate sono installate lato server, e dunque sono automaticamente compatibili anche con i client bedrock.

**Se giochi da Bedrock su console (Xbox, Switch o Playstation) è necessario modificare delle impostazioni di rete per poter accedere, in quanto Microsoft di base non permette l'accesso a server minecraft non approvati.**
Trova le impostazioni di rete della console, e modifica le seguenti impostazioni:

- Impostazioni DNS: Manuali
- DNS Primario: `57.129.16.229`
- DNS Secondario: `1.1.1.1`

A questo punto dovresti poter vedere il server nella tua lista di server, al posto di uno dei server approvati da Microsoft.

## Quality of life
Nel server sono presenti alcune funzionalità di quality of life:

- Prendere ortaggi dall'orto premendo il tasto destro li ripianta automaticamente;
- Si può distruggere un albero intero semplicemente distruggendo i suoi blocchi inferiori se tieni un'ascia in mano; 
- Limita i livelli massimi necessari per riparare degli utensili incantati a 10 livelli.
- Tenere una torcia in mano crea luce attorno a te.
- Tutte le ricette risultano immediatamente sbloccate.
- Aprire o chiudere una doppia porta apre o chiude entrambe le porte.

Queste mod semplificano la vita dei giocatori velocizzando alcuni processi lenti o tediosi, senza però modificare gli aspetti fondamentali del gioco.

**Puoi trovare la lista completa dei plugin nell'[apposita sezione](content.md).**

## Chat Vocale di Prossimità
La chat vocale è compatibile sia con client java che con client bedrock che usa una pagina web per creare un canale di comunicazione esterno tra giocatori. Questi sono i passaggi per accedervi:

- Per la versione **Java**, una volta entrato in partita riceverai un messaggio che ti chiede di "Cliccare qui" per abilitare la chat vocale; cliccando sul messaggio verrai indirizzato verso una pagina web in cui dovrai dare accesso al microfono, ed automaticamente verrai connesso alla chat vocale.
- Per la versione **Bedrock**, ti verrà inviato lo stesso messaggio, ma non potendo cliccare sui messaggi è necessario navigare manualmente su [session.openaudiomc.net](https://session.openaudiomc.net), e cliccare sul pulsante *continue to bedrock login* e dare i permessi al browser; dunque, la pagina ti mostrerà un codice (token) da inserire ingame con il comando `/audio <codice>`. A quel punto il procedimento continuerà come per java e verrai connesso alla chat vocale.

Una delle funzionalità della chat vocale è quella di creare dei canali di comunicazione privati (accesso su invito) con i rispettivi comandi:

- `/channel create <canale>`, per creare un canale.
- `/channel leave`, per uscire dal canale a cui si è connessi.
- `/channel invite <giocatore>`, per invitare altri ad un canale. 
- `/channel join <canale>`, per entrare in un canale vocale.

Per *uscire* dalla chat vocale basta chiudere la pagina del browser.

## Compatiblità client side
Il server offre le stesse possibilità a giocatori Bedrock e Java (Vanilla e non), tuttavia è possibile inserire compatibilità a mod client side che richiedono anche la controparte server, fin quando la mod non crea disuguaglianze e/o diminiuisce l'esperienza dei giocatori vanilla.
Attualmente vi è compatibilità lato server per le seguenti mod:

- [Xaero's Minimap](https://modrinth.com/mod/xaeros-minimap)

## Proporre nuovi plugin 
Le proposte sono sempre benvenute ma ci sono alcune regole da rispettare: 

- il plugin deve poter funzionare solo lato server affinché sia possibile mantenere la compatibilità con Bedrock,
- il plugin non deve modificare in modo eccessivo l'esperienza di gioco, che vogliamo resti un *Vanilla+*.

Per qualsiasi proposta ti invitiamo ad entrare nel [gruppo Telegram](https://t.me/sbekucraft/40112) e di parlarne con i moderatori.
