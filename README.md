# 1.1 Che cos'è un sistema operativo?

Un **sistema operativo (SO)** è un insieme di programmi software che gestisce le risorse hardware di un computer e fornisce servizi comuni ai programmi applicativi.

## Funzioni principali del sistema operativo:

- **Gestione delle risorse hardware:** processore, memoria, dispositivi di input/output (dischi, tastiera, schermo, ecc.).
- **Gestione dei processi:** crea, pianifica, e termina i processi, garantendo l'esecuzione corretta e coordinata di più programmi.
- **Gestione della memoria:** assegna e libera la memoria ai processi, mantenendo il controllo sull’accesso e l’isolamento.
- **Gestione del file system:** organizza, salva e recupera i dati dai dispositivi di memorizzazione.
- **Interfaccia utente:** fornisce un’interfaccia (testuale o grafica) che consente all’utente di interagire con il computer.

In sintesi, il sistema operativo è il **software di base** che fa da intermediario tra l’utente, i programmi applicativi e l’hardware, garantendo che tutte le parti funzionino correttamente e in modo efficiente.

# 1.2 Qual è uno dei compiti principali del sistema operativo?

Uno dei compiti principali del sistema operativo è la **gestione delle risorse del sistema**.

In particolare, il sistema operativo si occupa di:

- Allocare e liberare risorse hardware come CPU, memoria, dispositivi di I/O.
- Gestire l’esecuzione dei processi, assicurando che più programmi possano funzionare contemporaneamente senza interferenze.
- Coordinare l’accesso ai dispositivi di memorizzazione e garantire la sicurezza e l’integrità dei dati.

In pratica, il sistema operativo funge da **gestore e controllore delle risorse**, ottimizzando l’utilizzo dell’hardware e offrendo ai programmi e agli utenti un ambiente stabile e efficiente.

# 1.3 Quale delle seguenti opzioni rappresenta una tipica struttura gerarchica della memoria?

La **struttura gerarchica della memoria** è organizzata in livelli, ognuno con caratteristiche di velocità, capacità e costo diversi. Tipicamente, la gerarchia della memoria è la seguente:

1. **Registri della CPU**
   - Memoria più veloce e più piccola, direttamente accessibile dal processore.
2. **Cache**
   - Memoria veloce e di dimensioni limitate, usata per ridurre i tempi di accesso alla memoria principale.
3. **Memoria principale (RAM)**
   - Memoria volatile con capacità maggiore della cache, usata per caricare i programmi in esecuzione.
4. **Memoria secondaria (dischi rigidi, SSD)**
   - Memoria non volatile, con grande capacità ma tempi di accesso più lunghi.
5. **Memoria di massa esterna (nastri, cloud storage, ecc.)**
   - Utilizzata per archiviazione a lungo termine e backup, con velocità di accesso più lenta.

Questa struttura gerarchica permette di bilanciare velocità, costo e capacità, ottimizzando le prestazioni complessive del sistema.

# 1.4 Cosa caratterizza un sistema multiprocessore?

Un **sistema multiprocessore** è un sistema informatico che dispone di **due o più processori** (CPU) collegati tra loro e che condividono risorse come memoria, bus di sistema e dispositivi di I/O.

## Caratteristiche principali:

- **Parallelismo:** consente l’esecuzione simultanea di più processi o thread, aumentando la potenza di calcolo e l’efficienza.
- **Condivisione delle risorse:** i processori condividono la memoria principale e le periferiche, facilitando la comunicazione e la coordinazione tra processi.
- **Maggiore affidabilità:** in caso di guasto di un processore, gli altri possono continuare a funzionare (in certi sistemi).
- **Complessità di gestione:** richiede un sistema operativo capace di gestire la sincronizzazione, la comunicazione e la concorrenza tra più CPU.

## Tipi di sistemi multiprocessore:

- **Sistemi simmetrici (SMP):** tutti i processori sono equivalenti e gestiti dallo stesso sistema operativo.
- **Sistemi asimmetrici:** un processore principale gestisce il sistema operativo e coordina gli altri processori.

In sintesi, un sistema multiprocessore migliora le prestazioni attraverso l’uso simultaneo di più CPU, ma richiede una gestione sofisticata per coordinare le risorse condivise.

# 1.5 Cos'è la multiprogrammazione?

La **multiprogrammazione** è una tecnica di gestione dei processi che consente di **eseguire più programmi contemporaneamente** su una singola CPU, aumentando l’efficienza dell’utilizzo della macchina.

## Come funziona:

- Il sistema operativo mantiene in memoria più processi pronti all’esecuzione.
- Quando un processo si blocca (ad esempio in attesa di I/O), la CPU viene assegnata a un altro processo pronto.
- In questo modo, la CPU non rimane mai inattiva e si massimizza il suo utilizzo.

## Benefici della multiprogrammazione:

- Riduce i tempi di inattività della CPU.
- Aumenta il throughput del sistema (numero di processi completati in un dato intervallo).
- Migliora la risposta complessiva del sistema agli utenti.

## Differenza con il multitasking:

- La multiprogrammazione si concentra sul tenere più programmi in memoria per utilizzare al meglio la CPU.
- Il multitasking prevede la condivisione del processore in modo più fine (con switch frequenti e percepiti dall’utente come simultaneità).

In sintesi, la multiprogrammazione è una strategia fondamentale per far convivere più processi e sfruttare al massimo le risorse del computer.

# 1.6 A cosa serve il timer in un sistema operativo?

Il **timer** è un componente hardware fondamentale per la gestione del tempo nel sistema operativo.

## Funzioni principali del timer:

- **Prevenire l’esecuzione illimitata di un processo:** Il timer genera un’interruzione periodica (interrupt) che consente al sistema operativo di controllare quanto tempo un processo ha utilizzato la CPU.
- **Abilitare il time sharing e il multitasking:** Grazie al timer, il sistema operativo può **interrompere un processo in esecuzione** e passare la CPU a un altro processo, implementando la pianificazione a intervalli di tempo (time slice o quantum).
- **Gestire le operazioni di timeout:** permette di terminare o gestire operazioni che non rispondono entro un certo limite di tempo (es. attesa di I/O).

## In sintesi:

Il timer serve a **controllare e suddividere il tempo di CPU tra i processi**, garantendo che nessun processo monopolizzi la CPU e permettendo una gestione equa e reattiva delle risorse.

# 1.7 Cosa rappresenta una macchina virtuale?

Una **macchina virtuale (VM)** è un ambiente software che emula un sistema hardware completo, consentendo di eseguire un sistema operativo e applicazioni come se fossero su un computer fisico reale.

## Caratteristiche principali:

- **Isolamento:** ogni macchina virtuale è isolata dalle altre e dall’hardware fisico sottostante.
- **Portabilità:** una VM può essere spostata o copiata facilmente tra diversi host fisici.
- **Multipli sistemi operativi:** consente di far girare più sistemi operativi differenti sulla stessa macchina fisica.
- **Gestione tramite hypervisor:** un software chiamato *hypervisor* gestisce le VM, allocando risorse hardware e isolando i diversi ambienti.

## Tipi di macchine virtuali:

- **Macchine virtuali di sistema:** emulano un’intera macchina fisica, compreso il processore, la memoria, i dispositivi di I/O.
- **Macchine virtuali processore:** eseguono un singolo programma in un ambiente isolato, traducendo le istruzioni del programma.

## Vantaggi:

- Semplificazione della gestione dei sistemi.
- Maggiore sicurezza e isolamento.
- Utilizzo più efficiente delle risorse hardware.

In sintesi, una macchina virtuale è un **computer simulato** che permette di eseguire sistemi e programmi in modo indipendente dall’hardware fisico.

# 2.1 Cos'è un interprete dei comandi (shell)?

Un **interprete dei comandi**, comunemente chiamato **shell**, è un programma che fornisce un'interfaccia tra l'utente e il sistema operativo.

## Funzioni principali della shell:

- **Interpreta i comandi** digitati dall’utente e li traduce in istruzioni eseguibili dal sistema operativo.
- **Gestisce l’avvio di programmi** e script.
- **Consente la gestione di file e processi**, offrendo comandi per navigare nel file system, manipolare file, e controllare i processi.
- **Supporta la programmazione di script**, permettendo di automatizzare operazioni ripetitive.

## Tipi di shell:

- **Shell testuale (CLI - Command Line Interface):** come Bash, sh, zsh su sistemi Unix/Linux, o PowerShell su Windows.
- **Shell grafica:** interfacce grafiche come Windows Explorer o Finder su macOS che offrono comandi tramite interazione visuale.

In sintesi, la shell è il **punto di accesso principale** tramite cui l’utente comunica con il sistema operativo, traducendo comandi testuali in azioni concrete.

# 2.2 A cosa serve una chiamata di sistema?

Una **chiamata di sistema (system call)** è un meccanismo che permette a un programma utente di richiedere servizi e risorse al sistema operativo in modo controllato e sicuro.

## Scopi principali delle chiamate di sistema:

- **Accesso alle risorse hardware:** come file, dispositivi di I/O, memoria, processori.
- **Gestione dei processi:** creazione, terminazione, sospensione e comunicazione tra processi.
- **Gestione del file system:** apertura, lettura, scrittura, chiusura di file e directory.
- **Gestione della memoria:** allocazione e rilascio di memoria.
- **Controllo e comunicazione:** invio di segnali, sincronizzazione, gestione di permessi e sicurezza.

## Perché sono necessarie?

- I programmi utente non possono accedere direttamente all’hardware o ad alcune risorse per motivi di sicurezza e stabilità.
- Le chiamate di sistema forniscono un’interfaccia standard e protetta per accedere ai servizi del sistema operativo.

In sintesi, le chiamate di sistema sono il **ponte tra i programmi applicativi e il sistema operativo**, permettendo l’esecuzione di operazioni privilegiate in modo controllato.

# 2.3 Cosa fa un linker?

Il **linker** è un programma che si occupa di **unire insieme uno o più file oggetto** (compilati da codice sorgente) per creare un file eseguibile o una libreria.

## Funzioni principali del linker:

- **Risoluzione dei simboli:** collega riferimenti a variabili e funzioni presenti in file diversi, trovando gli indirizzi corretti.
- **Assemblaggio del codice:** combina il codice macchina e i dati di più moduli in un unico programma.
- **Allocazione degli indirizzi di memoria:** assegna indirizzi di memoria agli elementi del programma in modo che possano essere correttamente eseguiti.
- **Incorporamento di librerie:** aggiunge codice di librerie esterne richieste dal programma.

## Tipi di linker:

- **Linker statico:** produce un eseguibile completo, incorporando tutte le librerie necessarie direttamente nel file eseguibile.
- **Linker dinamico:** collega librerie al momento dell’esecuzione (dynamic linking), riducendo la dimensione dell’eseguibile e permettendo aggiornamenti più semplici.

In sintesi, il linker è il **collegamento finale** tra il codice compilato e il programma eseguibile pronto per essere lanciato.

# 2.4 Sistema operativo monolitico

Un **sistema operativo monolitico** è un'architettura in cui tutti i servizi del sistema operativo — come la gestione dei processi, della memoria, del file system, e dei dispositivi di I/O — sono integrati in un unico grande blocco di codice che gira in **modalità kernel**.

## Caratteristiche principali:

- Tutti i componenti sono strettamente interconnessi e comunicano direttamente tra loro.
- Elevate prestazioni grazie all’assenza di sovraccarichi di comunicazione tra moduli separati.
- Maggiore difficoltà nella manutenzione e nell’estensione del sistema, perché un errore in una parte del kernel può compromettere l’intero sistema.
- Tipico esempio di sistema operativo monolitico è **Linux**.

