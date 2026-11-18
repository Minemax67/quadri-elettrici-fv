# Registro delle modifiche

Novità di ogni versione, dalla più recente. Le versioni precedenti alla 2.92 non sono registrate qui.

## 3.36 – Pagina del programma (18 novembre 2026)

- Nella finestra «ℹ Informazioni» compare ora l'indirizzo della pagina del programma su GitHub (https://github.com/Minemax67/quadri-elettrici-fv): è un collegamento su cui si può cliccare. Lì si scarica l'ultima versione e si leggono le novità.
- Nella Guida, capitolo 13, c'è una riga in più che lo cita.
- Non cambia altro: schemi, simulazione, stampe, file SVG esportati e progetti salvati sono identici alla 3.35. Non serve rifare nulla.

## 3.35 – Timer nel simulatore (18 novembre 2026)

- Nella scheda Simulazione, scegliendo lo schema multifilare, dentro la scheda di ogni temporizzatore compare il tempo impostato («imp. 2 s»). Quando il timer è alimentato il conteggio sale («1,4 / 2 s») e una barra si riempie; a tempo scaduto compare la spunta verde.
- Sotto il tempo c'è un piccolo commutatore per ogni contatto in scambio: COM a sinistra, NC in alto (chiuso a riposo) e NO in basso (si chiude a tempo scaduto), con i numeri dei morsetti. La lama passa da NC a NO quando il tempo scade, così si vede quale pin è il comune, quale il normalmente chiuso e quale il normalmente aperto.
- Si simula il ritardo all'eccitazione, che è la funzione più comune. Le altre funzioni dei timer multifunzione non ci sono. I numeri dei contatti sono quelli della libreria del programma: controllali sull'etichetta del tuo temporizzatore.
- Non cambia altro: schemi, stampe, file SVG esportati e progetti salvati sono identici alla 3.34. Non serve rifare nulla.

## 3.34 – Intestazione su due righe (18 novembre 2026)

- In alto ci sono ora il logo, il titolo con la versione e, a destra, i pulsanti «ℹ Informazioni» e «↶ Annulla». Sotto, su tutta la larghezza, ci sono le schede (Fronte quadri, Collegamenti, Schema unifilare…). Prima il titolo e le schede stavano sulla stessa riga e, se la finestra non era abbastanza larga, i due pulsanti finivano su una riga a parte sotto le schede.
- Il logo è un po' più grande (34 punti invece di 26) e l'intestazione è alta circa 25 punti in più. Se la finestra è stretta le schede vanno a capo da sole.
- Non cambia altro: schemi, simulazione, stampe, file SVG esportati e progetti salvati sono identici alla 3.33. Non serve rifare nulla.

## 3.33 – Logo «Minemax» nel programma (18 novembre 2026)

- Il programma ha ora un logo: un lupo davanti a una ruota, con un circuito integrato e delle piste di rame, in blu e ambra. È il logo dell'autore e compare in tre punti: un piccolo distintivo in alto a sinistra, al posto del fulmine, davanti al titolo; l'icona nella scheda del browser (accanto al nome della pagina); e il logo completo, con la scritta «Minemax», in cima alla finestra «ℹ Informazioni».
- Non cambia niente nel resto: schemi, simulazione, stampe, file SVG esportati e progetti salvati sono identici alla 3.32 (il logo non finisce negli SVG scaricati e non si stampa). Il file pesa circa 12 KB in più. Non serve rifare nulla.
- La Guida (capitolo 13) lo cita. Il logo c'è anche in questa edizione condivisa.

## 3.32 – Fronte quadri, «↻ Proponi dai fili» compila «Alimentato da» (18 novembre 2026)

