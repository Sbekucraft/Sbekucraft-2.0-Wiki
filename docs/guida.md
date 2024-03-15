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
Con il passaggio a paper, nel server è stato introdotto il framework economico [xConomy](https://www.spigotmc.org/resources/xconomy.75669/) che introduce una valuta, la *Lore* (al plurale sempre *Lore*). Questa valuta cerca di standardizzare le transazioni tra giocatori e dare un senso di progressione ai claim. In futuro, questa valuta sarà integrata con funzionalità aggiuntive che permetteranno di comprare funzionalità di "flavour" che non vanno ad intaccare gli equilibri di gioco.

I comandi principali da conoscere sono `/balance` per controllare il proprio bilancio e `/pay <giocatore> <quantità>` per inviare soldi ad un altro giocatore.

Ogni 24 ore verranno accreditati a tutti i giocatori registrati 400 lore fino ad un tetto massimo di 250k lore, indipendentemente dall'attività sul server.

## Claim
In seguito al rework del server, per creare dei claim è necessario disporre di una certa quantità di Lore.
Il costo dell'area è di 1.5 lore per blocco, e quando proverai a claimare un'area che non puoi permetterti verrà esplicitata la quantità di lore necessaria.

Per creare un claim devi prima definire l'area da claimare. Per farlo, ti consigliamo di usare della lana, o dei blocchi facilmente riconoscibili per definire gli estremi del claim; poi mettiti sopra al primo vertice dell'area da claimare e usa `//pos1`, poi usa `//pos2` sul vertice opposto. Una volta selezionata l'area, puoi creare un claim tramite il comando `/lc claim <Nome dell'area>`. L'area claimata si estenderà lungo tutto l'asse verticale, dalla bedrock fino al limite di altezza.

Puoi aprire un'interfaccia contentenente tutto ciò che riguarda i claim con `/lc`, tramite cui sarà anche possibile aggiungere giocatori al tuo claim. 

L'area claimata non è necessariamente quadrata, è possibile claimare un'area rettangolare fino a un rapporto di 9:1. Per estendere un claim, basta crearne un altro accanto. Tuttavia, una singola regione non può eccedere un'area di 160801 blocchi, ovvero poco 628 chunk.

## PvP
Il PvP nel server è disattivato di base. Per attivarlo basta usare il comando `/pvp on`, e per disattivarlo `/pvp off`.
Due giocatori possono entrare in combattimento quando entrambi hanno il pvp attivato e, se sono in un claim, soltanto se il claim ha il pvp attivo.

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
- La notte passa più velocemente in base a quanti giocatori stanno dormendo. Superati il 60% dei giocatori verrà comunque saltata automaticamente.

Queste mod semplificano la vita dei giocatori velocizzando alcuni processi lenti o tediosi, senza però modificare gli aspetti fondamentali del gioco.

**Puoi trovare la lista completa dei plugin nell'[apposita sezione](content.md).**

## Compatiblità client side
Il server offre le stesse possibilità a giocatori Bedrock e Java (Vanilla e non), tuttavia è possibile inserire compatibilità a mod client side che richiedono anche la controparte server, fin quando la mod non crea disuguaglianze e/o diminiuisce l'esperienza dei giocatori vanilla.
Attualmente vi è compatibilità lato server per le seguenti mod:

- [Xaero's Minimap](https://modrinth.com/mod/xaeros-minimap)

## Proporre nuovi plugin 
Le proposte sono sempre benvenute ma ci sono alcune regole da rispettare: 

- il plugin deve poter funzionare solo lato server affinché sia possibile mantenere la compatibilità con Bedrock,
- il plugin non deve modificare in modo eccessivo l'esperienza di gioco, che vogliamo resti un *Vanilla+*.

Per qualsiasi proposta ti invitiamo ad entrare nel [gruppo Telegram](https://t.me/sbekucraft/40112) e di parlarne con i moderatori.