In sintesi, il sistema operativo monolitico è una struttura compatta e integrata, in cui il kernel controlla tutte le funzioni principali del sistema in modo centralizzato.

# 2.5 Qual è la caratteristica principale di un microkernel?

La caratteristica principale di un **microkernel** è che implementa **solo le funzionalità di base essenziali** all'interno del kernel, mentre la maggior parte dei servizi del sistema operativo (come gestione dei file, driver, rete, ecc.) vengono eseguiti in **processi separati in modalità utente**.

## Vantaggi principali:

- **Modularità e isolamento:** i servizi sono separati dal kernel, quindi un errore in un servizio non compromette l’intero sistema.
- **Maggiore sicurezza e stabilità:** grazie alla riduzione del codice eseguito in modalità kernel.
- **Facilità di manutenzione e aggiornamento:** è possibile modificare o aggiungere servizi senza toccare il kernel.

## Svantaggi:

- Possibile sovraccarico dovuto alla comunicazione tra kernel e servizi tramite messaggi (IPC - Inter Process Communication).

In sintesi, il microkernel è progettato per essere **piccolo, modulare e più sicuro**, delegando la maggior parte delle funzioni a processi esterni al kernel.

# 2.6 Cosa si intende per 'loader'?

Il **loader** è un componente del sistema operativo responsabile di **caricare un programma eseguibile dalla memoria di massa alla memoria principale (RAM)** per permetterne l’esecuzione.

## Funzioni principali del loader:

- Legge il file eseguibile dal disco.
- Alloca lo spazio di memoria necessario per il programma.
- Trasferisce il codice e i dati del programma in memoria.
- Imposta i registri della CPU e il puntatore di programma (PC) per iniziare l’esecuzione.
- Risolve eventuali indirizzi relativi o simboli, se richiesto.

In sintesi, il loader prepara un programma affinché possa essere eseguito dalla CPU, svolgendo il passaggio essenziale dal file su disco al processo in memoria.

# 3.1 Cos'è un processo in un sistema operativo?

Un **processo** è un'istanza di un programma in esecuzione, ovvero un’entità dinamica che rappresenta l’esecuzione di un codice con le sue risorse associate.

## Componenti principali di un processo:

- **Codice eseguibile:** il programma in esecuzione.
- **Contesto di esecuzione:** include il contenuto dei registri della CPU, il program counter, lo stack e altre informazioni necessarie per riprendere l’esecuzione.
- **Spazio di indirizzamento:** la memoria allocata al processo (codice, dati, stack, heap).
- **Stato:** informazioni sullo stato corrente del processo (pronto, in esecuzione, bloccato, terminato).

## Ruolo nel sistema operativo:

- Il sistema operativo gestisce i processi, pianificandoli e allocando risorse per permettere l’esecuzione concorrente o parallela di più programmi.
- I processi possono comunicare tra loro e sincronizzarsi tramite meccanismi messi a disposizione dal sistema operativo.

In sintesi, un processo è la **unità base di esecuzione** in un sistema operativo, rappresentando un programma in esecuzione con tutte le sue risorse e informazioni di stato.

# 3.2 Quali sono gli stati tipici di un processo?

Un processo, nel ciclo di vita gestito dal sistema operativo, può trovarsi in diversi stati principali:

1. **New (Nuovo)**
   Il processo è in fase di creazione, il sistema sta preparando le risorse necessarie.
2. **Ready (Pronto)**
   Il processo è caricato in memoria, attende di essere assegnato alla CPU per essere eseguito.
3. **Running (In esecuzione)**
   Il processo sta effettivamente utilizzando la CPU per eseguire le istruzioni.
4. **Waiting (Bloccato o in attesa)**
   Il processo è in attesa di un evento esterno, come il completamento di un’operazione di I/O o la disponibilità di una risorsa.
5. **Terminated (Terminato)**
   Il processo ha completato la sua esecuzione o è stato terminato dal sistema operativo.

# 3.3 Cosa contiene il blocco di controllo del processo (PCB)?

Il **Blocco di Controllo del Processo (PCB, Process Control Block)** è una struttura dati che il sistema operativo utilizza per tenere traccia di tutte le informazioni relative a un processo.

## Informazioni contenute nel PCB:

- **Identificatori del processo:** PID (Process ID), informazioni sul proprietario, priorità.
- **Stato del processo:** stato attuale (Ready, Running, Waiting, ecc.).
- **Contesto di esecuzione:** registri della CPU, program counter, stack pointer, ecc.
- **Informazioni sulla gestione della memoria:** indirizzi di base, tabelle delle pagine, limiti di memoria.
- **Informazioni sulle risorse:** file aperti, dispositivi utilizzati, segnali in attesa.
- **Informazioni di scheduling:** priorità, informazioni sulla coda di pianificazione, tempo di CPU utilizzato.
- **Informazioni di comunicazione:** pipe, messaggi, segnali.

In sintesi, il PCB è il **contenitore di tutte le informazioni necessarie per gestire e riprendere un processo** durante il suo ciclo di vita.

# 3.4 Cos'è il cambio di contesto?

Il **cambio di contesto** (context switch) è il processo con cui il sistema operativo **salva lo stato di un processo in esecuzione e carica lo stato di un altro processo**, permettendo la condivisione della CPU tra più processi.

## Come funziona:

- Il sistema operativo salva nel PCB del processo corrente tutti i registri della CPU, il program counter, e altre informazioni di stato.
- Carica dal PCB del processo successivo tutte le informazioni necessarie per riprendere la sua esecuzione.
- Aggiorna lo stato dei processi coinvolti (ad esempio, da Running a Ready, e da Ready a Running).

## Perché è importante:

- Consente il **multitasking** e la gestione concorrente di più processi.
- Permette di eseguire più programmi apparentemente simultaneamente su una singola CPU.
- Garantisce una gestione equa e responsiva della CPU tra i processi.

In sintesi, il cambio di contesto è il meccanismo che consente al sistema operativo di **passare da un processo all’altro** mantenendo il corretto stato di ciascuno.

# 3.5 Quale funzione UNIX viene spesso usata per creare un nuovo processo?

La funzione UNIX più comunemente usata per creare un nuovo processo è la **`fork()`**.

## Caratteristiche di `fork()`:

- Crea un **processo figlio** duplicando il processo chiamante (processo padre).
- Il processo figlio è una copia quasi identica del processo padre, con un proprio spazio di indirizzamento.
- La funzione ritorna due volte:
  - Nel processo padre ritorna il PID del processo figlio.
  - Nel processo figlio ritorna 0.
- Permette al sistema operativo di eseguire più processi contemporaneamente.

Spesso `fork()` è combinata con la funzione **`exec()`** per caricare un nuovo programma nel processo figlio appena creato.

In sintesi, `fork()` è la chiamata di sistema chiave in UNIX per **creare nuovi processi**.

# 3.6 Quale tra queste è una modalità di comunicazione tra processi?

Le modalità comuni di comunicazione tra processi (Inter-Process Communication, IPC) includono:

- **Pipes**
- **Message Passing (scambio di messaggi)**
- **Shared Memory (memoria condivisa)**
- **Semafori (per sincronizzazione)**

Se hai una lista specifica di opzioni, inviamele e ti indicherò qual è la modalità corretta.

---

In generale, tra le modalità tipiche di comunicazione tra processi troviamo:

- **Pipes:** canali di comunicazione unidirezionali o bidirezionali usati per trasferire dati tra processi correlati.
- **Message Passing:** i processi si scambiano messaggi tramite chiamate di sistema, utile per processi non correlati.
- **Shared Memory:** due o più processi accedono a una porzione di memoria comune per scambiare dati in modo rapido.
- **Semafori:** meccanismi per sincronizzare l’accesso a risorse condivise.

Quindi, se la domanda riguarda modalità di comunicazione tra processi, una di queste è la risposta corretta.

# 3.7 Cosa sono le pipe nei sistemi operativi?

Le **pipe** sono un meccanismo di comunicazione tra processi (IPC - Inter-Process Communication) che permette di trasferire dati in modo unidirezionale da un processo a un altro.

## Caratteristiche principali delle pipe:

- **Comunicazione in modalità flusso:** i dati scritti da un processo in una pipe possono essere letti dall’altro processo in ordine sequenziale.
- **Unidirezionalità:** i dati fluiscono in una sola direzione, dal processo scrittore a quello lettore.
- **Utilizzo tipico:** comunicazione tra processi correlati, come padre e figlio.
- **Pipe anonime:** utilizzate tra processi che hanno un legame diretto (es. creati tramite `fork()`).
- **Pipe nominate (FIFO):** possono essere usate anche tra processi non correlati e hanno un nome nel file system.

## Vantaggi:

- Semplicità di implementazione e utilizzo.
- Permettono il passaggio di dati senza la necessità di memorizzazione intermedia complessa.

In sintesi, le pipe sono un metodo semplice e efficiente per la comunicazione e la sincronizzazione tra processi all’interno di un sistema operativo.

# 3.8 A cosa servono i socket nei sistemi client-server?

I **socket** sono un meccanismo di comunicazione che permette a due processi, anche su macchine diverse collegate in rete, di **scambiarsi dati in modo bidirezionale**.

## Funzioni principali dei socket:

- **Creare un canale di comunicazione tra client e server.**
- Supportare la comunicazione tramite protocolli di rete come TCP (affidabile, orientato alla connessione) o UDP (non affidabile, senza connessione).
- Permettere lo scambio di dati a basso livello tra processi su reti locali o internet.

## Utilizzo nei sistemi client-server:

- Il **server** crea un socket in ascolto su una porta specifica.
- Il **client** crea un socket e si connette al socket del server.
- Dopo la connessione, i due processi possono inviare e ricevere dati tramite i socket.

In sintesi, i socket sono fondamentali per la **comunicazione di rete** tra processi in architetture client-server.

# 4.1 Cos'è un thread?

Un **thread** è la più piccola unità di esecuzione all'interno di un processo.

## Caratteristiche principali:

- Un processo può contenere uno o più thread (multithreading).
- I thread di uno stesso processo condividono lo stesso spazio di indirizzamento, cioè memoria, file aperti e altre risorse.
- Ogni thread ha un proprio contesto di esecuzione: program counter, registri CPU, e stack.
- Permettono l’esecuzione concorrente di più flussi di controllo all’interno dello stesso processo.

## Vantaggi dell’uso dei thread:

- Maggiore efficienza e reattività nei programmi.
- Minori costi di creazione e gestione rispetto ai processi.
- Facilitano la programmazione di applicazioni parallele e interattive.

In sintesi, un thread è un **flusso di esecuzione indipendente** che condivide risorse con altri thread dello stesso processo.

# 4.2 Cos'è il parallelismo dei dati?

Il **parallelismo dei dati** è una tecnica di calcolo parallelo che consiste nell'eseguire la stessa operazione contemporaneamente su diversi subset di dati distribuiti tra più processori o nodi. Questo approccio è particolarmente efficace per elaborare grandi volumi di dati in modo rapido ed efficiente.

## Come funziona

1. **Suddivisione dei dati**: un ampio dataset viene diviso in blocchi più piccoli e gestibili.
2. **Elaborazione distribuita**: ciascun blocco di dati viene assegnato a un processore o thread separato.
3. **Elaborazione simultanea**: i processori lavorano sui rispettivi blocchi in parallelo, applicando la stessa operazione su ciascun blocco.
4. **Aggregazione dei risultati**: i risultati ottenuti da ciascun blocco vengono combinati per produrre l'output finale.

## Vantaggi

