Alice Photo Viewer

Alice è un gestore di librerie fotografiche desktop progettato per la velocità. È costruito per gestire archivi massivi — centinaia di gigabyte e decine di migliaia di file — evitando i rallentamenti tipici dei visualizzatori standard.

Il cuore di Alice è il mantenimento del Flusso: l'obiettivo è eliminare la "presura" (quello stress da caricamento infinito) per permettere all'utente di scorrere tra i propri ricordi in modo fluido, naturale e senza interruzioni tecniche.
🚀 Caratteristiche

    Progettato per la Velocità: Ottimizzato per gestire librerie da 300GB+ con tempi di risposta immediati.

    Rendering Intelligente: Utilizza Virtual Scrolling e Lazy Loading. Le immagini vengono caricate in memoria e renderizzate via GPU solo quando necessario, liberando risorse appena escono dallo schermo.

    Indexing Multi-Thread: Uno scanner asincrono parallelo analizza file e metadati EXIF senza bloccare l'interfaccia.

    Cache Dinamica: Le miniature vengono generate al volo e gestite tramite una cache LRU (Least Recently Used), garantendo una navigazione fluida anche in cartelle con migliaia di elementi.

    Interfaccia Frameless: Design moderno e pulito con integrazione nativa delle API Windows per il trascinamento della finestra e i controlli di sistema.

    Organizzazione: Supporto nativo per Album, Preferiti e filtri rapidi, con persistenza dei dati tramite SQLite.

🛠️ Stack Tecnologico

Alice sfrutta un'architettura ibrida per unire stabilità e flessibilità:

    Backend: Python 3 (Logica di sistema e I/O)

    Database: SQLite3 con modalità WAL (Write-Ahead Logging) per transazioni rapide.

    Interfaccia: pywebview per la comunicazione a bassa latenza tra Python e il frontend.

    Elaborazione Immagini: Pillow (PIL).

    Frontend: Vanilla JavaScript, HTML5 e CSS3 (Zero framework per la massima leggerezza).

    Iconografia: Lucide Icons.

📂 Struttura del Progetto
Plaintext

Alice/
├── main.py               # Backend, motore DB e API Webview
├── alice_archivio.db     # Database SQLite (generato al primo avvio)
├── .alice_cache/         # Directory nascosta per le miniature WebP
└── ui/
    └── index.html        # UI, Stili e logica JS (Virtual Rendering & Caching)

🤝 Contribuire

Le Pull Request sono benvenute, specialmente se mirate a ottimizzare ulteriormente il caricamento o a supportare nuovi formati RAW. L'unica regola: il thread principale della UI deve rimanere sempre libero per garantire il Chilling
