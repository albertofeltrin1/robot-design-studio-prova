# Robot Design Studio — versione di prova

**Robot Design Studio** è un software per Windows che accompagna la progettazione di un robot industriale a braccio, dall'idea al dimensionamento dei componenti. Interfaccia e report in italiano e in inglese.

## Scaricare e installare

1. Aprire la pagina **[Releases](../../releases/latest)** e scaricare `Robot.Design.Studio.Setup.0.2.0.exe`.
2. Avviare il file. L'installer non è firmato digitalmente: Windows può mostrare «Windows ha protetto il PC». Cliccare **«Ulteriori informazioni»** e poi **«Esegui comunque»**.
3. Aprire **Robot Design Studio** dal menu Start. Non serve installare altro: il motore di calcolo è incluso.

Per una prima prova: **«Carica il progetto UR5 completo»** → **«Genera report»**, poi **«Robot 3D →»** per la vista interattiva e **«Modifica progetto»** per l'editor.

## Il problema che risolve

Progettare un robot richiede molti calcoli collegati tra loro: movimento, forze nei giunti, scelta di motori e riduttori, resistenza della struttura, cuscinetti, vibrazioni, ingombri. Di solito si usano strumenti diversi e scollegati, e ogni modifica (un componente più pesante, un ciclo più veloce) costringe a rifare tutto a mano. Robot Design Studio riunisce questi calcoli in un unico flusso e li ripete in automatico quando qualcosa cambia.

## Cosa fa

- **Descrizione del robot:** parametri geometrici nella convenzione standard della robotica (Denavit-Hartenberg) e requisiti del cliente (carico, velocità, ciclo di lavoro).
- **Movimento e forze:** posizioni raggiungibili, traiettorie, forze e coppie in ogni giunto lungo il ciclo di lavoro.
- **Scelta dei componenti da catalogo:** motori, riduttori e cuscinetti di produttori reali; la scelta viene ripetuta finché la soluzione è coerente, perché ogni componente aggiunge peso e carico.
- **Verifica della struttura:** analisi agli elementi finiti dei link con le sollecitazioni reali del ciclo, verifica di alberi e collegamenti a vite secondo le norme tecniche, durata dei cuscinetti.
- **Comportamento dinamico:** frequenze proprie del robot.
- **Collisioni:** controllo del robot nella cella di lavoro.
- **Ottimizzazione:** miglior compromesso tra peso del robot e tempo ciclo.
- **Compensazione del peso:** progetto di una molla di bilanciamento con scheda tecnica per il fornitore.
- **Documenti:** report completo (HTML e PDF), distinta base in Excel, geometria dei link per SolidWorks, modello per la simulazione in MATLAB/Simscape.

## Visualizzazione

Vista 3D interattiva del robot con il ciclo di lavoro animato e la mappa delle sollecitazioni sulla struttura; editor del progetto con anteprima 3D aggiornata durante la modifica.

## Affidabilità

- Ogni valore è marcato come dato di catalogo (con la fonte), ipotesi o mancante: il report dichiara sempre su cosa si basa ogni risultato.
- I risultati sono confrontati con metodi indipendenti e con la simulazione in MATLAB/Simscape.
- Centinaia di test automatici a ogni modifica del software.
- Provato su un robot collaborativo commerciale noto, ricostruito dai dati delle schede pubbliche.

## Stato e sviluppi

Software funzionante e installabile. Prossimi passi: conferma dei modelli in SolidWorks, ampliamento dei cataloghi, validazione su robot reali, verifiche di sicurezza secondo le norme sui robot industriali.

## Licenza

Software proprietario. © 2026 Alberto Feltrin, tutti i diritti riservati. L'installer è messo a disposizione **solo per la valutazione**; non è concesso alcun diritto di copia, modifica, distribuzione o uso commerciale. Il codice sorgente non è pubblico.

---

*English: Robot Design Studio is a Windows application for designing serial industrial robot arms, from kinematics to component sizing. Download the installer from [Releases](../../releases/latest). Proprietary software, evaluation only, all rights reserved.*