- **Velocità**: l'elaborazione parallela riduce significativamente il tempo complessivo di calcolo.
- **Scalabilità**: è possibile gestire dataset di dimensioni crescenti aggiungendo più risorse computazionali.
- **Efficienza**: ottimizza l'uso delle risorse hardware disponibili, come CPU e GPU.

## Applicazioni

Il parallelismo dei dati è ampiamente utilizzato in vari ambiti, tra cui:

- **Machine Learning e Deep Learning**: per addestrare modelli su grandi dataset, migliorando la velocità e l'efficienza dell'addestramento.
- **Elaborazione di immagini e video**: per applicare filtri o trasformazioni a grandi volumi di dati visivi.
- **Analisi genomica**: per processare sequenze di DNA o RNA in modo rapido e accurato.
- **Simulazioni scientifiche**: per eseguire calcoli complessi su modelli fisici o chimici.

## Conclusione

Il parallelismo dei dati è una strategia fondamentale per affrontare le sfide poste dall'elaborazione di grandi volumi di dati, permettendo di ottenere risultati in tempi ridotti e con un uso ottimale delle risorse computazionali disponibili.

# 4.3 Nel modello 'molti a uno', cosa accade?

Nel modello **"molti a uno" (many-to-one)** di gestione dei thread:

- **Molti thread utente sono mappati su un solo thread del kernel.**
- La gestione e il scheduling dei thread avviene a livello utente tramite una libreria di thread.
- Il sistema operativo vede solo un singolo thread kernel per tutti i thread utente.

## Conseguenze principali:

- Se un thread utente si blocca (es. per I/O), **tutti gli altri thread dello stesso processo si bloccano** perché il kernel gestisce solo un thread.
- Non è possibile sfruttare il parallelismo su sistemi multi-core, dato che solo un thread kernel può essere in esecuzione alla volta.
- Il cambio di contesto tra thread è veloce perché gestito in user-space, senza passare al kernel.

## Sintesi

Il modello "molti a uno" è semplice e leggero, ma limita le prestazioni in applicazioni multithread su sistemi moderni multi-core a causa della mancanza di parallelismo reale e problemi di blocco.

# 4.4 Cosa permette il modello 'molti a molti'?

Il modello **"molti a molti" (many-to-many)** permette di mappare **molti thread utente su un numero uguale o minore di thread kernel**.

## Caratteristiche principali:

- Il sistema operativo gestisce un pool di thread kernel.
- I thread utente vengono associati dinamicamente ai thread kernel disponibili.
- Consente di eseguire più thread utente contemporaneamente su più processori (vero parallelismo).
- Se un thread si blocca, gli altri thread possono continuare a essere eseguiti senza problemi.
- Offre un buon equilibrio tra efficienza e capacità di parallelismo.

## Vantaggi:

- Supporta il multithreading con parallelismo su sistemi multi-core.
- Riduce il sovraccarico di creare troppi thread kernel rispetto al modello "molti a uno".
- Migliora la reattività e la scalabilità rispetto agli altri modelli.

In sintesi, il modello "molti a molti" combina la flessibilità del multithreading a livello utente con la potenza del parallelismo a livello kernel.

# 4.5 Qual è il ruolo del thread pool?

Un **thread pool** è un insieme di thread pre-creati e mantenuti pronti all’uso dal sistema operativo o da una libreria di runtime per eseguire compiti o richieste multiple.

## Ruolo principale del thread pool:

- **Riutilizzare thread esistenti** invece di crearne e distruggerne di nuovi continuamente, riducendo il costo associato alla creazione e terminazione dei thread.
- **Gestire efficientemente il numero di thread attivi**, evitando di saturare le risorse di sistema con troppi thread contemporanei.
- **Migliorare le prestazioni** delle applicazioni che eseguono molti compiti concorrenti, specialmente in ambienti server o applicazioni I/O-bound.

## Come funziona:

- Il thread pool mantiene un certo numero di thread pronti.
- Quando arriva un nuovo compito, il sistema assegna un thread libero per eseguirlo.
- Al termine del compito, il thread torna al pool in attesa di un nuovo incarico.

In sintesi, il thread pool serve a **ottimizzare la gestione dei thread** migliorando l’efficienza e la scalabilità delle applicazioni concorrenti.

# 4.6 Cosa rappresenta il modello fork-join?

Il modello **fork-join** è un paradigma di programmazione parallela in cui un processo o thread principale **si divide (fork) in più thread o processi concorrenti**, che eseguono in parallelo, e successivamente **si sincronizzano (join)** per unire i risultati prima di continuare l'esecuzione.

## Fasi principali:

1. **Fork:** il thread principale crea (fork) più thread figli per eseguire compiti paralleli.
2. **Esecuzione parallela:** i thread figli lavorano contemporaneamente su parti diverse del problema.
3. **Join:** i thread figli terminano il lavoro e si sincronizzano, permettendo al thread principale di attendere che tutti abbiano completato prima di procedere.

## Utilizzo:

- Ampiamente usato in algoritmi paralleli come divide-and-conquer.
- Presente in framework di parallelismo come Java Fork/Join Framework o OpenMP.

## Vantaggi:

- Facilita la scrittura di codice parallelo strutturato.
- Permette di sfruttare il parallelismo a livello di thread o processi.
- Migliora le prestazioni su sistemi multi-core.

In sintesi, il modello fork-join consente di suddividere un compito in sotto-compiti paralleli e di sincronizzarli in modo efficiente al termine dell’elaborazione.

# 4.7 In che modo i thread Java possono essere gestiti in modo implicito?

In Java, i thread possono essere gestiti **implicitamente** utilizzando framework e librerie che nascondono la complessità della creazione, gestione e sincronizzazione dei thread.

## Modi comuni per la gestione implicita dei thread in Java:

### 1. **Executor Framework**

- Fornisce un'interfaccia di alto livello per gestire pool di thread e l’esecuzione di task asincroni.
- Con l’uso di `ExecutorService`, è possibile sottomettere task (`Runnable` o `Callable`) senza gestire direttamente la creazione o terminazione dei thread.
- Esempio:
  ```java
  ExecutorService executor = Executors.newFixedThreadPool(5);
  executor.submit(() -> {
      // codice eseguito in un thread del pool
  });
  executor.shutdown();
  ```

# 5.1 Cos'è lo scheduling della CPU?

Lo **scheduling della CPU** è il processo mediante il quale il sistema operativo decide **quale processo o thread deve ottenere la CPU** e per quanto tempo, gestendo così l’esecuzione concorrente di più processi.

## Funzioni principali dello scheduling:

- Assegnare la CPU ai processi pronti all’esecuzione.
- Massimizzare l’utilizzo della CPU e migliorare le prestazioni del sistema.
- Garantire equità e rispetto delle priorità tra i processi.
- Gestire la condivisione della CPU tra processi in multitasking o multiprogrammazione.

## Tipi di scheduling:

- **Preemptive:** il sistema può interrompere un processo in esecuzione per assegnare la CPU a un altro processo più urgente.
- **Non-preemptive:** un processo mantiene la CPU fino al completamento o a un'operazione di attesa.

## Algoritmi comuni di scheduling:

- First-Come, First-Served (FCFS)
- Round Robin (RR)
- Shortest Job Next (SJN)
- Priority Scheduling

In sintesi, lo scheduling della CPU è il meccanismo che coordina l’esecuzione dei processi, ottimizzando l’uso della CPU e garantendo la correttezza e l’efficienza del sistema operativo.

# 5.2 Qual è la funzione del dispatcher?

Il **dispatcher** è il componente del sistema operativo che si occupa di:

- **Eseguire il cambio di contesto** tra processi o thread.
- Passare il controllo della CPU al processo o thread selezionato dallo scheduler.
- Riprendere l’esecuzione del processo/thread scelto caricando il suo stato salvato.

## Operazioni principali del dispatcher:

1. Salvataggio del contesto del processo corrente (registri, program counter, ecc.).
2. Caricamento del contesto del nuovo processo/thread da eseguire.
3. Trasferimento del controllo alla CPU per eseguire il nuovo processo.

## Importanza:

- È responsabile della **transizione rapida ed efficiente** tra processi.
- Permette al sistema operativo di gestire il multitasking e il time-sharing.

In sintesi, il dispatcher è il modulo che attua materialmente lo **switch tra processi** sulla CPU, rendendo possibile l’esecuzione concorrente.

# 5.3 Lo scheduling 'first-come, first-served' (FCFS) è basato su:

Lo scheduling **First-Come, First-Served (FCFS)** è basato su un criterio di **ordinamento FIFO (First-In, First-Out)**.

## Caratteristiche principali:

- I processi vengono eseguiti nell'ordine in cui arrivano nella coda dei processi pronti.
- Il primo processo che arriva viene eseguito fino al completamento, senza preemption.
- Non tiene conto della durata o della priorità dei processi.

## Implicazioni:

- È semplice da implementare.
- Può causare il fenomeno di **convoy effect**, dove processi brevi attendono a lungo dietro a processi lunghi.
- Può portare a tempi di attesa elevati per processi successivi.

In sintesi, lo scheduling FCFS assegna la CPU in ordine cronologico di arrivo, eseguendo ogni processo fino alla sua fine.

# 5.4 L'algoritmo 'shortest-job-first' (SJF) seleziona:

L'algoritmo **Shortest-Job-First (SJF)** seleziona il processo con il **tempo di esecuzione più breve** (burst time minimo) tra quelli pronti.

## Caratteristiche principali:

- Minimizza il tempo medio di attesa dei processi.
- Può essere **preemptive** (Shortest Remaining Time First) o **non-preemptive**.
- Richiede la conoscenza preventiva del tempo di esecuzione di ogni processo, che non sempre è disponibile.

## Vantaggi:

- Ottimizza l'efficienza complessiva e riduce la latenza.

## Svantaggi:

- Rischio di **starvation** per processi con burst time lungo, se arrivano continuamente processi con burst più breve.

In sintesi, SJF dà priorità ai processi che richiedono meno tempo di CPU, migliorando la risposta globale del sistema.

# 5.5 Cos'è il 'quantum' nello scheduling circolare (round-robin)?

Il **quantum** (o time slice) nello scheduling **Round-Robin (RR)** è un intervallo di tempo fisso durante il quale un processo può utilizzare la CPU prima di essere sospeso per permettere l'esecuzione di un altro processo.

## Caratteristiche principali:

- Ogni processo riceve la CPU per un massimo di un quantum di tempo.
- Se il processo termina prima della scadenza del quantum, cede volontariamente la CPU.
- Se il quantum scade e il processo non ha terminato, viene preemptato e messo in fondo alla coda dei processi pronti.
- Il scheduler passa quindi al processo successivo, garantendo a tutti i processi un'allocazione equa di CPU.

## Importanza del quantum:

- Un quantum troppo piccolo causa frequenti cambi di contesto, aumentando l'overhead.
- Un quantum troppo grande si avvicina al comportamento di FCFS, riducendo la reattività.

In sintesi, il quantum definisce la **durata massima di esecuzione consecutiva** di un processo nel Round-Robin, bilanciando equità e efficienza.

# 5.6 Cosa distingue lo scheduling con prelazione da quello senza?

## Scheduling con prelazione (Preemptive Scheduling)

- Il sistema operativo può **interrompere un processo in esecuzione** per assegnare la CPU a un altro processo con priorità più alta o che è diventato pronto.
- Permette una maggiore **reattività** e supporta il multitasking vero.
- Esempi: Round Robin, Shortest Remaining Time First, Priority Scheduling preemptive.

## Scheduling senza prelazione (Non-preemptive Scheduling)

