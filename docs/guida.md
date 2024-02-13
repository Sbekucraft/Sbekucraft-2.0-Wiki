# Guida al server

## Primo accesso al server 
Per avere accesso al server è necessario **essere abbonati a Twitch (anche Prime), Patreon (qualsiasi tier) o YouTube** ed effettuare il login dal sito di [whitelist](https://whitelist.sbekucraft.it). 
Se sei un abbonato di YouTube non è ancora presente il sistema di whitelist automatico tramite il sito, ti invitiamo a scrivere ai moderatori tramite il [gruppo Telegram](https://t.me/sbekucraftchat).

## Mappa del server
Tramite la mod Dynmap è possibile visualizzare tramite web una [mappa del server](https://map.sbekucraft.it) completa di tutti i chunk attualmente esplorati.
Questo perché mentre i giocatori della Java edition possono usare mod come journeymap, bluemap, etc.. per avere una mappa locale, i giocatori bedrock non possono installare mod.
Questa mappa cerca di bilanciare la situazione.

Di default la mappa mostra la posizione degli altri giocatori nella mappa, ma è possibile utilizzare il comando `/dynmap hide` per nascondersi, e `/dynmap show` per essere nuovamente visibili.

Inoltre è possibile creare dei marker personalizzati sulla mappa tramite dei normali cartelli.
Per farlo, la prima riga deve contenere: *[dynmap]*, la seconda il nome del marker e la terza *icon:icona*. Si può trovare l'elenco delle icone disponibili [qua](https://camo.githubusercontent.com/29c0ba4976a7db3d89d141ab38fd0dcb6126e994fd9d43d2e6341010b89679c6/687474703a2f2f6d696b657072696d6d2e636f6d2f696d616765732f4d61726b6572732e706e67).

## Claim
Il server contiene la mod [Get Off My Lawn](https://github.com/Patbox/get-off-my-lawn-reserved) per gestire i claim.
Questa mod unisce funzionalità e gameplay, in quanto per aumentare l'area del tuo claim dovrai usare degli augment che necessitano diversi materiali di upgrade.
Puoi trovare un ricettario della mod in [questa](https://github.com/Patbox/get-off-my-lawn-reserved/blob/1.19.4/recipes.md) pagina.
Si possono aggiungere persone al claim interagendo con l'anchor del claim, ed è anche possibile attivare il pvp.

Inoltre è presente un plugin che collega Get Off My Lawn e Dynmap, dunque è possibile visualizzare i claim sulla mappa.

## PvP
Il PvP nel server è disattivato di base. Per attivarlo basta usare il comando `/pvp on`, e per disattivarlo `/pvp off`.
Due giocatori possono entrare in combattimento quando entrambi hanno il pvp attivato e, se sono in un claim, soltanto se il claim ha l'augment del PvP control attivato.

## Generazione del mondo
Per incentivare l'esplorazione abbiamo aggiunto diverse strutture ognuna con i propri reward sia nell'overworld che nelle altre dimensioni.
Inoltre, visto il nerf dei villager della 1.20.2, i villaggi dovrebbero essere un po' più frequenti e distinti da quelli vanilla.
Puoi capire che strutture sono presenti nel mondo guardando la lista completa di plugin, ma noi ti consigliamo di esplorare e trovarle in "blind".

**Nota**: Il tetto del nether non è più raggiungibile.

## Cross Platform Compatibility
Il server è aperto sia a giocatori della versione Java che a giocatori della versione bedrock grazie al plugin [GeyserMC](https://geysermc.org/).
Puoi capire se un giocatore sta usando la versione bedrock grazie al prefisso `.` prima del nome. Quindi `.Username`, è un username bedrock.
Tutte le mod indicate sono installate lato server, e dunque sono automaticamente compatibili anche con i client bedrock.

**Se giochi da Bedrock su console (Xbox, Switch o Playstation) è necessario modificare delle impostazioni di rete per poter accedere, in quanto Microsoft di base non permette l'accesso a server minecraft non approvati.**
Trova le impostazioni di rete della console, e modifica le seguenti impostazioni:

- Impostazioni DNS: Manuali
- DNS Primario: 57.129.16.229
- DNS Secondario: 1.1.1.1

A questo punto dovresti poter vedere il server nella tua lista di server, al posto di uno dei server approvati da Microsoft.

## Quality of life
Nel server sono presenti alcune mod di quality of life:

- [*harvest with ease*](https://modrinth.com/mod/harvest-with-ease) permette di prendere ortaggi dall'orto premendo il tasto destro con una falce in mano;
- [*tree harvester*](https://modrinth.com/mod/tree-harvester) permette di distruggere un albero intero semplicemente distruggendo i suoi blocchi inferiori se tieni un'ascia in mano; 
- [*extended bone meal*](https://modrinth.com/mod/extended-bone-meal) permette di usare la farina d'ossa su tutte le piante del gioco. Inoltre usare la farina d'ossa da accovacciati con abbastanza stack nell'inventario userà tanta farina quanta necessaria per far crescere la pianta fino alla maturazione completa;
- [*anvil restoration*](https://modrinth.com/mod/anvil-restoration) ti permette di riparare le incudini interagendovi con un lingotto di ferro in mano;
- [*fixed anvil repair cost*](https://modrinth.com/mod/fixed-anvil-repair-cost) limita i livelli massimi necessari per riparare degli utensili incantati a 5 livelli.

Queste mod semplificano la vita dei giocatori velocizzando alcuni processi lenti o tediosi, senza però modificare gli aspetti fondamentali del gioco.

**Puoi trovare la lista completa delle mod nell'[apposita sezione](content.md).**

## Compatiblità client side
Il server offre le stesse possibilità a giocatori Bedrock e Java (Vanilla e non), tuttavia è possibile inserire compatibilità a mod client side che richiedono anche la controparte server, fin quando la mod non crea disuguaglianze e/o diminiuisce l'esperienza dei giocatori vanilla.
Attualmente vi è compatibilità lato server per le seguenti mod:

- [Roughly Enough Items](https://modrinth.com/mod/rei)
- [AppleSkin](https://modrinth.com/mod/appleskin)
- [Xaero's Minimap](https://modrinth.com/mod/xaeros-minimap)

## Proporre nuove mod 
Le proposte sono sempre benvenute ma ci sono alcune regole da rispettare: 

- la mod deve poter funzionare solo lato server affinché sia possibile mantenere la compatibilità con Bedrock,
- la mod non deve modificare in modo eccessivo l'esperienza di gioco, che vogliamo resti un *Vanilla+*.

Per qualsiasi proposta ti invitiamo ad entrare nel [gruppo Telegram](https://t.me/sbekucraftchat) e di parlarne con i moderatori.