- Se hai già disegnato i fili di un componente non devi più scegliere a mano da chi è alimentato. Nel Fronte quadri seleziona il componente: sotto «Alimentato da» c'è il pulsante «↻ Proponi dai fili». Legge i fili di potenza di quel solo componente (non quelli di comando né la terra) e si apre un riquadro con la proposta: «Alimentato da» e gli eventuali ingressi aggiuntivi (per esempio un MPPT: la batteria come «Alimentato da» e le quattro stringhe come ingressi).
- Non cambia niente finché non premi «Applica». Nel riquadro puoi correggere: il pallino sceglie «Alimentato da», la casella un ingresso aggiuntivo; sotto vedi «Ora» e «Proposto». Con «↶ Annulla» torni com'eri. Cambia soltanto quel componente: gli altri, i fili e i morsetti restano come sono.
- Il riquadro avvisa se qualcosa non torna: se un componente risulta già a valle (la catena sarebbe al contrario e si chiuderebbe un anello) non lo propone, e se la proposta toglierebbe un ingresso che c'è già te lo scrive prima. Le batterie, le stringhe e la rete sono sorgenti: restano «Nessuno».
- Nelle verifiche, accanto all'avviso su uno scaricatore («lo schema unifilare lo disegna sotto… ma i suoi fili…»), c'è lo stesso pulsante: apre la proposta già pronta, e dopo «Applica» l'avviso sparisce.
- I fili non dicono da che parte va la corrente: il programma lo ricava dai morsetti (nei fusibili e negli interruttori l'alto è l'ingresso e il basso l'uscita) e dai nomi (per ATS, UPS, inverter, caricabatterie). Se il tuo cablaggio usa il verso opposto, il riquadro lo scrive («verso incerto») e lascia la scelta a te.
- Gli schemi, la Simulazione e i progetti salvati sono identici alla 3.31: non serve rifare nulla.

## 3.31 – Schema a blocchi, il sezionatore FV a 4 poli ha quattro contatti (17 novembre 2026)

- Nella scheda Multifilare, stile schema a blocchi, il «Sezionatore FV 4 poli, 2 stringhe» veniva disegnato con soli due contatti e i fili delle due stringhe finivano sullo stesso punto («PV1+ in+PV2+ in»). Ora ha quattro contatti, uno per ogni conduttore: PV1+, PV1−, PV2+, PV2−, ognuno con i nomi dei suoi morsetti («in» sopra, «out» sotto) e con il filo di ogni stringa separato dagli altri.
- Vale per i sezionatori messi dalla palette «Aggiungi al quadro» (gruppo «Protezioni DC») o scelti dalla libreria. Se colleghi una sola stringa, il disegno resta a due contatti, come prima.
- Gli altri schemi, il calcolo della Simulazione e i colori dell'unifilare sono identici alla 3.30; i progetti salvati si aprono come prima e non serve rifare i collegamenti.

## 3.30 – Collegamenti, sposta i fili di un morsetto su un altro (17 novembre 2026)

- Se hai collegato un filo al morsetto sbagliato non devi più eliminarlo e rifarlo. Nella scheda Collegamenti clicca il morsetto sbagliato: in basso, accanto a «Collega da qui», compare «↪ Sposta i fili su…» (solo se a quel morsetto è collegato almeno un filo).
- Premi il pulsante, poi clicca il morsetto giusto, anche di un altro componente o, scorrendo la pagina, di un altro quadro. L'altro capo del filo, anche lontano, resta dov'è. Esc o «Annulla (Esc)» per rinunciare.
- Se sul morsetto ci sono più fili, la barra li elenca con una spunta: togli quella ai fili che devono restare dove sono. Con un solo filo non ti chiede nulla.
- Restano uguali il tipo di filo, la sezione, le note e la sigla scritta a mano. La sigla messa dalla numerazione automatica si toglie, perché il filo cambia nodo: si rifà con «Numera i fili senza sigla».
- Il programma non sposta un filo se così collegherebbe un morsetto a sé stesso o se tra i due morsetti c'è già un filo uguale, e te lo dice; gli altri fili scelti si spostano comunque. Con «↶ Annulla» in alto torni indietro.
- Il calcolo della Simulazione e i colori dell'unifilare sono identici alla 3.29; i progetti salvati si aprono come prima.

## 3.29 – Palette, il sezionatore fotovoltaico pronto in «Protezioni DC» (17 novembre 2026)

- Nel Fronte quadri, aprendo il gruppo «Protezioni DC» della palette «Aggiungi al quadro», subito sotto «Sezionatore DC» c'è ora «Sezionatore FV 4 poli, 2 stringhe»: un clic aggiunge il sezionatore già compilato (4 poli, 32 A, 1000 V DC, morsetti PV1+/PV1−/PV2+/PV2− dal lato pannelli e dal lato inverter).
- Prima quell'articolo si trovava solo cercando «sezionatore fv», e la ricerca «sezionatore fotovoltaico» mostrava solo il «Sezionatore DC» vuoto. Ora l'articolo si trova anche con «fotovoltaico», «pannelli», «stringa» e «pv».
- Marca, codice, corrente e tensione sono generici: dopo averlo aggiunto sostituiscili con i dati del tuo pezzo. Le altre ricerche danno gli stessi risultati di prima.
- Il calcolo della Simulazione e i colori dell'unifilare sono identici alla 3.28; i progetti salvati si aprono come prima.

## 3.28 – Simulazione, lo schema subito sotto le schede di stato (17 novembre 2026)

- Nella scheda Simulazione il disegno dello schema finiva in fondo alla pagina, sotto la lunga colonna dei comandi (sorgenti, selettori, interruttori…), e bisognava scorrere molto per vederlo.
- Ora sta nella colonna di destra, subito sotto «Registro eventi»: vedi insieme lo stato (barre, contattori, timer, anomalie) e lo schema che cambia colore. I comandi restano a sinistra.
- Su una finestra stretta le parti si dispongono una sotto l'altra, come prima. Il disegno è un po' più piccolo su schermo largo (circa un quinto): la lente lo ingrandisce dove serve.
- Nella Guida ho corretto la posizione dello stato («in alto a destra»). Il calcolo della Simulazione e i colori dell'unifilare sono identici alla 3.27; i progetti salvati si aprono come prima.

## 3.27 – Importare quadri da un altro progetto, con fili e cavi (17 novembre 2026)

- «Aggiungi quadri da un altro progetto» (scheda Progetto, quadri e file) ora porta con il quadro anche i fili tra i suoi componenti, i cavi di comunicazione, la piastra su misura e il pannello frontale. Prima arrivavano solo il quadro e i componenti, senza fili: bisognava ricollegare tutto a mano.
- Si può così tenere in un file separato un quadro già pronto (un quadro di stringa, un quadro di commutazione rete/inverter, un centralino) e riusarlo in più progetti, adattandolo poi a quello nuovo.
- I fili verso componenti che non si importano restano fuori: vanno rifatti a mano, come i campi «Alimentato da» che puntano fuori dal quadro. Le sigle dei fili messe in automatico vengono tolte; si rifanno con «Numera i fili senza sigla».
- Se un componente ha una sigla già usata nel progetto, il programma non la cambia ma lo scrive nelle note del componente, così lo ritrovi nelle verifiche. Se il nome del quadro esiste già, viene aggiunto «(importato)».
- La finestra di scelta mostra per ogni quadro quanti componenti e quanti fili contiene. Il calcolo della Simulazione e i colori dell'unifilare sono identici alla 3.26; i progetti salvati si aprono come prima.

## 3.26 – Eliminata la scheda Schema ATS (17 novembre 2026)

- La scheda Schema ATS è stata eliminata dal programma. Mostrava un solo schema fisso, disegnato a mano: il commutatore rete/inverter di un impianto preciso (contattori KM1 e KM2, interblocco, temporizzatori). Non serviva ad altri impianti.
- Con la scheda sono spariti i controlli sui fili dell'ATS in Distinta e verifiche e il suo capitolo nella Guida, che ora ha 13 capitoli numerati di seguito.
- Nell'edizione condivisa la scheda non c'era già più: se usi quella, non vedi nessuna differenza. I progetti salvati si aprono come prima, perché la scheda non scriveva nulla nel file.
- Restano lo Schema multifilare dei quadri, il componente «Commutatore / ATS» della libreria e la Simulazione, che non dipendevano dalla scheda. Il calcolo della Simulazione e i colori dell'unifilare sono identici alla 3.25.

## 3.25 – Colori dell'unifilare nella Simulazione con sezionatori cablati al contrario e shunt sul polo − (17 novembre 2026)

- Se un interruttore o un sezionatore è collegato «al contrario», cioè con chi lo alimenta sui morsetti 2-4-6 invece che su 1-3-5 (succede per esempio con un sezionatore batterie con le batterie sui morsetti pari), il disegno scambiava i due lati: con il sezionatore aperto colorava il tratto verso l'utilizzo e lasciava grigio quello verso le batterie. Ora il lato alto del simbolo è sempre quello da cui arriva l'alimentazione, qualunque sia la numerazione dei morsetti.
- Uno shunt sul solo polo − (come il Victron SmartShunt) restava colorato finché c'era il −, anche senza il +: con il sezionatore batterie aperto, o con il fusibile della linea saltato, la linea verso l'inverter risultava ancora in tensione. Ora il tratto è colorato solo se arriva anche il + dal fusibile o dal componente che lo alimenta.
- Con tutto chiuso, e negli impianti di esempio, il disegno è identico a prima. Il calcolo della simulazione non è cambiato: era solo il colore a essere sbagliato.

## 3.24 – Quattro-II, porta GEN dei Luxpower e inverter fotovoltaici on-grid (17 novembre 2026)

- Tra gli inverter di libreria ci sono ora i Victron Quattro-II 24/5000/120-50 e 48/5000/70-50, quelli con due ingressi AC e due uscite: AC-in1 (il generatore, che ha la precedenza) e AC-in2 (la rete), ciascuno con L, N e PE, più AC-out1 (uscita sempre alimentata) e AC-out2 (uscita che si stacca quando si va a batteria). Hanno la sagoma blu dei Multi, con la scritta «Quattro-II».
- I Luxpower SNA 3000 e 4000 WPV hanno ora anche la porta GEN L / GEN N, come gli altri Luxpower. Nei progetti già salvati la porta compare da sola alla prima apertura del file e i fili non vengono toccati.
- Aprendo la finestra ✎ di un Luxpower, di un Quattro-II o di uno dei nuovi inverter compare un riquadro azzurro di promemoria. Per i Luxpower spiega che la porta GEN serve per il generatore, per l'AC coupling o per lo smart load, secondo l'impostazione scelta nell'inverter, e dove si collega un inverter fotovoltaico. Il riquadro non entra nella distinta e non viene salvato nel progetto.
- Nuovi inverter fotovoltaici on-grid, per disegnare un impianto con AC coupling: Fronius Primo 3.0-1, 5.0-1 e 8.2-1; Fronius Symo 5.0-3-M e 8.2-3-M (trifase); FIMER (ex ABB) UNO-DM-3.3, 5.0 e 6.0-TL-PLUS. Hanno gli ingressi dei pannelli, i morsetti AC e le porte dati Ethernet, Wi-Fi e RS485 (sui FIMER anche il comando remote on/off e il relè allarme). Sui FIMER solo il Wi-Fi è integrato: Ethernet, RS485 e relè richiedono una scheda opzionale, e lo dice il riquadro.
- Per ora questi inverter sono solo disegnati e collegati: nella Simulazione non producono tensione. Restano per i prossimi passi le impostazioni di comunicazione già pronte tra il Cerbo GX e i Fronius o i FIMER e la simulazione dell'AC coupling.
- Cose da controllare sul pezzo: di AC-out2 del Quattro-II il manuale non dà la disposizione dei morsetti (qui L e N, con il PE di AC-out1); i nomi A e B dell'RS485 dei Fronius sono generici; i Fronius hanno due coppie di morsetti DC in parallelo per ogni ingresso, mentre qui se ne disegna una; i codici dei FIMER vanno completati con i suffissi del tuo modello (-B, -SB, -Q).

## 3.23 – Sezionatore fotovoltaico generico a due stringhe (17 novembre 2026)

- Tra gli articoli di base c'è ora un «Sezionatore FV 4 poli, 2 stringhe»: quello che si mette subito a valle dei pannelli per sezionare due stringhe insieme (PV1 e PV2, oppure PV3 e PV4). È un articolo generico: marca e codice sono vuoti, mentre 32 A e 1000 V DC si cambiano con i dati del pezzo che hai davvero.
- I quattro poli hanno il nome del conduttore: PV1+ in, PV1− in, PV2+ in, PV2− in dal lato pannelli, e gli stessi con «out» dal lato inverter. Nei collegamenti si capisce subito dove va ogni filo.
- Nella Simulazione ogni polo è un conduttore a sé: aprendo il sezionatore spariscono le tensioni di tutte e due le stringhe a valle, e nello schema unifilare i fili a valle passano al grigio.
- Per usarlo: aggiungi un «Sezionatore DC» al quadro e scegli la voce dall'elenco «Articolo da libreria».

## 3.22 – Avviso sugli scaricatori (SPD) con «Alimentato da» sbagliato (17 novembre 2026)

- Lo schema unifilare disegna uno scaricatore sotto il componente scelto in «Alimentato da», mentre la Simulazione colora seguendo i fili. Se i due non coincidono (per esempio lo scaricatore è collegato a monte di un fusibile ma in «Alimentato da» c'è il sezionatore dopo il fusibile), disegno e colori si contraddicono.
- Ora la scheda «Distinta e verifiche» lo segnala con un avviso giallo: dice cosa trova («i suoi fili sono collegati a monte di QS1…» oppure «non arrivano a…») e, quando è chiaro, quale componente scegliere in «Alimentato da» o negli «Ingressi aggiuntivi».
- Vale solo per gli scaricatori e solo se hanno dei fili: negli impianti di esempio non compare nessun avviso. Non cambia il disegno né la simulazione.

## 3.21 – Corrente continua nell'unifilare: tensione solo se arrivano + e − (17 novembre 2026)

- Nello schema unifilare della Simulazione un tratto di corrente continua si colora solo quando ha tensione, cioè quando arrivano sia il positivo sia il negativo. Prima bastava un polo: con un fusibile saltato su un solo polo e il sezionatore chiuso, il tratto dopo il sezionatore restava colorato perché l'altro polo passava.
- Ora, con il fusibile saltato, il tratto a valle del fusibile, il sezionatore e la linea dopo il sezionatore restano grigi. Un componente a un solo polo, come un fusibile sul positivo, è colorato finché passa il suo polo.
- Sparisce anche il rosso che compariva sullo stesso tratto con un fusibile della batteria saltato (sembrava che due sorgenti si toccassero, ma della batteria arrivava un solo polo).
- Il pannello «Corrente continua» continua a mostrare il dettaglio polo per polo. Con l'impianto intatto i colori sono identici alla 3.20; il motore di simulazione è invariato.

## 3.20 – Scaricatori agganciati a una stringa con TA (17 novembre 2026)

- Quando uno scaricatore (SPD) è appeso a un componente che ha un TA, il punto in cui si aggancia ora sta sotto l'anello del TA e non al suo centro.
- La Guida spiega come scegliere «Alimentato da» per gli SPD: se nel quadro sono collegati a monte di un fusibile o di un interruttore, vanno appesi al componente a monte (per esempio la stringa). Lo schema unifilare si disegna da «Alimentato da», mentre la Simulazione segue i fili: così disegno e colori dicono la stessa cosa.
- Cambia solo il disegno e solo in questo caso: gli altri schemi sono identici alla 3.19.

## 3.19 – Scaricatori nell'unifilare della Simulazione (17 novembre 2026)

- Gli scaricatori (SPD) restano sempre grigi: proteggono, ma non sono una sorgente né un percorso della corrente, anche se i loro morsetti sono collegati al filo della stringa.
- Il filo che porta all'SPD è colorato solo se la stringa che lo alimenta ha tensione. Prima prendeva il colore anche della seconda stringa: in un SPD in comune a due stringhe (per esempio SPD12 per PV1 e PV2) restava arancione anche con PV1 spenta.
- Il collegamento tratteggiato dell'altra stringa resta colorato: è un filo vero e porta la sua tensione.
- Cambia solo il disegno: il motore non è toccato, stesse uscite della 3.18 su 12 scenari.

## 3.18 – Corrente continua nella Simulazione (17 novembre 2026)

- Batterie, stringhe FV e alimentatori sono ora sorgenti in corrente continua. Il positivo e il negativo si seguono polo per polo attraverso sezionatori, interruttori e fusibili chiusi: nel multifilare i fili hanno il colore della sorgente (magenta la batteria, ambra le stringhe, viola gli alimentatori; il positivo è a linea piena, il negativo tratteggiato), nell'unifilare si colorano i tratti.
- L'inverter produce corrente alternata solo se tra BAT+ e BAT− c'è la tensione della batteria. Apri il sezionatore delle batterie, o fai saltare il fusibile sul positivo, e l'inverter si spegne: l'ATS passa alla rete dopo il ritardo del suo timer. Quando la batteria torna, l'inverter riparte. Il controllo vale solo se nel disegno BAT+ e BAT− arrivano davvero a una batteria; altrimenti l'inverter resta come prima (si accende e si spegne a mano).
- Il Cerbo senza alimentazione lascia i relè a riposo. Uno sganciatore (SG) apre da solo l'interruttore a cui è montato quando la sua bobina riceve tensione; per provare il rilevatore d'arco c'è la casella «arco rilevato»: il relè K1 si eccita e gli sganciatori aprono QS1 e QS2. Se la bobina resta alimentata, richiudere l'interruttore non basta: riscatta.
- I fusibili hanno una casella «integro / SALTATO» e nell'unifilare portano la scritta INTEGRO o SALTATO. I fusibili non saltano da soli per sovracorrente: si fanno saltare a mano.
- Nuovo pannello «Corrente continua» nello stato: per inverter, regolatori e Cerbo dice se la batteria e ogni stringa sono presenti, assenti o su un solo polo, e avvisa se le stringhe hanno tensione ma la batteria è scollegata. Il programma segnala come anomalia la polarità invertita.
- Cosa non c'è: correnti, potenze, regolatori di carica (MPPT), ricarica dalla rete, BMS e autonomia. L'inverter è una scatola nera.
- Con la continua intatta le uscite sono identiche a quelle della 3.17 (verificato su 12 scenari e su 20 sequenze casuali di manovre).

## 3.17 – Componenti senza fili nella Simulazione (17 novembre 2026)

- Un interruttore, un sezionatore, un fusibile o un contattore che nella scheda Collegamenti non ha fili (per esempio un sezionatore «previsto», non ancora montato) ora porta la scritta grigia NON COLLEGATO. Resta pallido, come prima, ma non si può più scambiare per un componente aperto o chiuso.
- Per la simulazione quel componente non esiste: le linee che gli passano sopra sono i tratti che collegano i livelli dello schema, e la corrente passa dai fili veri.
- Quando lo monti, sposta i fili sui suoi morsetti: comparirà con CHIUSO o APERTO e con il riquadro colorato, e potrai aprirlo e chiuderlo dall'elenco «Interruttori e fusibili».
- Il motore della simulazione non è cambiato: stesse uscite della 3.16 (verificato su tre scenari).

## 3.16 – Stato dei contatti nella Simulazione (17 novembre 2026)

- Nello schema unifilare della Simulazione gli interruttori magnetotermici, i differenziali, i sezionatori e i fusibili mostrano sempre CHIUSO o APERTO, come già i contattori. Prima la scritta compariva solo quando il componente era aperto.
- Dietro ogni simbolo c'è un riquadro colorato: verde se è chiuso, rosso se è aperto. Così lo stato si legge anche da lontano, anche per i simboli piccoli come il sezionatore.
- La scritta si mette in un punto libero accanto al riquadro, senza coprire altre scritte. Il motore della simulazione non è cambiato: stesse uscite della 3.15 (verificato su tre scenari).
- Nella Guida, il capitolo Simulazione e la legenda sotto lo schema descrivono i riquadri.

## 3.15 – Scheda Simulazione, licenza e firma (16 novembre 2026)

- Nuova scheda Simulazione: accendi e spegni rete e inverter, sposta i selettori, chiudi o apri i contatti, e guarda quali contattori si chiudono, quali relè si eccitano e quali timer partono, con il registro di ogni commutazione. Lo schema mostrato è colorato in base a chi alimenta cosa (blu rete, verde inverter) e accanto a ogni contattore compare CHIUSO o APERTO. Non scrive nulla nel progetto.
- La simulazione segue la parte in corrente alternata e il comando (contattori, timer, relè, selettori, gruppo di continuità, relè del Cerbo GX). Inverter, regolatori di carica e caricabatterie non sono simulati, e nemmeno l'autonomia del gruppo di continuità.
- Lente: passando il mouse sullo schema si vede la zona ingrandita. Tasto L per accenderla e spegnerla, + e − per cambiare l'ingrandimento.
- Il programma ora è libero e gratuito, con licenza GNU GPL versione 3 o successive. Puoi usarlo, copiarlo e condividerlo; chi lo modifica e lo ridistribuisce deve mantenere la stessa licenza, indicare le modifiche e conservare il nome dell'autore. Non c'è nessuna garanzia: è un ausilio al disegno e non sostituisce il progetto di un professionista.
- Pulsante «ℹ Informazioni» in alto a destra: versione, autore, licenza e avviso sulla garanzia.
- Negli SVG scaricati o copiati e nelle stampe compare in fondo una piccola riga con il nome del programma e dell'autore. Si disattiva dalla finestra Informazioni. Se in una copia modificata i dati dell'autore vengono alterati, compare una striscia rossa in alto.
- Guida: due capitoli nuovi, «12. Simulazione» e «13. Informazioni e licenza».

## 3.14 – Porte dati su Cerbo GX e sugli altri apparecchi

- Il Cerbo GX della libreria aveva solo alimentazione, relè, ingressi digitali e temperatura. Ora ha tutte le porte: Ethernet, VE.Bus, VE.Can, BMS-Can, 3 VE.Direct, 3 USB e HDMI, più gli ingressi temperatura 3 e 4 e i 4 ingressi livello serbatoio (TNK1–4). C'è anche il Cerbo GX MK2, con due VE.Can.
- Anche gli altri apparecchi hanno le loro porte, controllate sui datasheet e sui manuali dei produttori: VE.Bus e relè programmabile sul MultiPlus-II (con Ethernet, VE.Can, VE.Direct e USB sulle versioni GX), VE.Direct su SmartSolar e SmartShunt, VE.Direct e VE.Can sugli MPPT RS, RS485 sui contatori ET112, ET340, EM540, EM24, EM112 ed EM111, Ethernet e VE.Can sul VM-3P75CT, Ethernet sugli Shelly Pro, RS485 sui gateway Elfin. Nei Luxpower SNA: porta batteria RS485/CAN, WiFi o dongle, CT, parallelo e contatti a secco. Nei Voltronic Axpert: USB, RS232, BMS e, dove il datasheet lo dà, parallelo e ripartizione di corrente.
- Sono nuove anche le sei versioni con VE.Can dei SmartSolar -Tr 150/70, 150/85, 150/100, 250/70, 250/85 e 250/100.
- Nei progetti già salvati le porte nuove si aggiungono da sole la prima volta che li apri: i fili restano dove sono e nessun morsetto cambia nome. Se avevi già cambiato dei morsetti a mano, restano i tuoi e le porte nuove vanno in fondo.
- Nella finestra dei morsetti (la matita ✎) una barra | tra i morsetti dice quali vanno sopra e quali sotto. I nomi lunghi (VE.Direct 1, Ethernet…) hanno un morsetto più largo, così le scritte non si sovrappongono.
- Nella scheda Comunicazione i campi «porta» propongono prima le porte vere dell'apparecchio scelto.
- Non ho aggiunto ciò che non ho potuto verificare: il parallelo dei Voltronic VM III e delle versioni TWIN, i contatti NC dei SNA-EU 12K e 14K, i pin ausiliari del MultiPlus-II e le porte degli altri apparecchi di rete (switch, router, telecamere: restano il numero «porte» della scheda Rete).

## 3.13 – Schema unifilare più basso

- Prima tutti i livelli dello schema unifilare avevano la stessa altezza, calcolata sul livello con più collegamenti blu e cavi viola, anche dove non passava nessuna linea. Ora ogni livello ha l'altezza che gli serve davvero: quella normale se da lì non parte nessun collegamento o cavo, più alta solo sotto i livelli da cui ne partono.
- I componenti sono quindi più vicini e il disegno è più corto: nell'esempio a 7,2 kW lo schema completo è più basso di circa il 12%; con tanti cavi di comunicazione il guadagno è molto maggiore.
- Nulla cambia nelle scritte, nei collegamenti e nel multifilare. Anche le batterie in parallelo (la barra «parallelo batterie») non fanno più allargare tutti i livelli.

## 3.12 – Cavi di comunicazione più distanziati nello schema unifilare

- Quando a uno stesso dispositivo arrivano più cavi viola (tipico il Cerbo GX, collegato a shunt, regolatori, contatori e batterie), le linee non corrono più ammassate: ognuna ha il suo canale verticale a 16 punti dalla vicina e il suo punto d'attacco sul simbolo, in un ordine che evita gli incroci.
- La colonna di quel dispositivo si allarga a sinistra per fare posto; due dispositivi nella stessa colonna non usano mai lo stesso canale.
- Anche le corsie orizzontali con le scritte («COM1 · CAN»…) sono più distanziate (14 punti invece di 11).
- Se non hai cavi di comunicazione, gli schemi restano identici alla 3.11.

## 3.11 – La scheda Rete

- C'è una nuova scheda, «Rete», dopo Comunicazione. Disegna la rete dati: router, switch, telecamere, gateway Wi-Fi/RS485 (come l'Elfin EW11) e PC, con le porte usate e il luogo dove sta ogni apparecchio. Serve per documentare anche ciò che sta fuori dal quadro elettrico.
- Dal menu in alto scegli un apparecchio (per esempio lo switch HP ProCurve 2610-24/12PWR, il FRITZ!Box 7490, l'Elfin EW11, un generico switch a 5, 8, 16 o 24 porte, una telecamera) e premi Aggiungi: finisce in un quadro chiamato «Rete». Cliccando il suo riquadro cambi sigla, ubicazione (per esempio «Rack batterie» o «Esterno»), indirizzo IP, numero di porte e porte PoE.
- I collegamenti si inseriscono come cavi nella scheda Comunicazione, dove ci sono nuovi abbinamenti (Switch → router, Switch → telecamera PoE, Gateway → router Wi-Fi, Mini PC → BMS…) e i nuovi tipi Ethernet PoE e Wi-Fi. Sui due lati del cavo scrivi il numero della porta.
- Nello schema il router sta in alto e gli apparecchi seguono a livelli. Linea blu = cavo di rete, arancione = PoE, verde-acqua puntinata = Wi-Fi, viola tratteggiata = collegamento seriale (RS485, USB). Ogni ubicazione ha il suo colore. Cliccando un riquadro si apre l'apparecchio per modificarlo.
- Sotto lo schema trovi l'elenco degli apparecchi e, per switch e router, la tabella porta per porta con le porte libere; una porta usata da due cavi è in rosso. C'è anche la stampa, il file SVG e la lista dei collegamenti da copiare.
- I cavi Wi-Fi, PoE e quelli che toccano un apparecchio di rete non compaiono negli schemi unifilare e multifilare, che restano come prima. Gli articoli di rete in libreria hanno solo dati di scheda tecnica, senza prezzi. Non c'è ancora il controllo automatico delle porte.

## 3.10 – I cavi di comunicazione negli schemi unifilare e multifilare

- Nello schema unifilare i cavi della scheda Comunicazione sono ora linee tratteggiate viola (trattino e punto) tra i simboli dei due dispositivi, con scritti sigla, protocollo e lunghezza, per esempio «COM1 · CAN · 2 m». Escono dal lato sinistro del simbolo e hanno una corsia propria, così non si sovrappongono. Se l'altro capo del cavo non è nel disegno (per esempio perché nel menu «Mostra» hai scelto un solo quadro) accanto al simbolo compare «COM1 ⇢ GX1». Nel cartiglio c'è la legenda.
- Nello schema multifilare, stile «Schema con simboli», in fondo c'è la nuova sezione «Circuito di comunicazione»: i dispositivi dei cavi che toccano il quadro scelto sono riquadri, con il nome delle porte («CAN», «VE.Direct»…) e i cavi tratteggiati in mezzo, con sigla, protocollo e lunghezza.
- In tutte e due le schede c'è la casella «cavi di comunicazione» per mostrare o nascondere questi disegni, anche nella stampa e nel file SVG. Se non hai inserito cavi, gli schemi restano esattamente come prima.
- Non c'è ancora un controllo automatico di compatibilità tra batteria e inverter: è il passo successivo.

## 3.09 – Scheda Comunicazione: i cavi dei dati tra batterie, inverter e Cerbo GX

- C'è una nuova scheda, «Comunicazione», dopo lo Schema multifilare. Serve per annotare i cavi che portano i dati e non la potenza: il CAN o l'RS485 tra la batteria (BMS) e l'inverter o il Cerbo GX, il VE.Can, il VE.Direct e il VE.Bus di regolatori e shunt, l'RS485 dei contatori Carlo Gavazzi, la rete dei Shelly. Non sono fili degli schemi: e hanno una lista propria; dalla 3.10 si vedono anche negli schemi (vedi sotto).
- Si parte da un abbinamento del menu (per esempio «JK PB → Cerbo GX (CAN)», «TianPower → Voltronic Axpert MAX (RS485)», «Basen Green → LuxPower (CAN)»): il programma compila bus, pin su ogni lato, protocollo da scegliere sulla batteria e impostazioni da fare sull'inverter, e cerca da solo la batteria e il Cerbo GX nel tuo progetto. Oppure si parte da un cavo vuoto.
- Ogni cavo ha uno stato: «documentato» (c'è un manuale o una prova sul campo), «dedotto» (ricavato da altri modelli) o «da provare» (nessuna conferma). I pin dei vari abbinamenti vengono da una ricerca sui manuali fatta a novembre 2026: prima di crimpare controlla sempre il manuale o l'etichetta del tuo apparecchio. Per esempio i pin delle TianPower sono quelli delle EG4, e quelli dell'Axpert sono del MAX II da 8 kW.
- La «Lista per la crimpatura» mostra, per ogni cavo con connettori RJ45, i due connettori con il pin e il colore di ogni filo (standard T568B; il colore suggerito è quello che lo standard mette sul pin del lato A, ma si può cambiare). Il programma avvisa se un pin è usato due volte, se due fili hanno lo stesso colore, se manca un componente, e ricorda quando i due fili di un segnale stanno su doppini diversi, come i pin 3 e 5 dell'Axpert.
- Distinta e verifiche elencano i cavi di comunicazione per tipo, con la lunghezza totale. I cavi si salvano nel file del progetto (.json) e compaiono nello storico delle modifiche. Eliminando un componente si tolgono anche i suoi cavi; Annulla li riporta.
- Nella Guida c'è il nuovo capitolo «Comunicazione tra i dispositivi».

## 3.08 – Contatori Carlo Gavazzi e Shelly, con le note d'uso con Victron

- In libreria, tipo «Misuratore / Shelly», ci sono ora i contatori Carlo Gavazzi ET112, ET340, EM540, EM24, EM112 ed EM111 e i Shelly Pro EM-50, Pro 3EM, Pro 3EM-400, Pro 3EM-3CT63, Pro 1PM, Pro 2PM e Pro 4PM, accanto ai Victron ET112, ET340 (nuovo), EM540 e VM-3P75CT.
- Scegliendo uno di questi articoli compare, sotto il codice, un riquadro azzurro «Uso con sistema Victron»: dice come si collega al Cerbo GX (per esempio con l'interfaccia Victron RS485 to USB, un contatore per interfaccia) e che cosa è documentato o no. È un promemoria: non finisce in distinta e non viene salvato nel progetto.
- Il Shelly Pro 3EM ora è largo 1 modulo (la scheda tecnica dà 19 mm), non 3 come prima. Un Pro 3EM già inserito nel tuo progetto resta com'è: se è a 3 moduli lo cambi nella scheda delle proprietà.
- Le larghezze di EM24 (4 moduli), EM112 (2) ed EM111 (1) sono da confermare sul prodotto.

## 3.07 – Un simbolo per ogni polo del sezionatore

- Nello schema multifilare un sezionatore con un polo per ogni batteria (2 poli per due batterie, 4 poli per tre) veniva disegnato con un solo polo positivo e i morsetti scritti insieme (1+3 sopra, 2+4 sotto), come se le batterie si unissero prima del sezionatore. Ora ogni polo ha il suo simbolo, il suo fusibile e i suoi morsetti. Vale per qualsiasi interruttore o sezionatore con più poli dello stesso tipo: un 4P trifase si disegna con quattro poli (L1, L2, L3, N). Gli interruttori con un solo polo per tipo (fase e neutro, positivo e negativo) sono disegnati come prima. I fili del progetto non cambiano.

## 3.06 – Esempi rifatti: una batteria per polo, shunt fuori dal sezionatore

- Negli impianti di esempio (quello generico del pulsante «Carica impianto FV di esempio» e il file di esempio a 7,2 kW, non più pubblicato nel repository) il negativo delle batterie passava da un polo del sezionatore prima di arrivare allo shunt, e le batterie stavano tutte sullo stesso polo positivo. Nella pratica lo shunt non passa mai da un sezionatore: ora ogni batteria ha il suo fusibile e il suo polo del sezionatore sul positivo (2 poli per due batterie, 4 poli per tre), i negativi di tutte le batterie vanno diretti al BATT− dello shunt, e l'uscita LOAD− va alle barre del negativo. Il file 7,2 kW è stato sostituito: se l'avevi già aperto e modificato, tieni il tuo; questo serve solo come esempio.
- Nello schema multifilare in continua il sezionatore ora sta sempre sopra le barre anche quando le barre sono alimentate dallo shunt (prima, in quel caso, restava appeso sotto). Gli altri schemi non cambiano.

## 3.05 – Sezionatore batterie e shunt nel multifilare (corretto)

- Nello schema multifilare in continua, quando lo shunt è collegato al morsetto in alto di un sezionatore (per esempio il 3 del polo negativo di un sezionatore batterie a 2 poli), il polo sembrava aperto: il 3 e il 4 comparivano insieme sotto e il filo dello shunt pareva partire dal sezionatore. Ora il filo dello shunt risale, passa sopra il polo e rientra dall'alto: il 3 sta sopra, il 4 sotto, e il polo è in serie. I fili del progetto non cambiano, cambia solo il disegno.

## 3.04 – Collegamenti tra i quadri (nuovo)

- Nella scheda Schema multifilare, nel menu Stile, c'è una voce nuova: «Collegamenti tra i quadri (tabella)». Mostra i soli fili che uniscono componenti di quadri diversi, una tabella per ogni coppia di quadri: componente e morsetto di partenza, sigla del filo, sezione, tipo (fase, neutro, terra, positivo, negativo, comando), componente e morsetto di arrivo, note. Serve per tirare i cavi tra un armadio e l'altro.
- Nel menu del quadro si sceglie «Tutti i quadri» oppure un quadro solo: in quel caso vedi i suoi fili verso gli altri, con il quadro scelto sempre a sinistra.
- I fili senza sigla o senza sezione sono segnati con «—» in arancione e contati in fondo: si vede subito cosa manca. Si stampa e si scarica come gli altri schemi.

## 3.03 – Ricerca negli elenchi «Alimentato da» e «Ingressi aggiuntivi» (nuovo)

- Nelle proprietà di un componente, sopra «Alimentato da» e sopra «Ingressi aggiuntivi» c'è ora una casella di ricerca. Scrivi parte della sigla, del nome, del codice o del quadro (anche più parole, per esempio «fus bat») e nell'elenco restano solo le voci che corrispondono. Invio sceglie la prima, Esc svuota la ricerca.
- Gli elenchi sono ora ordinati: prima per quadro (nell'ordine dei quadri, con il nome del quadro come intestazione), poi per sigla. Prima l'ordine seguiva la posizione sulla guida e sembrava casuale.
- Negli ingressi aggiuntivi un clic su una voce la aggiunge o la toglie, senza dover tenere premuto Ctrl e senza perdere le altre.

## 3.02 – Scaricatori DEHN per due stringhe, 5 moduli (nuovo)

- I due scaricatori DEHN da guida DIN per due stringhe, il 952514 e il 952519 (con contatto di segnalazione), sono ora importati con la larghezza di 5 moduli, come dalla scheda tecnica DEHN. Il 900920 è in una custodia e non ha una larghezza in moduli. Per tutti gli altri articoli DEHN la larghezza resta quella standard del tipo, da controllare sul catalogo. Va reimportato il listino DEHN.

## 3.01 – Scaricatori DEHN per due stringhe (nuovo)

- Nel listino DEHN i modelli «2MPP» (codici 900920, 952514 e 952519) proteggono due stringhe con un solo scaricatore; il 900910 («1MPP») ne protegge una. Ora la descrizione lo dice («per 2 ingressi MPPT (due stringhe)»), quindi cercando «due stringhe» nella ricerca del quadro o nel campo Articolo da libreria li trovi. Il secondo ingresso si collega con il campo Ingressi aggiuntivi del componente, come nell'impianto di esempio: la nota dell'articolo lo ricorda. Va reimportato il listino DEHN per avere le nuove descrizioni.

## 3.00 – Scaricatori DEHN dal listino (nuovo)

- Il comando Importa listino produttore, nella scheda Progetto, quadri e file, legge ora anche il listino prezzi DEHN Italia in formato Excel (file .xlsx, anche dentro lo zip che di solito si chiama XLS_DEH…). Il programma riconosce da solo la marca. Il file METEL di DEHN (DEHLSP…) non viene letto: il programma lo dice e chiede l'Excel.
- Si importano solo gli scaricatori di sovratensione: 278 in alternata (DEHNguard, DEHNshield, DEHNventil, DEHNbloc, Tipo 1, 2 e 3) e 48 in continua (fotovoltaico, batterie). Il codice è il numero d'ordine a sei cifre; nella descrizione c'è anche il nome del modello (per esempio DG M TNC 275). Poli e tensione vengono dal nome; per gli scaricatori in continua la tensione va nel campo Tensione.
- Non si importano moduli di ricambio, linee dati, TV, telefono, parafulmini, dispersori e il resto del listino. Il listino non dà la larghezza in moduli: resta quella standard, da controllare sul catalogo. Alcuni articoli hanno una nota nel campo Note (per esempio i moduli «per N» e tre modelli da 1000 V di cui non si sa se sono in alternata o in continua): leggila prima di usarli.
- ABB, Finder, Chint e DEHN possono stare insieme; se reimporti una marca, il suo catalogo viene sostituito, senza doppioni. Nella Guida, capitolo 7, c'è la sezione Listino DEHN.

## 2.99 – Schede in un nuovo ordine (nuovo)

- Le schede in alto seguono ora l'ordine del lavoro: Fronte quadri, Collegamenti, Schema unifilare, Schema multifilare, Distinta e verifiche, Progetto, quadri e file, Guida. La scheda Multifilare si chiama ora Schema multifilare. Non cambia nient'altro: i capitoli della Guida restano nell'ordine di prima.

## 2.98 – Guida più leggibile (nuovo)

- Nella Guida, capitolo 7 (Progetto, quadri e file), la parte sulla libreria articoli era un unico blocco di testo lunghissimo. Ora è divisa in sezioni con il titolo: Libreria articoli e cataloghi dei produttori, Cercare un articolo, Listino ABB, Catalogo Finder, Listino Chint, Salvare, ripristinare e unire i progetti. Ogni marca ha voci brevi (file da scaricare, famiglie, bobina, morsetti, larghezza, cosa non si importa) e le famiglie sono elencate una per riga. Il contenuto è lo stesso di prima.

## 2.97 – Accessori Chint: contatti e sganciatori (nuovo)

- L'importazione del listino Chint porta ora anche 127 accessori degli interruttori: 18 contatti ausiliari e di allarme (XF9, AX, AL) e 109 sganciatori, a lancio di corrente (S9, SHT, NM8N-SHT) e di minima tensione (V9, UVT, NM8N-UVT), alcuni anche di sovratensione. Nella finestra di importazione trovi una famiglia in più, Accessori; il totale degli articoli Chint passa da circa 2.200 a 2.332.
- Per gli sganciatori si legge la tensione di bobina (24 V AC/DC, 230 V AC, 12-24 V…) e si vede anche nelle liste e nella ricerca: cercando sganciatore 24 v trovi quelli giusti. Ricerche utili: sganciatore, minima tensione, s9, sht, xf9, contatto ausiliario.
- Il listino non dice su quale interruttore si monta ciascun accessorio (qualche volta c'è «per NB8-125» o la taglia): quando manca, nelle note dell'articolo trovi l'invito a controllare sul catalogo. Dieci sganciatori non hanno la tensione scritta nel listino. La larghezza è nota solo per S9, V9 e XF9R; per gli altri vale quella standard del tipo.
- XF9 e XF9J erano già nella libreria e non si ripetono; S9 e V9 della libreria e quelli del listino (S9/24, S9/230, V9/230…) compaiono vicini, con codici diversi. Come sempre gli accessori si montano a sinistra dell'interruttore a cui li colleghi e si vedono nel fronte, nei collegamenti e nella distinta (non nello schema unifilare).
- Non ci sono le bobine di chiusura, i blocchi contatti dei contattori, i contatti degli interruttori aperti NA1, le barre di collegamento e le maniglie.

## 2.96 – Listino Chint (nuovo)

- Lo stesso comando Importa listino produttore ora legge anche il listino prezzi Chint in formato Excel (file .xlsx, anche dentro lo zip, che trovi nell'area Download del sito chint.it). Il programma riconosce da solo se il file è ABB, Finder o Chint.
- Si importano circa 2.200 articoli (più gli accessori, vedi sopra): magnetotermici modulari (NB1-63, NXB, NB2, NB8, Ex9B, eB, DZ158), magnetotermici per corrente continua (NB1-63/DC), magnetotermici differenziali (NB1L, NB2LE, NXBLE, NXBL), differenziali puri e blocchi differenziali (NL1, NL210, NXL), sezionatori modulari (NH4, NXHB, NH9) e per corrente continua (BTY2, NM8NSD), scaricatori in alternata (NXU, NU6, JSP) e per fotovoltaico (Ex9UEP, OBV5), portafusibili e fusibili gPV, contattori (NC1, NC2, NC6, NC8, NXC, NCH8), relè NXJ e passo-passo NJMC1, commutatori automatici NXZ.
- Come codice si usa il modello scritto nel listino (per esempio NB1-63/C16-2P-6), non il codice d'ordine numerico. I modelli uguali con codice d'ordine diverso compaiono una volta sola. I prezzi non si importano.
- Attenzione: il METEL di Chint non va bene, perché tronca le descrizioni a 40 caratteri; il programma lo dice e chiede l'Excel. La larghezza in moduli c'è per circa un terzo degli articoli (NB1-63 e NXB-63: 18 mm per polo): per gli altri resta quella standard del tipo, controllala sul catalogo. Nei contattori la corrente è quella AC-3 (AC-1 per i quadripolari) scritta nel listino e la bobina è in alternata se il listino non dice DC. Non ci sono interruttori scatolati e aperti, gli altri accessori, temporizzatori e fusibili a cartuccia.
- ABB, Finder e Chint possono stare insieme; se reimporti la stessa marca il suo catalogo viene sostituito, senza doppioni. Dopo l'importazione dai un'occhiata ai dati dell'articolo scelto.

## 2.95 – Ricerca degli articoli più chiara (nuovo)

- Nella casella «Cerca» a sinistra e nel campo «Articolo da libreria» ogni articolo ora mostra anche la descrizione, per esempio «Relè a interfaccia 2 scambi 8 A, morsetti a vite · bobina 24 V AC»: si distingue un relè a uno scambio da uno a due scambi senza aprirlo.
- Nella casella «Cerca» puoi combinare le parole (finder 2 scambi 24 v). Un numero seguito da scambi, V, A, kA, NA o NC viene cercato intero: «2 scambi» non trova più «1 scambio» e «24 v» non trova 220 V.
- Contattori ABB: la corrente è la stessa per tutte le tensioni di bobina dello stesso modello (prima, per esempio, l'AF52-40-00 aveva 100 A con alcune bobine e 52 A con altre).

## 2.94 – Relè e contattori Finder (nuovo)

- Lo stesso comando Importa listino produttore ora legge anche il catalogo elettronico di Finder (formato BMEcat/ETIM, file .zip o .xml con nome tipo FINBMECAT_ENG_…, che trovi nell'area download del sito Finder). Il programma riconosce da solo se il file è ABB o Finder.
- Si importano circa 3.700 articoli: relè a interfaccia per guida DIN (serie 38, 39, 48, 4C, 58), relè a innesto (serie 40, 41, 43, 45, 46, 55, 56, 60, 62, 65, 66), contattori modulari serie 22, relè passo-passo serie 20 e contattori serie 6K. Per ogni articolo si compilano codice, contatti (scambio o solo NA), corrente, tensione e tipo della bobina (AC, DC, AC/DC) e morsetti (A1-A2 e 11-12-14, 21-22-24…): il multifilare disegna bobina e contatti.
- ABB e Finder possono stare insieme: importare l'uno non cancella l'altro. Se reimporti la stessa marca, il suo catalogo viene sostituito, senza doppioni.
- Attenzione: per i relè della serie 60 con bobina «multitensione» la tensione non è un numero solo: il programma scrive «AC/DC (multitensione, vedi codice)», controllala. La larghezza in moduli c'è per i relè a interfaccia, i contattori serie 22 e i passo-passo; per i relè a innesto e per la serie 6K resta quella standard. Non ci sono zoccoli, relè bistabili, temporizzatori, relè di controllo e relè statici.

## 2.93 – Contattori, relè e alimentatori (nuovo)

- L'importazione del listino ABB ora comprende anche contattori di potenza (AF, AS, UA, EK, GAF, modulari ESB ed EN, minicontattori B6/B7), relè ausiliari (NF, K6), relè a interfaccia (CR-P, CR-M, CR-U) e alimentatori monofase CP: in tutto circa 3.900 articoli invece di 2.600. Per averli devi importare di nuovo il listino (basta ripetere l'operazione, i progetti già fatti non cambiano).
- Applicando un contattore al componente si compilano codice, poli, corrente, tensione della bobina e morsetti (1L1-2T1, 3L2-4T2, 5L3-6T3, bobina A1-A2). Per i relè si compilano anche i morsetti dei contatti, e il multifilare li disegna con i loro simboli.
- Attenzione: la corrente dei contattori è quella di impiego in AC-3 ricavata dal numero del modello (AF09 = 9 A): controllala sul catalogo. La larghezza in moduli non viene importata. Dei relè a interfaccia si importa il relè senza zoccolo. Timer, relè termici, salvamotori e scatolati per ora non ci sono.
- Corretto anche un difetto dei file SVG scaricati dai multifilari: alcuni programmi non li aprivano. Ora sono validi.

## 2.92 – Importa listino produttore (nuovo)

- Nella scheda Progetto, quadri e file, sezione Libreria articoli, c'è il pulsante Importa listino produttore. Serve per avere nella lista degli apparecchi anche magnetotermici, differenziali, scaricatori e fusibili fotovoltaici che non sono nella libreria di base, senza scriverli a mano.
- Per ora funziona con il listino ABB. Lo scarichi dal sito ABB (new.abb.com/low-voltage/it/area-tecnica/listino-prezzi): va bene il file Excel, anche se è ancora dentro lo zip, oppure il file METEL. Il programma lo legge da solo, in pochi secondi, senza inviare nulla su internet.
- Prima di confermare vedi le famiglie di prodotti trovate (S200, S700/S800, differenziali, scaricatori OVR, S800 PV, fusibili e sezionatori fotovoltaici) e quanti articoli verrebbero importati: puoi togliere la spunta a quelle che non ti servono. Gli articoli importati sono circa 3.900 (dalla 2.93, con contattori e relè).
- Gli articoli importati compaiono nella ricerca di Aggiungi al quadro e nel campo Articolo di libreria dei componenti. Scrivendo parole come «ABB S202 C16» l'elenco si restringe. Sono già compilati codice, corrente, curva, poli e potere di interruzione.
- Attenzione: per circa un quarto degli articoli il listino non dice quanti moduli è largo: in quel caso resta la larghezza standard del tipo, da controllare sul catalogo. I prezzi non vengono importati.
- Il listino resta nel browser di questo dispositivo, non dentro il file .json del progetto: su un altro computer va importato di nuovo. Un impianto salvato non dipende dal listino. Conviene rifarlo ogni tanto, quando ABB pubblica il nuovo.