- Un processo mantiene il controllo della CPU fino a quando **termina la sua esecuzione o si blocca volontariamente** (es. per I/O).
- Non è possibile interrompere un processo in esecuzione.
- Può portare a tempi di attesa più lunghi e meno reattività.
- Esempi: First-Come, First-Served (FCFS), Shortest Job Next (SJN) non-preemptive.

## Differenza principale

- **Con prelazione:** la CPU può essere tolta a un processo in esecuzione.
- **Senza prelazione:** la CPU è assegnata a un processo fino al completamento o blocco.

In sintesi, la prelazione consente al sistema operativo di gestire meglio la condivisione della CPU e rispondere rapidamente a eventi urgenti.

# 5.7 Qual è lo scopo dello scheduling real-time?

Lo **scheduling real-time** ha lo scopo di garantire che i processi o task vengano eseguiti **entro vincoli temporali rigorosi**, detti **deadline**, necessari per applicazioni dove il tempo di risposta è critico.

## Caratteristiche principali:

- Priorità basate su tempi di scadenza o urgenza.
- Assicura che i task vengano completati entro il limite temporale previsto.
- Minimizza la latenza e le variazioni nei tempi di risposta.
- Utilizzato in sistemi embedded, controllo industriale, robotica, e applicazioni multimediali.

## Tipi di scheduling real-time:

- **Hard real-time:** scadenze obbligatorie, il mancato rispetto può causare guasti.
- **Soft real-time:** scadenze importanti ma non critiche, occasionali ritardi sono tollerabili.

## Obiettivo principale:

Garantire la **deterministicità** nell’esecuzione dei task per rispettare le scadenze temporali.

In sintesi, lo scheduling real-time è progettato per gestire processi che richiedono risposte tempestive e prevedibili in ambienti con vincoli temporali stringenti.

# 6.1 Cos'è il problema della sezione critica?

Il **problema della sezione critica** riguarda la gestione della **concorrenza** tra processi o thread che accedono **contemporaneamente a risorse condivise** (come variabili, strutture dati, dispositivi) in modo da evitare **inconsistenze e condizioni di gara (race conditions)**.

## Definizione

Una **sezione critica** è la porzione di codice in cui un processo accede a risorse condivise che non devono essere usate contemporaneamente da più processi.

## Problema

- Garantire che **solo un processo alla volta** possa eseguire la sezione critica per evitare problemi di integrità dei dati.
- Coordinare i processi affinché si **eviti la sovrapposizione** nell’accesso alle risorse condivise.

## Requisiti per la soluzione:

1. **Mutua esclusione:** solo un processo alla volta può entrare nella sezione critica.
2. **Progressione:** se nessun processo è nella sezione critica, i processi che vogliono entrarci devono poter procedere senza blocchi inutili.
3. **Attesa limitata (bounded waiting):** nessun processo deve attendere indefinitamente per entrare nella sezione critica (nessuno starvation).

In sintesi, il problema della sezione critica è un problema fondamentale nella programmazione concorrente, volto a garantire l’accesso sicuro e coordinato alle risorse condivise.

# 6.2 Quale condizione è fondamentale per evitare problemi di race condition?

La condizione fondamentale per evitare problemi di **race condition** è la **mutua esclusione**.

## Mutua esclusione

- Garantisce che **solo un processo o thread alla volta** possa accedere alla risorsa condivisa o eseguire la sezione critica.
- Previene accessi concorrenti che potrebbero causare inconsistenze o corruzione dei dati.

## Perché è importante

- Senza mutua esclusione, due o più processi potrebbero modificare simultaneamente una risorsa condivisa, portando a risultati imprevedibili o errati.

In sintesi, la mutua esclusione è la condizione chiave per sincronizzare l'accesso alle risorse condivise e prevenire race condition.

# 6.3 Cosa fa l’istruzione atomica test_and_set()?

L’istruzione atomica **`test_and_set()`** è un'operazione hardware che serve a **realizzare la mutua esclusione** nella programmazione concorrente.

## Funzionamento:

- Legge il valore di una variabile (spesso un lock) e lo imposta a `true` in modo **atomico**, cioè indivisibile e non interrompibile.
- Restituisce il valore precedente della variabile.

## Uso tipico:

- Viene utilizzata per implementare **spinlock** e meccanismi di sincronizzazione.
- Un thread tenta di acquisire il lock chiamando `test_and_set()`:
  - Se il valore precedente era `false` (lock libero), il thread ottiene il lock.
  - Se il valore precedente era `true` (lock occupato), il thread continua a riprovare (spin) finché non riesce ad acquisirlo.

## Esempio semplificato:

```c
bool test_and_set(bool *lock) {
    bool old = *lock;
    *lock = true;
    return old;
}
```

# 6.4 Quale struttura è usata per sincronizzazione nei monitor?

Nei **monitor**, la sincronizzazione tra processi o thread avviene tramite **variabili di condizione** (condition variables).

## Dettagli:

- Le variabili di condizione permettono ai processi di **attendere** e **segnalare** eventi specifici durante l’esecuzione nella sezione critica del monitor.
- Offrono le operazioni principali:
  - `wait()`: un processo si sospende finché non viene notificato.
  - `signal()`: risveglia almeno un processo in attesa.
  - `broadcast()`: risveglia tutti i processi in attesa.

## Funzione nel monitor:

- Consentono di sincronizzare l’accesso alle risorse condivise coordinando l’ordine di esecuzione dei processi.
- Permettono di gestire situazioni di attesa condizionale all’interno della sezione critica.

In sintesi, la sincronizzazione nei monitor si basa su **variabili di condizione**, strumenti che permettono ai thread di comunicare e coordinarsi in modo sicuro e controllato.

# 6.5 Cos'è un semaforo?

Un **semaforo** è una primitiva di sincronizzazione usata nei sistemi operativi e nella programmazione concorrente per **gestire l'accesso a risorse condivise** e **coordinare l'esecuzione di processi o thread**.

## Definizione:

- È una variabile intera che può assumere valori non negativi.
- Supporta due operazioni atomiche principali:
  - `wait()` (o `P`): decrementa il valore del semaforo. Se il valore diventa negativo, il processo che ha chiamato `wait` viene bloccato.
  - `signal()` (o `V`): incrementa il valore del semaforo. Se ci sono processi bloccati, ne viene sbloccato almeno uno.

## Tipi di semafori:

- **Semaforo binario:** può assumere solo i valori 0 o 1, funziona come un mutex.
- **Semaforo contatore:** può assumere valori maggiori di 1, utile per gestire più risorse identiche.

## Scopo principale:

- Garantire la **mutua esclusione** e sincronizzare l’accesso alle risorse condivise evitando condizioni di gara.

In sintesi, un semaforo è uno strumento fondamentale per la sincronizzazione e il controllo della concorrenza nei sistemi operativi.

# 6.6 Quale meccanismo assicura la sincronizzazione usando lock espliciti?

La sincronizzazione usando **lock espliciti** è assicurata tramite:

## Meccanismo di mutua esclusione (mutex)

- Un **lock (mutex)** è una primitiva che garantisce che **solo un thread alla volta** possa accedere a una sezione critica o a una risorsa condivisa.
- I thread devono **acquisire (lock)** il mutex prima di entrare nella sezione critica e **rilasciarlo (unlock)** al termine.
- Se un thread tenta di acquisire un lock già posseduto da un altro, viene bloccato fino a quando il lock non viene rilasciato.

## Come funziona:

1. Thread A chiama `lock()` e acquisisce il mutex.
2. Thread A esegue la sezione critica.
3. Thread A chiama `unlock()` e rilascia il mutex.
4. Un altro thread in attesa può ora acquisire il mutex.

## Importanza:

- Previene race condition e accessi concorrenti non controllati.
- Garantisce la mutua esclusione durante l’accesso a risorse condivise.

In sintesi, la sincronizzazione con lock espliciti si basa su **mutex** che assicurano l’accesso esclusivo alle risorse condivise.

# 6.7 Cosa può causare uno stallo (deadlock)?

Uno **stallo (deadlock)** si verifica quando un insieme di processi rimane **bloccato indefinitamente** perché ciascuno attende una risorsa detenuta da un altro processo dello stesso insieme.

## Cause principali dello stallo:

1. **Mutua esclusione:** almeno una risorsa è utilizzata in modalità esclusiva (non condivisibile).
2. **Hold and wait (attesa e mantenimento):** un processo tiene almeno una risorsa e ne richiede altre.
3. **No preemption (assenza di prelievo):** le risorse non possono essere sottratte forzatamente a un processo che le detiene.
4. **Attesa circolare:** esiste un ciclo chiuso di processi, ognuno dei quali attende una risorsa detenuta dal processo successivo nel ciclo.

## In sintesi:

- Lo stallo nasce dall'interazione di queste quattro condizioni simultanee.
- Se una di queste condizioni viene eliminata, lo stallo può essere evitato.
-

# Cos'è l'inversione di priorità?

L'**inversione di priorità** è un problema che si verifica nei sistemi con scheduling a priorità quando:

- Un **processo a bassa priorità** detiene una risorsa (ad esempio un lock) necessaria a un **processo a priorità più alta**.
- Nel frattempo, un **processo a priorità media** (intermedia) può eseguire perché il processo a bassa priorità non riesce a proseguire (perché in attesa che il processo a priorità alta termini).
- Questo causa un'inversione nell'ordine naturale di esecuzione, poiché il processo a priorità alta viene "bloccato" indirettamente da quello a priorità media.

## Effetti:

- Il processo ad alta priorità subisce un ritardo imprevisto.
- Può compromettere la prevedibilità e la correttezza dei sistemi real-time.

## Soluzioni comuni:

- **Priority inheritance:** il processo a bassa priorità "eredita" temporaneamente la priorità più alta per liberare più velocemente la risorsa.
- **Priority ceiling protocol:** assegna una priorità massima alle risorse per prevenire inversioni.

In sintesi, l'inversione di priorità è un fenomeno di blocco anomalo causato dall’interazione tra priorità di processi e gestione delle risorse condivise

# 6.8 Cos'è l'inversione di priorità?

L'**inversione di priorità** è un problema che si verifica nei sistemi con scheduling a priorità quando:

- Un **processo a bassa priorità** detiene una risorsa (ad esempio un lock) necessaria a un **processo a priorità più alta**.
- Nel frattempo, un **processo a priorità media** (intermedia) può eseguire perché il processo a bassa priorità non riesce a proseguire (perché in attesa che il processo a priorità alta termini).
- Questo causa un'inversione nell'ordine naturale di esecuzione, poiché il processo a priorità alta viene "bloccato" indirettamente da quello a priorità media.

## Effetti:

- Il processo ad alta priorità subisce un ritardo imprevisto.
- Può compromettere la prevedibilità e la correttezza dei sistemi real-time.

## Soluzioni comuni:

- **Priority inheritance:** il processo a bassa priorità "eredita" temporaneamente la priorità più alta per liberare più velocemente la risorsa.
- **Priority ceiling protocol:** assegna una priorità massima alle risorse per prevenire inversioni.

In sintesi, l'inversione di priorità è un fenomeno di blocco anomalo causato dall’interazione tra priorità di processi e gestione delle risorse condivise.

# 7.1 Qual è il problema principale nel classico caso produttore/consumatore?

Il problema principale nel classico caso **produttore/consumatore** è la **sincronizzazione** tra i processi produttore e consumatore per:

- **Evitare che il consumatore legga dati inesistenti** (cioè non ancora prodotti).
- **Evitare che il produttore sovrascriva dati non ancora consumati** (cioè il buffer è pieno).

## Dettagli:

