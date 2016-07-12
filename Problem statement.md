# Autori Progetto "Smart Green House"

- Pasquale Oppido
- Angelo Marzucco
- Andrea Russo

# Introduzione

Le colture in serra rappresentano un importante comparto produttivo all�interno del settore orticolo-floricolo, con una forte rilevanza economica. L'idea � quella di implementare le tecniche usate nelle serre per produzione agricola industriale in una serra completamente automatizzata di uso domestico, da utilizzare, ad esempio su un balcone o una terrazza.

# Scopo

Il sistema ha il compito di controllare il processo di irrigazione in una serra a partire dalla misura dell'umidit� del terreno, al fine di mantenerla costante alla soglia necessaria per il tipo di piantagione prescelto.
Il sistema, inoltre controlla la luce all'interno della serra, con l'ausilio di un sensore crepuscolare, al fine di attuare una coltivazione intensiva. Attraverso la misura dell'altezza delle piante viene abilitato un segnle di pronta raccolta . Inoltre vengono monitorati parametri ambientali come temperatura ed umidit� dell'aria al fine di controllare l'eventuale attivazione dei sistemi di riscaldamento e/o di umidificazione all'interno della serricoltura.

# Stato dell'arte nella serricoltura

Nella breve discussione sottostante vengono riportati tre importanti aspetti riguardanti le situazioni correnti nelle colture in serra, ovvero la climatizzazione, l'accumulo termico e l'illuminazione.

1. Climatizzazione

Climatizzare una serra significa effettuare il controllo non solo della temperatura ma anche dell�umidit� relativa, della luminosit� ambientale e del ricambio dell�aria.  La dotazione di un impianto di condizionamento in una serra � fondamentale per garantire il mantenimento della temperatura e umidit� ideale alla crescita delle piante. Nelle serre temperate e calde il riscaldamento � la componente pi� importante. Non essendo sufficiente l��effetto serra� per garantire la temperatura, il riscaldamento artificiale � quasi sempre indispensabile. Esso si ottiene generalmente con generatori d�aria calda dotati di ventilatori.  La tipologia pi� diffusa per il riscaldamento dell�aria � quella sospesa che insuffla aria calda in una tubazione in film plastico forato, anch�essa sospesa.  Per il riscaldamento del substrato di coltivazione si impiegano invece tubazioni in pvc posizionate all�interno dello stesso o sul fondo del bancale. Nella coltivazione a terra le tubazioni vanno interrate ad una profondit� di 20-30 cm.  Nel periodo estivo l��effetto serra� crea problemi di surriscaldamento per cui occorre raffrescare la serra ricorrendo all�effetto combinato di ombreggiamento e ventilazione naturale o forzata. Vi sono poi sistemi che sfruttano l�evaporazione dell�acqua per produrre il raffrescamento e che non richiedono l�ombreggiamento. 
Si tratta dei cosiddetti �cooling system�e �fog system�:

-Il �cooling system� � costituito da ventilatori sistemati su una parete e da una batteria di pannelli alveolati umidificatori collocati nella parete opposta. I ventilatori, dovendo garantire un frequente ricambio dell�aria, hanno elevate portate e sono scelti e posizionati in modo da aspirare dai pannelli umidificatori aria a bassa velocit�. La quantit� d�acqua da dosare sui panelli � intorno a 2 litri per metro quadro di pannello.  

-Il �fog system� consiste nella diffusione in serra di acqua nebulizzata ad alta pressione (35-40 bar) ad opera di ugelli montati su tubazioni poste sopra la coltura. L�intero sistema operativo delle serre moderne (teli-ombreggianti, aperture e chiusure meccanizzate, regolazione termica, ecc.) pu� essere gestito interamente da computer sulla base degli input trasmessi da sensori e da microprocessori periferici. 

2. Accumulo termico nel terreno

Com�� noto, le temperature nel suolo sono pi� costanti rispetto a quelle dell�aria e meno influenzabili dalle variazioni climatiche esterne a mano a mano che la profondit� aumenta.  Queste considerazioni hanno suggerito la messa a punto di sistemi adatti alla stabilizzazione della temperatura nelle serre che si basano sulla circolazione forzata dell�aria all�interno di tubi corrugati sistemati nel terreno.  Nel periodo estivo l�aria esterna che entra nei tubi in corrispondenza del ventilatore � pi� calda del terreno. Nel passaggio all�interno dei tubi sotterranei essa cede il proprio calore al terreno ed esce pi� fresca e pu� raffreddare la serra. Nello stesso tempo il terreno si scalda. Questa tecnica ha un�interessante possibilit� di applicazione nelle serre in stagione fredda.  Il sistema prevede di far ricircolare l�aria della serra, con l�accumulo del calore nel terreno durante il giorno e la restituzione del calore durante la notte, con il risultato di mantenere pi� alta la temperatura della serra durante le ore notturne. Il sistema pu� essere migliorato prevedendo sistemi di accumulo costituiti, ad esempio, da serbatoi con un certo volume d�acqua posti nel suolo e attraversati dalle tubazioni dell�aria.   

3. Illuminazione

Nel Nord Europa nel periodo invernale il ridotto numero di ore giornaliere di illuminazione limita fortemente le possibilit� di crescita delle piante. Si ricorre cos� all�illuminazione artificiale. La potenza elettrica normalmente installata � dell�ordine di 50 W/m2 . Poich� buona parte dell�energia elettrica viene convertita in calore l�illuminazione artificiale contribuisce anche al riscaldamento.  Vengono usate per lo pi� lampade fluorescenti mentre sono sconsigliate le lampade ad incandescenza sia per i consumi elevati sia per la fascia di luce rossa emessa inadatta alla crescita delle piante.  In Italia il problema � meno sentito e il ricorso all�illuminazione artificiale viene fatto per scopi particolari. Ad esempio per la forzatura dei bulbi o delle piante da fiore, dove si arriva a potenze elettriche di 100 W/m2  


