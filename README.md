# Alice
A Simpler Photo Viewer

Un gestore di librerie fotografiche desktop ultra-veloce, progettato per archivi massivi.

Alice è una galleria fotografica standalone costruita per la velocità assoluta. Progettata per gestire centinaia di gigabyte di dati e decine di migliaia di file senza rallentamenti, mantiene la mente dell'utente in un flusso continuo, eliminando del tutto la presura (lo stress) dei classici caricamenti lenti o dei crash dovuti a librerie troppo grandi.
🚀 Caratteristiche Principali

    ⚡ Prestazioni Estreme: Gestisce librerie da oltre 300+ GB con tempi di avvio quasi istantanei (sotto i 50ms).

    🧠 Virtual Scrolling & Lazy Loading: Le immagini vengono caricate in RAM e renderizzate dalla GPU solo quando entrano nell'area visibile dello schermo, per poi essere distrutte quando escono.

    🏎️ Indicizzazione Multi-Thread: Scansione asincrona parallela che sfrutta tutti i core della CPU per analizzare e indicizzare migliaia di file e metadati EXIF in pochi secondi.

    📦 Miniature On-The-Fly: Le anteprime pesanti non vengono generate in blocco bloccando l'interfaccia, ma calcolate al volo e servite tramite una cache LRU in JavaScript intelligente.

    🎨 UI Frameless Custom: Design moderno, pulito e nativo, con controlli finestra personalizzati e un drag perfetto integrato a livello di sistema operativo (Windows API).

    📁 Gestione Avanzata: Supporto per creazione di Album, Preferiti (con salvataggio rapido in localStorage e SQLite), filtri e visualizzazione dei dettagli del file.

🛠️ Stack Tecnologico

Il software utilizza un'architettura ibrida all'avanguardia per unire la potenza del backend alla flessibilità del web:

    Backend: Python 3

    Database: SQLite3 (con transazioni ottimizzate WAL)

    Ponte di Comunicazione: pywebview (connessione C++/JS)

    Elaborazione Immagini: Pillow (PIL)

    Frontend: HTML5, CSS3, Vanilla JavaScript (Zero framework per la massima efficienza)

    Iconografia: Lucide Icons

📂 Struttura del Progetto
Plaintext

Alice/
├── main.py               # Backend Python, Motore DB, API Webview
├── alice_archivio.db     # Database SQLite (generato al primo avvio)
├── .alice_cache/         # Cartella nascosta per le miniature WebP (generata al primo avvio)
└── ui/
    └── index.html        # Frontend: UI, Stili e logica JavaScript (Radar, Caching, Virtual Rendering)

💻 Installazione e Sviluppo
Prerequisiti

Assicurati di avere Python 3.8+ installato sul tuo sistema.
1. Clona e installa le dipendenze

Apri il terminale nella cartella del progetto ed esegui:
Bash

pip install pywebview Pillow

2. Avvia in modalità sviluppo

Per lanciare l'applicazione ed eseguire i test:
Bash

python main.py

📦 Compilazione (Eseguibile Standalone)

Per distribuire Alice su macchine Windows senza la necessità di installare Python o altre dipendenze, utilizza PyInstaller.

    Installa PyInstaller:
    Bash

    pip install pyinstaller

    Compila l'eseguibile (lancia il comando dalla root del progetto):
    Bash

    pyinstaller --noconsole --name "Alice" --add-data "ui;ui" main.py

    Troverai la tua applicazione pronta all'uso all'interno della cartella dist/Alice. Basterà copiare l'intera cartella su una chiavetta per avere Alice sempre con te.

🤝 Contribuire

Hai un'idea per ottimizzare ulteriormente il caricamento o aggiungere il supporto per nuovi formati RAW? Le Pull Request sono benvenute! Assicurati di non bloccare mai il thread principale della UI nei tuoi commit.