- Il produttore produce dati e li inserisce in un buffer condiviso.
- Il consumatore preleva i dati dal buffer per elaborarli.
- Devono essere coordinati per non accedere contemporaneamente allo stesso elemento del buffer (mutua esclusione).
- Devono sincronizzarsi per gestire i casi in cui il buffer è pieno (produttore deve aspettare) o vuoto (consumatore deve aspettare).

In sintesi, il problema riguarda la **corretta gestione della concorrenza e della comunicazione** tra produttore e consumatore per evitare condizioni di gara e sovrascrittura.

# 7.2 Qual è il rischio principale nel problema lettori-scrittori?

Il rischio principale nel **problema lettori-scrittori** è la **starvation**, ovvero la possibilità che uno dei due gruppi di processi (lettori o scrittori) venga bloccato indefinitamente a causa dell'altro gruppo che monopolizza l'accesso alla risorsa condivisa.

## Dettagli:

- **Starvation dei lettori:** Se i lettori hanno priorità (lettori-preference), un flusso continuo di lettori può impedire l'accesso ai processi scrittori, che rimangono in attesa indefinitamente.:contentReference[oaicite:2]{index=2}
- **Starvation degli scrittori:** Se gli scrittori hanno priorità (scrittori-preference), i lettori possono monopolizzare l'accesso alla risorsa, impedendo agli scrittori di procedere.:contentReference[oaicite:5]{index=5}

## Soluzioni:

Per evitare la starvation, è possibile implementare politiche di accesso equo, come l'uso di code FIFO (First-In-First-Out) per gestire le richieste di accesso alla risorsa condivisa.:contentReference[oaicite:8]{index=8}

In sintesi, la **starvation** è il rischio principale nel problema lettori-scrittori, e la sua gestione è fondamentale per garantire l'equità nell'accesso alle risorse condivise.

# 7.3 Nel problema dei cinque filosofi, cosa rappresentano le forchette?

Nel classico problema dei cinque filosofi, le **forchette** rappresentano le **risorse condivise** necessarie affinché i filosofi possano mangiare.

## Dettagli:

- Ogni filosofo ha bisogno di due forchette per mangiare: quella a sinistra e quella a destra.
- Ci sono solo cinque forchette totali, una tra ogni coppia di filosofi.
- Le forchette simboleggiano quindi risorse limitate che devono essere **condivise e sincronizzate** tra più processi (filosofi).

## Problemi evidenziati:

- Se ogni filosofo prende una forchetta e aspetta l’altra, si può verificare un **deadlock** (stallo), dove nessuno riesce a proseguire.
- Il problema illustra le difficoltà nel gestire l’accesso concorrente a risorse condivise e nel prevenire situazioni di blocco o starvation.

In sintesi, le forchette nel problema dei cinque filosofi rappresentano le risorse condivise e limitate che richiedono meccanismi di sincronizzazione per evitare conflitti e garantire il corretto funzionamento del sistema.

# 7.4 Tecnica per risolvere il problema dei cinque filosofi

Una tecnica comune per risolvere il problema dei filosofi è:

- **Prendere le forchette in un ordine prestabilito** (ad esempio sempre prima la forchetta con il numero più basso e poi quella più alta).
  Questo evita la formazione di un ciclo di attesa e quindi il deadlock.

Altre soluzioni includono:

- **Introdurre un arbitro (cameriere)** che controlla l’accesso alle forchette, concedendo il permesso solo se entrambe sono disponibili.
- **Limitare il numero di filosofi che possono mangiare contemporaneamente** (ad esempio massimo 4 filosofi su 5).

Queste tecniche servono a garantire la sincronizzazione e a prevenire deadlock e starvation.

# 7.5 Qual è uno scopo della sincronizzazione all’interno del kernel?

Lo scopo principale della sincronizzazione all’interno del kernel è **gestire l'accesso concorrente alle risorse condivise** per:

- Evitare condizioni di gara (race conditions).
- Garantire la coerenza e l’integrità dei dati.
- Prevenire deadlock e starvation.
- Coordinare correttamente l’esecuzione di più processi o thread che operano simultaneamente.

In sintesi, la sincronizzazione nel kernel assicura che le operazioni critiche vengano eseguite in modo sicuro e ordinato.

# 7.6 Cosa permette il costrutto `synchronized` in Java?

Il costrutto `synchronized` in Java permette di:

- Garantire la **mutua esclusione** nell’accesso a sezioni critiche del codice.
- Evitare che più thread eseguano contemporaneamente codice che accede a risorse condivise, prevenendo race condition.
- Bloccare un oggetto monitor associato per un thread, mentre gli altri thread devono attendere il rilascio del blocco.

In sintesi, `synchronized` serve a sincronizzare i thread per assicurare l’integrità dei dati condivisi.

# 7.7 Obiettivo principale del problema dei lettori-scrittori

Il **problema dei lettori-scrittori** riguarda la gestione dell'accesso concorrente a una risorsa condivisa, come una base di dati, da parte di due tipi di processi:

- **Lettori**: accedono alla risorsa in sola lettura.
- **Scrittori**: possono sia leggere che scrivere nella risorsa.

## Obiettivo

L'obiettivo principale è:

- **Permettere l'accesso simultaneo ai lettori** senza conflitti.
- **Garantire l'accesso esclusivo agli scrittori**, evitando che lettori o altri scrittori interferiscano durante l'operazione di scrittura.

## Sfide

Le sfide principali includono:

- **Starvation**: rischio che lettori o scrittori non ottengano mai accesso alla risorsa.
- **Deadlock**: possibilità di blocchi reciproci tra processi in attesa di risorse.

## Soluzioni

Esistono diverse varianti del problema, spesso basate su politiche di priorità, come:

- **Priorità ai lettori**: i lettori hanno sempre accesso, anche se uno scrittore è in attesa.
- **Priorità agli scrittori**: gli scrittori hanno la precedenza, evitando che i lettori monopolizzino la risorsa.

Queste soluzioni mirano a bilanciare l'efficienza e l'equità nell'accesso alla risorsa condivisa.

# 7.8 Nel problema dei cinque filosofi, cosa può causare uno stallo (deadlock)

Uno stallo (deadlock) si verifica quando **tutti i filosofi prendono contemporaneamente la forchetta a sinistra e aspettano quella a destra**, bloccandosi a vicenda senza mai riuscire a mangiare.

## Le quattro condizioni per il deadlock nel problema sono:

1. **Mutua esclusione**: ogni forchetta può essere utilizzata da un solo filosofo alla volta.
2. **Possesso e attesa**: ogni filosofo possiede una forchetta e attende l’altra.
3. **Non preemption**: una forchetta non può essere tolta a un filosofo finché lui non la rilascia volontariamente.
4. **Attesa circolare**: ogni filosofo attende una forchetta detenuta dal filosofo successivo, formando un ciclo.

## Per evitare il deadlock si possono adottare strategie come:

- Numerare le forchette e acquisirle in ordine.
- Limitare il numero di filosofi che possono mangiare contemporaneamente.

# 8.1 Cosa si intende per stallo (deadlock) nei sistemi operativi?

Uno **stallo** (o **deadlock**) nei sistemi operativi si verifica quando **un insieme di processi resta bloccato in attesa reciproca di risorse**, che non verranno mai rilasciate.

## Condizioni necessarie per un deadlock:

1. **Mutua esclusione**: una risorsa non può essere condivisa; è assegnata a un solo processo alla volta.
2. **Possesso e attesa**: un processo che detiene una risorsa ne richiede un’altra già assegnata.
3. **Non preemption**: una risorsa non può essere forzatamente tolta a un processo; deve essere rilasciata volontariamente.
4. **Attesa circolare**: esiste un ciclo di processi, ciascuno in attesa di una risorsa detenuta dal successivo.

## Esempio:

Un processo A detiene la stampante e vuole accedere allo scanner, mentre il processo B ha lo scanner e aspetta la stampante: nessuno dei due può procedere.

## Conseguenza:

I processi coinvolti restano **permanentemente bloccati**, a meno che non intervenga un meccanismo esterno per rompere lo stallo.

# 8.2 Quale delle seguenti è una condizione necessaria per il verificarsi di uno stallo?

Perché si verifichi uno **stallo (deadlock)**, devono essere vere **contemporaneamente** le seguenti **quattro condizioni necessarie** (secondo Coffman):

1. **Mutua esclusione**
   Almeno una risorsa deve essere non condivisibile, cioè solo un processo alla volta può utilizzarla.
2. **Possesso e attesa (Hold and Wait)**
   Un processo che detiene almeno una risorsa sta aspettando di acquisire risorse aggiuntive già allocate ad altri processi.
3. **Non preemption (assenza di forzatura)**
   Le risorse non possono essere sottratte ai processi che le possiedono; devono essere rilasciate volontariamente.
4. **Attesa circolare (Circular wait)**
   Deve esistere un ciclo chiuso di processi in cui ciascun processo sta aspettando una risorsa detenuta dal processo successivo.

## Conclusione

**Tutte e quattro** le condizioni sopra devono verificarsi affinché si possa avere uno stallo. Se anche **una sola di queste condizioni viene evitata**, il deadlock non può accadere.

# 8.3 Cosa rappresenta un grafo di assegnazione delle risorse?

Un **grafo di assegnazione delle risorse** è una rappresentazione grafica utilizzata per **analizzare e rilevare situazioni di deadlock** in un sistema operativo.

## Componenti principali:

- **Nodi**:
  - **Processi** (rappresentati come cerchi).
  - **Risorse** (rappresentate come quadrati).
- **Archi**:
  - **Da un processo a una risorsa**: indica che il processo **richiede** quella risorsa.
  - **Da una risorsa a un processo**: indica che la risorsa è **assegnata** a quel processo.

## Utilizzo:

- Serve a **verificare se esiste un ciclo** nel grafo:
  - Se c’è un ciclo e **ogni risorsa ha un solo istanza**, allora **esiste un deadlock**.
  - Se le risorse hanno più istanze, un ciclo **può indicare** una situazione di deadlock, ma non è una condizione sufficiente.

# 8.4 Quale strategia può prevenire uno stallo (deadlock)?

Una strategia efficace per prevenire uno stallo è **rompere almeno una delle quattro condizioni necessarie al deadlock**.

## Strategie comuni:

1. **Ordinare l'acquisizione delle risorse**

   - Ogni filosofo deve prendere prima la forchetta con numero più basso, poi quella con numero più alto.
   - Questo elimina l’attesa circolare.
2. **Limitare il numero di filosofi che siedono al tavolo**

   - Permettere solo a **quattro filosofi su cinque** di cercare le forchette contemporaneamente.
   - Garantisce che almeno uno possa mangiare, evitando lo stallo.
3. **Introdurre un arbitro (cameriere)**

   - I filosofi chiedono il permesso al cameriere prima di prendere le forchette.
   - L'arbitro permette l’accesso solo se entrambe le forchette sono disponibili.

## In sintesi:

> La prevenzione del deadlock si basa sul **controllo dell’accesso alle risorse condivise**, evitando le condizioni che lo rendono possibile.

# 8.5 Cos’è lo stato sicuro nell’algoritmo del banchiere?

Nell’**algoritmo del banchiere**, uno **stato sicuro** è una configurazione del sistema in cui esiste almeno una sequenza di esecuzione dei processi tale che:

- Ogni processo può ottenere le risorse di cui ha bisogno,
- E poi può completare ed eventualmente rilasciare le risorse,
- Permettendo così agli altri processi di fare lo stesso.

## Obiettivo

Lo stato sicuro serve a **prevenire il deadlock**: il sistema concede risorse **solo se** dopo la concessione si rimane in uno stato sicuro.