# Requisiti Funzionali

In base alle richieste da parte del cliente e da un'attenta analisi in relazione al tipo di coltura scelta, sono stati estratti i seguenti requisiti:  

- Tipo di coltivazione

Per l'implementazione del sistema � stata scelta la coltivazione di piante di Basilico. La medesima coltura richiede i seguenti requisiti:

- Temperatura

Per un ottimale crescita della piantina del basilico la temperatura esterna deve essere compresa tra i 20� ed i 25� diurni ed attorno ad i 18� notturni. Inoltre la stessa non deve scendere mai al di sotto di 10� onde evitare la morte della pianta.

- Umidit� aria/terreno

L'umidit� del terreno non deve essere superiore al 70% al fine di evitare insorgenza di parassiti (malattie come perenospera) e marciume radicale nella pianta. Il basilico necessita tra i 2 ed i 4 l/m^2 di acqua al giorno, forniti tra il tramonto ed il crepuscolo(ore pi� fresche).
L'umidit� dell'aria deve essere compresa tra il 55 ed il 75% e la stessa cresce in funzione della temperatura dell'aria.

- Luce

Il basilico necessita, per una crescita omogenea, un'esposizione luminosa(solare o a luce artificiale) di almeno 10-12 ore.

- Altezza

La pianta � pronta all'uso quando la sua altezza � superiore al 20 cm. Il taglio della parte pi� alta della medesima pu� essere effettuato dopo 60 giorni dalla semina e pu� essere ripetuta successivamente, senza apportare problemi alla pianta, ogni 12-14 giorni. Il taglio pu� essere effettuato ad un'altezza da terra di 15 cm.

In sintesi i dati riferiti all'impianto sono riportati nella tabella in basso:

| Tipo di coltivazione     | Basilico |
| :---:                    | :---:    |
|     Temp. Min [�]        | >18      |
|     Temp.Max[�]          |  20-25   |
|    Umidit� aria[RH%]     |  55-75   |
|    Umidit� terreno[RH%]  |   <70    |
|     Ore Luce             | >10-12   |
|    Altezza uso[cm]       |   20     |
|    Altezza taglio[cm]    |  >15     |


- Controllo Manuale/Automatico

Il cliente ha espressamento richiesto la possibilit� di controllare manualmente, ad esempio, l'attivazione del sistema di irrigazione. Ad ogni modo vuole che la serra sia, in mancanza di personale addetto, controllata autonomanente da parte di un sistema esterno. Quest'ultimo pu� attuare processi al fine di mantenere i parametri dell'impianto all'interno dei range elencati nella tabella in alto.

# Scenari di utilizzo

- Temperatura: il sistema deve monitorare la temperatura ambientale e verificare che si trovi all'interno della fascia definita da Temp.Min e Temp.Max, questi ultimi dettati dalla coltura del basilico. Deve fornire segnalazione al sistema dell'eventuale superamento delle soglie consentite. In modalit� di controllo automatico il sistema deve autoregolare la medesima accendendo un impianto di riscaldamento.
- Umidit� Aria: il sistema deve monitorare l'umidit� ambientale e verificare che si trovi all'interno del range consentito. Deve fornire segnalazione al sistema dell'eventuale superamento delle soglie consentite. In modalit� di controllo automatico il sistema deve autoregolare la medesima accendendo un sistema di umidificazione collegato ad una ventola.
- Umidit� terreno: il sistema deve monitorare l'umidit� del terreno e verificare che si trovi all'interno del range consentito. Al fine di evitare problematiche deve fornire segnalazione al sistema dell'eventuale superamento delle soglie consentite. In modalit� di controllo automatico il sistema deve abilitare o disabilitare un sistema di irrigazione del terreno.
- Luce: il sistema deve monitorare l'illuminazione della serricoltura. Al di sotto di una determinata soglia lo stesso deve abilitare un impianto di illuminazione a raggi ultravioletti.
- Altezza Pianta: il sistema deve monitorare l'altezza della pianta. Superato il livello dei 20 cm di altezza deve segnalare la possibilit� di cimare/raccogliere la piantina.
- Controllo automatico/manuale: il sistema pu� controllare la serricoltura in modo automatico o manuale. Nel primo caso il sistema, mendiante appositi sensori, controlla i vari apparati di attuazione in modo autonomo (come esplicitato negli scenari riportati precedentemente). Nella modalit� manuale il sistema, mediante i comandi forniti da un utente, pu� abilitare o disabilitare i vari ssitemi di attuazione(es.Gestione irrigazione).


# Requisiti non funzionali

Sono stati fissati i seguenti requisiti funzionali all'interno del sistema da realizzare:

1. Interfaccia Utente
- Il sistema pu� essere utilizzato dal proprietario della serra e dai suoi collabotori; lo stesso pu� essere usato da chiunque voglia realizzare un prototipo di serra all'interno di un'ambiente domestico.
- L'interfaccia deve mostrare i dati relativi al monitoraggio dell'impianto e aprire alla possibilit� di controllare automaticamente e manualmente i processi di attuazione all'interno della serra. 

# Ambiente fisico di operativit�

- Il sistema opera all'interno di una serricoltura dove lo stesso viene impiegato.