## Esempio

Se un processo richiede risorse, l’algoritmo verifica **in anticipo** se concederle porterà a uno stato sicuro.
Se sì → le risorse vengono assegnate.
Se no → la richiesta viene sospesa.

In sintesi, uno stato sicuro è una garanzia che il sistema potrà sempre completare tutti i processi senza bloccarsi.

# 8.6 Quale dei seguenti è un metodo per rilevare lo stallo (deadlock)?

Un metodo comune per **rilevare lo stallo** nei sistemi operativi è:

- **Il grafo di attesa (wait‑for graph)**
  Si costruisce un grafo in cui ogni nodo rappresenta un processo. Un arco \(P_i \to P_j\) indica che \(P_i\) è in attesa di un processo \(P_j\) che detiene una risorsa. Se nel grafo esiste un **ciclo**, allora si è in presenza di un deadlock. :contentReference[oaicite:0]{index=0}

### Altri metodi noti:

- **Resource Allocation Graph (RAG)**:
  rappresenta risorse e processi con archi di richiesta e assegnazione, e rileva deadlock individuando cicli nel grafo. :contentReference[oaicite:1]{index=1}
- **Algoritmo del banchiere (Banker’s algorithm)**:
  simula l’allocazione delle risorse per verificare se lo stato futuro del sistema è “safe” o rischia il deadlock. :contentReference[oaicite:2]{index=2}
- **Controlli periodici (detection by periodic checking)**:
  il sistema verifica a intervalli prestabiliti lo stato delle risorse e delle richieste, cercando cicli o situazioni irrisolvibili. :contentReference[oaicite:3]{index=3}

---

## ✅ Riepilogo dei metodi principali


| Metodo                        | Descrizione breve                                                                          |
| ----------------------------- | ------------------------------------------------------------------------------------------ |
| **Wait‑for graph**           | Verifica l’esistenza di cicli tra processi in attesa di risorse                           |
| **Resource Allocation Graph** | Controlla cicli tra processi e risorse nei grafi di allocazione                            |
| **Banker’s algorithm**       | Simula allocazioni future per determinare se uno stato è sicuro o potenzialmente deadlock |
| **Controllo periodico**       | Analizza regolarmente la situazione del sistema per rilevare deadlock                      |

Tutti questi metodi servono per **identificare uno stallo** una volta che esso si è verificato o potrebbe verificarsi.

# 8.7 Come si può reagire a una situazione di stallo già avvenuta?

Se uno stallo (**deadlock**) si è già verificato, il sistema può adottare diverse strategie per **rilevarlo e risolverlo**:

## 1. **Rilevamento dello stallo (Deadlock Detection)**

Il sistema analizza periodicamente le risorse e i processi per identificare cicli di attesa.

- Si costruisce un **grafo di attesa** (Wait-For Graph).
- Se esiste un ciclo nel grafo, allora c’è uno stallo.

## 2. **Recupero dallo stallo (Recovery)**

Una volta rilevato lo stallo, si può procedere in vari modi:

- **Terminare uno o più processi coinvolti** nello stallo.
- **Prelevare forzatamente (preempt)** alcune risorse da certi processi.
- **Riavviare** i processi uno alla volta fino alla risoluzione dello stallo.

## 3. **Combinazione di metodi**

Spesso i sistemi combinano rilevamento e recupero per gestire gli stalli in modo controllato e minimizzare l’impatto.

## Nota

Queste tecniche sono usate solo **dopo** che lo stallo si è verificato. Per evitarlo a monte, si usano strategie di **prevenzione o evitamento dello stallo**.

# 8.8 Cos’è uno stallo attivo (livelock)?

Uno **stallo attivo (livelock)** è una situazione in cui **due o più processi continuano a cambiare stato in risposta l’uno all’altro**, ma **nessuno riesce a progredire** con l’esecuzione.

## Caratteristiche:

- Diversamente dal deadlock, i processi **non sono bloccati**: continuano ad eseguire azioni.
- Tuttavia, quelle azioni **non portano mai al completamento del lavoro**, generando un ciclo continuo di tentativi falliti.

## Esempio:

Due processi tentano di accedere a una risorsa condivisa; ogni volta che rilevano un conflitto, cedono il turno all’altro. Se entrambi fanno questo ripetutamente, **nessuno accede mai alla risorsa**.

## Conclusione:

Il livelock è simile al deadlock in quanto impedisce la progressione, ma si differenzia perché i processi **sono attivi ma inutilmente**.

# 9.1 Qual è il ruolo dell'unità di gestione della memoria (MMU)?

La **MMU** (Memory Management Unit) è un componente hardware del sistema che si occupa della **gestione della memoria virtuale**.

## Funzioni principali:

- **Traduzione degli indirizzi logici in indirizzi fisici**: converte gli indirizzi generati dai programmi (logici o virtuali) negli indirizzi reali usati dalla memoria fisica.
- **Protezione della memoria**: impedisce a un processo di accedere alla memoria di un altro processo, garantendo isolamento e sicurezza.
- **Supporto alla paginazione e segmentazione**: gestisce le tecniche di allocazione della memoria come pagine o segmenti.
- **Generazione di eccezioni**: rileva accessi non validi alla memoria (es. violazioni di accesso) e attiva le eccezioni appropriate.

## In sintesi:

La MMU permette di **astrarre la memoria fisica**, offrendo ai processi uno spazio di indirizzamento indipendente, sicuro e gestito in modo efficiente.

# 9.2 Qual è il principale svantaggio dell'allocazione contigua della memoria?

Il principale svantaggio dell'**allocazione contigua** della memoria è la **frammentazione esterna**.

## Dettagli:

- La memoria deve essere assegnata in blocchi contigui (cioè adiacenti).
- Con il tempo, l’allocazione e la deallocazione di processi di dimensioni diverse può lasciare **spazi liberi non utilizzabili** tra blocchi allocati.
- Anche se la memoria totale libera è sufficiente, potrebbe **non esserci un blocco contiguo abbastanza grande** da contenere un nuovo processo.

### Altri svantaggi:

- **Difficoltà nel ridimensionamento** di un processo (espansione o contrazione).
- Richiede **compattazione periodica** per riunire lo spazio libero, che è costosa in termini di tempo.

In sintesi, pur essendo semplice da implementare, l’allocazione contigua è inefficiente nella gestione dinamica della memoria a causa della frammentazione esterna.

# 9.3 Cosa rappresenta un frame nella paginazione?

Un **frame** è una **unità di memoria fisica** di dimensione fissa in cui viene suddivisa la memoria RAM.

## Dettagli:

- La memoria fisica è divisa in tanti frame, ognuno della stessa dimensione (es. 4 KB).
- Il sistema operativo carica le pagine (unità di memoria logica) nei frame disponibili.
- Ogni pagina della memoria virtuale corrisponde a un frame nella memoria fisica.

In sintesi, un frame è un blocco di memoria fisica che contiene una pagina della memoria virtuale durante la paginazione.

# 9.4 Cos'è il TLB (Translation Lookaside Buffer)?

Il **TLB (Translation Lookaside Buffer)** è una **cache hardware** usata nella gestione della memoria virtuale per velocizzare la traduzione degli indirizzi virtuali in indirizzi fisici.

## Funzioni principali:

- Memorizza le ultime traduzioni di pagine virtuali in indirizzi fisici.
- Riduce il tempo di accesso alla tabella delle pagine, evitando ricerche lente in memoria principale.
- Migliora le prestazioni complessive del sistema durante l'accesso alla memoria.

In sintesi, il TLB è una cache speciale che accelera la traduzione degli indirizzi nel processo di gestione della memoria virtuale.

# 9.5 Qual è lo scopo della rilocazione dinamica?

La **rilocazione dinamica** ha lo scopo di:

- Permettere che i programmi vengano caricati in qualsiasi posizione della memoria durante l'esecuzione.
- Consentire al sistema operativo di spostare processi o parti di essi in memoria senza modificare il codice sorgente.
- Facilitare la gestione efficiente della memoria, aumentando la flessibilità e l’utilizzo ottimale dello spazio disponibile.

In sintesi, la rilocazione dinamica supporta l'esecuzione di programmi in ambienti con memoria condivisa e variabile, migliorando la gestione e la protezione della memoria.

# 9.6 Cosa distingue la paginazione gerarchica?

La **paginazione gerarchica** si caratterizza per l'uso di **più livelli di tabelle delle pagine** anziché una singola tabella piatta.

## Caratteristiche principali:

- Divide la tabella delle pagine in più livelli (es. due o tre livelli).
- Ogni livello contiene puntatori a sottotabelle, che a loro volta puntano alle pagine di memoria.
- Riduce la quantità di memoria necessaria per memorizzare le tabelle delle pagine, specialmente per spazi di indirizzi molto grandi.
- Facilita la gestione della memoria virtuale su sistemi con grandi spazi di indirizzi, evitando tabelle troppo grandi e sparse.

In sintesi, la paginazione gerarchica è una struttura a più livelli che migliora l'efficienza e la scalabilità nella traduzione degli indirizzi virtuali.

# 9.7 A cosa serve la tabella delle pagine invertita?

La **tabella delle pagine invertita** (Inverted Page Table) serve a:

- Ridurre lo spazio di memoria richiesto per la gestione della memoria virtuale, soprattutto in sistemi con grandi spazi di indirizzi virtuali.
- Mantenere una mappatura **da frame di memoria fisica a pagine virtuali**, invece che da pagine virtuali a frame (come nella tabella delle pagine tradizionale).
- Facilitare la ricerca veloce dell'indirizzo fisico corrispondente a un indirizzo virtuale tramite una struttura più compatta.

## Caratteristiche principali:

- Ogni voce rappresenta un **frame di memoria fisica** e indica quale pagina virtuale lo sta usando.
- Si evita di dover mantenere una tabella per ogni processo molto grande.
- Richiede strutture di supporto come hash per effettuare la ricerca delle pagine virtuali.

In sintesi, la tabella delle pagine invertita migliora l’efficienza della gestione della memoria virtuale in sistemi con grandi spazi di indirizzi.

# 9.8 Cos'è lo swapping?

Lo **swapping** è una tecnica di gestione della memoria nei sistemi operativi che consiste nel:

- Spostare temporaneamente un processo dalla **memoria principale (RAM)** a un'area di memoria secondaria (tipicamente il disco, chiamata **swap space**).
- Liberare così spazio in RAM per altri processi.
- Successivamente, il processo può essere riportato in memoria principale per continuare l’esecuzione.

## Scopo dello swapping:

- Gestire più processi di quanti ne possa contenere la memoria fisica.
- Migliorare l’utilizzo della memoria e la multiprogrammazione.

Lo swapping permette quindi di aumentare il grado di multiprogrammazione e ottimizzare l’uso delle risorse di memoria.

# 10.1 Cos'è la memoria virtuale?

La **memoria virtuale** è una tecnica di gestione della memoria che:

- Permette a un sistema operativo di utilizzare lo spazio su disco come estensione della memoria RAM.
- Fornisce l'illusione di una memoria principale più grande di quella fisicamente disponibile.
- Consente a ogni processo di avere uno spazio di indirizzamento indipendente e continuo, migliorando sicurezza e isolamento.

## Funzionamento:

- La memoria virtuale divide la memoria in pagine.
- Le pagine non presenti in RAM vengono memorizzate su disco (area di swap o file di paging).
- Quando un processo accede a una pagina non in RAM, si verifica un "page fault" e la pagina viene caricata da disco.

## Vantaggi:

- Gestione efficiente della memoria.
- Possibilità di eseguire programmi più grandi della memoria fisica.
- Isolamento tra processi.

# 10.2 Cosa succede in caso di 'page fault'?

Quando si verifica un **page fault**, il processore tenta di accedere a una pagina di memoria virtuale che non è attualmente presente nella memoria fisica (RAM).Il sistema operativo allora:

- Interviene tramite l'handler di page fault.
- Cerca la pagina mancante sul disco (ad esempio nel file di swap o nel file system).
- Carica la pagina in memoria fisica.
- Aggiorna le tabelle delle pagine per riflettere la nuova mappatura.
- Riprende l'esecuzione del processo interrotto.

---

# 10.3 Cos'è la tecnica 'copy-on-write'?

La **copy-on-write (COW)** è una tecnica di ottimizzazione della gestione della memoria che consente a più processi di condividere la stessa copia di una pagina finché non è necessario modificarla.

- Le pagine sono inizialmente condivise in sola lettura.
- Quando un processo tenta di scrivere sulla pagina condivisa, viene creata una copia privata (scrittura su copia).
- Questo evita copie inutili e migliora l'efficienza nella gestione della memoria.

---

# 10.4 Quale tra questi algoritmi di sostituzione delle pagine è ottimale (teorico)?

L'algoritmo di sostituzione delle pagine **ottimale** (teorico) è quello che **sostituisce la pagina che non sarà più usata per il tempo più lungo nel futuro**.

- È detto anche algoritmo di **Belady**.
- Non può essere implementato praticamente perché richiede la conoscenza futura dei riferimenti di memoria.

---

# 10.5 Cosa si intende per thrashing?

Il **thrashing** è una condizione in cui il sistema operativo passa la maggior parte del tempo a gestire page fault e a spostare pagine tra memoria e disco, anziché eseguire effettivamente i processi.

- Succede quando la memoria fisica è insufficiente per mantenere le pagine necessarie ai processi.
- Porta a un drastico calo delle prestazioni del sistema.

---

# 10.6 Quale meccanismo aiuta a prevenire il thrashing?

Il meccanismo principale per prevenire il thrashing è il **working set model**:

- Tiene traccia del set di pagine attivamente usate da un processo in un intervallo di tempo recente.
- Garantisce che ogni processo abbia in memoria almeno le pagine del suo working set.
- Se la memoria è insufficiente, limita il numero di processi in esecuzione per evitare il sovraccarico.

---

# 10.7 Come funziona l’algoritmo della 'seconda chance'?

L'algoritmo della **seconda chance** è una variante dell'algoritmo FIFO per la sostituzione delle pagine:

- Ogni pagina ha un bit di riferimento (reference bit).
- Quando una pagina arriva in cima alla coda per essere sostituita:
  - Se il bit di riferimento è 0, la pagina viene sostituita.
  - Se il bit è 1, il bit viene resettato a 0, e la pagina viene spostata alla fine della coda (le viene data una "seconda chance").
- Questo permette di evitare di sostituire pagine usate di recente.

---

# 10.8 Cosa fa il sistema di allocazione 'buddy' nel kernel?

Il sistema di allocazione **buddy** è un algoritmo per la gestione della memoria fisica nel kernel:

- Divide la memoria in blocchi di dimensioni potenze di due.
- Quando un processo richiede memoria, il sistema trova il blocco più piccolo adeguato.
- Se il blocco è troppo grande, viene diviso in due "buddy" di dimensione minore.
- Quando i buddy liberi sono adiacenti, vengono uniti per formare blocchi più grandi, riducendo la frammentazione.

Questo sistema permette un'allocazione efficiente e la fusione rapida di blocchi contigui.

# 11.1 Qual è la funzione principale della memoria di massa?

La memoria di massa ha la funzione principale di **conservare i dati e i programmi in modo permanente** o a lungo termine, anche quando il computer è spento.
A differenza della memoria volatile (come la RAM), la memoria di massa mantiene le informazioni memorizzate indipendentemente dall'alimentazione elettrica.
Essa serve per immagazzinare sistemi operativi, applicazioni, file personali, database, e ogni altro tipo di dato digitale che deve essere preservato oltre la sessione di lavoro corrente.

---

# 11.2 Quale tra questi è un tipico dispositivo di memoria secondaria?

Un tipico dispositivo di memoria secondaria è il **disco rigido (Hard Disk Drive, HDD)**.Altri esempi comuni includono:

- SSD (Solid State Drive)
- CD/DVD
- Chiavette USB
- Dischi ottici o nastri magnetici

Questi dispositivi sono caratterizzati da una capacità elevata di memorizzazione e costi inferiori rispetto alla memoria principale (RAM), ma con tempi di accesso più lunghi.

---

# 11.3 Cos'è il 'seek time' in un disco rigido?

Il **seek time** è il tempo necessario affinché la testina di lettura/scrittura del disco rigido si sposti fisicamente dalla posizione corrente a quella della traccia su cui si trova il dato da leggere o scrivere.
È uno dei fattori principali che influiscono sulla velocità di accesso ai dati in un disco magnetico, insieme al tempo di latenza (rotazionale).
Minimizzare il seek time è cruciale per migliorare le prestazioni complessive del sistema di memorizzazione.

---

# 11.4 Qual è lo scopo degli algoritmi di scheduling dei dischi come SCAN o C-SCAN?

Gli algoritmi di scheduling come **SCAN** e **C-SCAN** hanno lo scopo di **ottimizzare l’ordine con cui le richieste di accesso al disco vengono servite**, riducendo il tempo totale di movimentazione della testina (seek time) e migliorando la produttività complessiva.

- **SCAN** fa muovere la testina avanti e indietro lungo il disco, servendo tutte le richieste in una direzione prima di invertire il movimento.
- **C-SCAN** (Circular SCAN) serve le richieste in una direzione e, arrivata all’ultima traccia, torna rapidamente all’inizio senza servire richieste nel percorso di ritorno, garantendo un trattamento più uniforme delle richieste.

Entrambi gli algoritmi evitano il problema di starvation che può verificarsi con lo scheduling FCFS e cercano di mantenere bassi i tempi medi di attesa.

---

# 11.5 Cosa distingue il RAID 1?

Il **RAID 1** è una configurazione di archiviazione che implementa il **mirroring** dei dati, cioè copia esatta dei dati su due o più dischi.Le caratteristiche principali sono:

- Alta affidabilità e tolleranza ai guasti, poiché se un disco si guasta, i dati sono ancora disponibili sull’altro disco.
- Prestazioni di lettura potenzialmente migliorate, poiché la lettura può avvenire da entrambi i dischi.
- Nessun miglioramento in termini di capacità o velocità di scrittura, in quanto ogni dato è duplicato integralmente.

RAID 1 è usato quando la sicurezza dei dati è prioritaria rispetto al costo dello spazio di memorizzazione.

---

# 11.6 A cosa serve l'area di swap?

L’**area di swap** è una porzione di memoria di massa (generalmente un file o una partizione su disco) utilizzata dal sistema operativo per estendere virtualmente la memoria principale (RAM).
Quando la RAM è insufficiente, alcune pagine di memoria vengono temporaneamente spostate nell’area di swap per liberare spazio e permettere l’esecuzione di altri processi.
Questo meccanismo consente di eseguire programmi più grandi della memoria fisica disponibile, anche se l’accesso allo swap è molto più lento rispetto alla RAM, quindi l’eccessivo uso può degradare le prestazioni.

---

# 11.7 Cos'è un blocco difettoso (bad block)?

Un **blocco difettoso** o **bad block** è un settore di un dispositivo di memoria di massa (come un disco rigido o una memoria flash) che non può più essere usato per memorizzare dati in modo affidabile.
Le cause possono essere danni fisici, usura o errori di fabbricazione.
Il sistema operativo o il firmware del dispositivo spesso marcano questi blocchi come non utilizzabili per evitare la perdita di dati e possono tentare di riparare o spostare i dati su blocchi funzionanti.

---

# 11.8 Cos'è una SAN (Storage Area Network)?

Una **SAN (Storage Area Network)** è una rete specializzata ad alta velocità che collega dispositivi di memorizzazione (come array di dischi) a server in modo che le risorse di storage possano essere condivise e gestite centralmente.

Caratteristiche principali:

- Fornisce accesso block-level (livello di blocco) alle risorse di storage, come se fossero dischi locali.
- Migliora la scalabilità, la disponibilità e la gestione dello storage rispetto alle soluzioni locali o tradizionali.
- Utilizza tecnologie di rete ad alte prestazioni come Fibre Channel o iSCSI.

La SAN è molto usata in ambienti aziendali e data center per supportare grandi carichi di lavoro e garantire alta affidabilità dei dati.

# 12.1 Qual è uno dei due compiti principali di un calcolatore secondo il Capitolo 12?

Uno dei due compiti principali di un calcolatore, come descritto nel Capitolo 12, è **gestire l’input/output (I/O)**, ovvero la comunicazione e il trasferimento di dati tra il sistema centrale (CPU e memoria) e i dispositivi periferici come tastiere, dischi, stampanti, e schermi. Questo compito è cruciale perché consente al sistema di interagire con il mondo esterno e gestire operazioni di lettura e scrittura su dispositivi di vario tipo. Il secondo compito fondamentale, anche se non richiesto dalla domanda, riguarda l’elaborazione dei dati, ma il focus qui è proprio sull’efficace gestione dell’I/O.

---

# 12.2 Cos'è il 'polling' nel contesto dell'I/O?

Il **polling** è una tecnica di controllo usata nel contesto dell’I/O in cui la CPU verifica continuamente lo stato di un dispositivo periferico per sapere se è pronto per un’operazione di input o output. In pratica, la CPU esegue ciclicamente una serie di istruzioni per controllare se il dispositivo ha completato un’operazione o necessita attenzione. Questo metodo è semplice ma inefficiente, perché la CPU spreca tempo prezioso in controlli ripetitivi invece di svolgere altre attività utili.

---

# 12.3 Cosa consente l'uso delle interruzioni nei sistemi di I/O?

L’uso delle **interruzioni** nei sistemi di I/O consente alla CPU di essere avvisata immediatamente da un dispositivo quando è pronto per trasferire dati o ha completato un’operazione, evitando così il continuo controllo tramite polling. Questo permette alla CPU di dedicarsi ad altre attività fino a quando non riceve il segnale di interruzione, migliorando l’efficienza complessiva del sistema e permettendo una gestione più reattiva e parallela delle operazioni di I/O.

---

# 12.4 Qual è la funzione principale del DMA (accesso diretto alla memoria)?

La funzione principale del **DMA (Direct Memory Access)** è consentire il trasferimento diretto dei dati tra la memoria centrale e i dispositivi di I/O senza coinvolgere continuamente la CPU. In questo modo, il DMA allevia il carico della CPU, che può continuare ad eseguire altre istruzioni mentre il trasferimento avviene autonomamente, migliorando l’efficienza e la velocità delle operazioni di I/O, specialmente per grandi blocchi di dati.

---

# 12.5 Cosa distingue i dispositivi con trasferimento a blocchi da quelli a caratteri?

I dispositivi con **trasferimento a blocchi** trasferiscono dati in blocchi di dimensioni fisse o variabili, generalmente grandi quantità di dati, come nel caso dei dischi rigidi o nastri. Questi dispositivi sono ottimizzati per spostare grandi quantità di dati in modo efficiente.

Al contrario, i dispositivi con **trasferimento a caratteri** trasferiscono i dati uno alla volta, carattere per carattere, come nel caso delle tastiere o delle stampanti. Questi dispositivi sono tipicamente più lenti e richiedono una gestione più frequente da parte del sistema operativo per ogni unità di dato trasferita.

---

# 12.6 Cos'è lo spooling?

Lo **spooling** (Simultaneous Peripheral Operations On-Line) è una tecnica utilizzata per gestire le operazioni di I/O che coinvolgono dispositivi lenti come le stampanti. Consiste nel memorizzare temporaneamente i dati in una coda o buffer (generalmente su disco) prima di inviarli al dispositivo, permettendo così al sistema di continuare a elaborare altri compiti senza attendere il completamento dell’operazione di I/O. Lo spooling migliora l’efficienza e la gestione delle risorse, soprattutto in ambienti multiutente.

---

# 12.7 A cosa serve la gestione dei buffer nel sottosistema I/O del kernel?

La gestione dei **buffer** nel sottosistema I/O del kernel serve a mediare tra la velocità differente di dispositivi hardware e CPU, immagazzinando temporaneamente i dati in memoria durante i trasferimenti. I buffer permettono di accumulare dati in entrata o in uscita, riducendo la frequenza degli accessi diretti ai dispositivi più lenti e migliorando così le prestazioni complessive del sistema. Inoltre, facilitano la sincronizzazione tra operazioni asincrone e aiutano a gestire dati in modo efficiente e ordinato.

---

# 12.8 Cosa permette l’I/O asincrono?

L’**I/O asincrono** permette a un processo di iniziare un’operazione di input/output e proseguire con altre attività senza dover attendere il completamento dell’I/O stesso. Quando l’operazione termina, il sistema notifica il processo tramite una interruzione o un segnale. Questo modello migliora la reattività e l’efficienza del sistema, permettendo di sovrapporre l’elaborazione con le operazioni di I/O e sfruttare meglio le risorse hardware.

# 13.1 Qual è la funzione principale del file system?

La funzione principale del file system è **organizzare, memorizzare e gestire i dati su dispositivi di memorizzazione** come dischi rigidi, SSD o dispositivi esterni. Il file system:

- Fornisce un’interfaccia logica per creare, leggere, scrivere, modificare e cancellare file.
- Gestisce lo spazio libero e allocato sul dispositivo.
- Tiene traccia delle informazioni sui file tramite strutture dati come inode o directory.
- Permette l’organizzazione gerarchica dei file tramite directory e sottodirectory.
- Garantisce la sicurezza e l’integrità dei dati, tramite controlli di accesso e gestione degli errori.

In sostanza, il file system traduce le richieste di alto livello dell’utente in operazioni hardware di basso livello sulla memoria di massa.

---

# 13.2 Cosa rappresenta un attributo di file?

Un attributo di file è una **informazione associata a un file** che ne descrive le proprietà o lo stato. Gli attributi tipici includono:

- **Nome del file**: identificatore univoco nella directory.
- **Dimensione**: quantità di dati memorizzati nel file.
- **Data e ora di creazione, modifica e ultimo accesso**.
- **Permessi di accesso**: chi può leggere, scrivere o eseguire il file.
- **Tipo di file**: ad esempio file normale, directory, link simbolico.
- **Proprietario e gruppo**: per controlli di sicurezza.
- **Indicazioni sullo stato**: come attributi di sola lettura o nascosto.

Gli attributi sono fondamentali per la gestione, il controllo degli accessi e la corretta interpretazione del file da parte del sistema operativo.

---

# 13.3 Qual è un'operazione tipica sui file?

Un’operazione tipica sui file è la **lettura** e la **scrittura** dei dati. Queste operazioni consentono rispettivamente di:

- **Leggere**: estrarre dati dal file, per esempio visualizzare il contenuto o caricarlo in memoria.
- **Scrivere**: modificare o aggiungere dati nel file, aggiornandone il contenuto.

Altre operazioni comuni includono:

- **Apertura** e **chiusura** di file per iniziare o terminare l’accesso.
- **Rinominare** o **cancellare** file.
- **Spostare** file tra directory o dispositivi.
- **Truncare** file per ridurne la dimensione.

Tutte queste operazioni sono orchestrate dal file system per garantire coerenza e sicurezza.

---

# 13.4 Cosa distingue un file ad accesso sequenziale da uno ad accesso diretto?

La differenza principale riguarda il modo in cui i dati vengono letti o scritti:

- **File ad accesso sequenziale**: i dati devono essere letti o scritti in ordine, dall’inizio alla fine. Per raggiungere una certa posizione si devono attraversare tutti i dati precedenti. È simile alla lettura di una cassetta audio.
- **File ad accesso diretto (o casuale)**: è possibile accedere direttamente a qualsiasi posizione del file senza dover leggere i dati precedenti. Questo è simile a un CD o un disco rigido, dove si può saltare a una traccia specifica.

L’accesso diretto è più efficiente per applicazioni che necessitano di frequenti letture/scritture in punti arbitrari del file, mentre l’accesso sequenziale è più semplice e adatto a flussi dati continui.

---

# 13.5 Quale tipo di struttura delle directory consente nomi duplicati in contesti diversi?

La struttura delle directory **gerarchica** (ad albero) consente nomi duplicati in contesti diversi, perché:

- Ogni file o directory è identificato univocamente dal **percorso completo**, che include la sequenza di directory padre.
- È possibile avere file con lo stesso nome in directory diverse senza conflitti.

Ad esempio, due file chiamati `documento.txt` possono esistere in due directory differenti: `/home/utente1/documento.txt` e `/home/utente2/documento.txt`.

Questo approccio facilita l’organizzazione e la gestione dei file in modo flessibile e scalabile.

---

# 13.6 Cosa rappresenta un file mappato in memoria?

Un file mappato in memoria è una tecnica che consente di **associare direttamente il contenuto di un file al processo di memoria virtuale**. In pratica:

- Il file viene "mappato" in uno spazio di indirizzi del processo, permettendo di leggere o scrivere sul file tramite normali operazioni di accesso alla memoria.
- Questa tecnica ottimizza le operazioni di I/O, eliminando la necessità di chiamate esplicite di lettura o scrittura.
- Facilita la condivisione del file tra più processi e la gestione efficiente di grandi file.

È spesso utilizzata in database, editor di testo e sistemi che richiedono accesso rapido ai dati su disco.

---

# 13.7 A cosa serve il controllo degli accessi nei file system?

Il controllo degli accessi serve a **limitare e gestire chi può effettuare determinate operazioni su file e directory**, proteggendo i dati da accessi non autorizzati. Esso:

- Definisce permessi come lettura, scrittura ed esecuzione per utenti o gruppi.
- Garantisce la sicurezza dei dati, impedendo modifiche o letture indebite.
- Supporta la separazione dei privilegi tra utenti, aumentandone la privacy.
- Può essere implementato tramite meccanismi come liste di controllo (ACL), bit di permessi o sistemi più complessi come SELinux.

In sostanza, il controllo degli accessi è essenziale per mantenere integrità, riservatezza e sicurezza nel sistema.

---

# 13.8 Quale tra i seguenti è un tipo di accesso ai file nei sistemi UNIX?

Nei sistemi UNIX, uno dei tipi principali di accesso ai file è:

- **Accesso sequenziale**: i dati vengono letti o scritti in ordine, dalla posizione corrente in avanti.
- **Accesso diretto (random access)**: tramite la system call `lseek()` si può spostare il puntatore di lettura/scrittura in una posizione arbitraria all’interno del file.

UNIX supporta entrambi i tipi, permettendo flessibilità nelle operazioni di I/O sui file. Inoltre, UNIX gestisce anche l’accesso tramite file descriptor e può utilizzare meccanismi come pipe e socket per la comunicazione interprocesso.

# 14.1 Cos'è una FCB (File Control Block)?

La **FCB (File Control Block)** è una struttura dati usata dal sistema operativo per gestire e tenere traccia delle informazioni relative a un file aperto. Contiene dettagli essenziali come:

- Nome del file
- Posizione corrente del puntatore nel file
- Permessi di accesso
- Dimensione del file
- Informazioni sui blocchi disco allocati al file
- Data e ora di creazione, modifica e accesso

La FCB viene mantenuta in memoria durante la vita del file aperto e permette al sistema operativo di controllare e accedere efficientemente ai dati del file.

---

# 14.2 Qual è lo scopo della struttura stratificata del file system?

La struttura stratificata del file system ha lo scopo di **modulare e semplificare la gestione dei file** suddividendo le funzioni in livelli distinti. Questi livelli includono, ad esempio:

- Gestione fisica del disco (livello più basso)
- Gestione dello spazio libero
- Organizzazione dei file (directory, inode, etc.)
- Interfaccia utente e API per l’accesso ai file

Questa stratificazione permette di isolare le responsabilità, facilitare la manutenzione, e permettere aggiornamenti o sostituzioni di singoli livelli senza impattare l’intero sistema.

---

# 14.3 Quale tecnica di allocazione consente l'accesso diretto ma può soffrire di frammentazione esterna?

La tecnica è **l'allocazione a blocchi contigui**.
In questo metodo, un file è allocato come una sequenza continua di blocchi su disco, permettendo un accesso diretto efficiente ai dati. Tuttavia, con il tempo, la continua creazione e cancellazione di file porta a spazi liberi non contigui, causando **frammentazione esterna**. Questo può rallentare le operazioni di allocazione e accesso.

---

# 14.4 Cosa rappresenta un inode nel file system UNIX?

Un **inode** è una struttura dati fondamentale nel file system UNIX che memorizza tutte le informazioni di un file, ad eccezione del nome. Contiene:

- Permessi di accesso
- Proprietario e gruppo
- Dimensione del file
- Timestamp (creazione, modifica, accesso)
- Puntatori ai blocchi fisici su disco dove sono memorizzati i dati del file

L’inode è identificato da un numero univoco e permette di separare i metadati dal nome del file, che è invece gestito dalla directory.

---

# 14.5 Quale tra i seguenti metodi di gestione dello spazio libero usa una sequenza di bit?

Il metodo che utilizza una **bitmap** (sequenza di bit) per la gestione dello spazio libero.
In questa tecnica, ogni bit rappresenta un blocco sul disco: un bit a 0 indica blocco libero, un bit a 1 indica blocco occupato. È una soluzione efficiente in termini di spazio e permette rapide verifiche e allocazioni.

---

# 14.6 Quale metodo di allocazione utilizza una lista di blocchi con puntatori nel contenuto?

Questo metodo è l’**allocazione concatenata** (o a liste concatenate).
Ogni blocco del file contiene un puntatore al blocco successivo, formando una lista collegata. Ciò consente di gestire file di dimensione variabile senza frammentazione esterna, ma l’accesso diretto è inefficiente perché bisogna scorrere la lista per raggiungere un dato blocco.

---

# 14.7 A cosa serve il journaling in un file system?

Il **journaling** è una tecnica usata nei file system moderni per aumentare l’affidabilità e la consistenza dei dati. Consiste nel mantenere un **registro (journal)** delle operazioni da eseguire prima che vengano applicate definitivamente ai dati e alle strutture del file system.

In caso di crash o spegnimento improvviso, il sistema può recuperare lo stato consistente riprendendo o annullando le operazioni incomplete registrate nel journal, evitando così corruzioni e perdite di dati.

---

# 14.8 Cos’è il TRIM in un file system?

Il **TRIM** è un comando usato nei sistemi con unità a stato solido (SSD) che permette al sistema operativo di comunicare al dispositivo quali blocchi di dati non sono più in uso e possono essere cancellati internamente.

Questo aiuta l’SSD a gestire meglio lo spazio libero, migliorare le prestazioni di scrittura e prolungare la durata dell’unità, riducendo l’usura delle celle di memoria.
