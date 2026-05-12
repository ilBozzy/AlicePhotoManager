Alice
A Simpler Photo Viewer

Alice è un gestore di librerie fotografiche desktop progettato per la velocità. È costruito per gestire archivi massivi — centinaia di gigabyte e decine di migliaia di file — evitando i rallentamenti tipici dei visualizzatori standard.

Il cuore di Alice è il mantenimento del Flusso: l'obiettivo è eliminare la "presura" (quello stress da caricamento infinito) per permettere all'utente di scorrere tra i propri ricordi in modo fluido, naturale e senza interruzioni tecniche.
⚠️ Disclaimer & Scarico di Responsabilità

Prima di procedere con l'utilizzo di questo software, è necessario leggere e comprendere le seguenti condizioni:

    Software non firmato: Il binario non possiede una firma digitale certificata. Windows Defender o altri antivirus potrebbero identificarlo come potenziale minaccia; questo è un comportamento previsto per software non firmati in fase di sviluppo.

    Limitazione di Responsabilità: Lo sviluppatore non si assume alcuna responsabilità per danni diretti o indiretti al sistema, perdita di dati o instabilità hardware/software derivanti dall'uso di questo tool. L'utilizzo avviene a totale rischio dell'utente.

    Versione Beta: Il software è destinato esclusivamente a utenti esperti consapevoli dei rischi legati all'esecuzione di codice in fase di testing.

    Utilizzo: Il software è di tipo portable. Non richiede installazione: è sufficiente estrarre l'archivio (.zip) in una cartella ed eseguire il file.

🚀 Caratteristiche

    Progettato per la Velocità: Ottimizzato per gestire librerie da 300GB+ con tempi di risposta immediati.

    Rendering Intelligente: Utilizza Virtual Scrolling e Lazy Loading. Le immagini vengono renderizzate via GPU solo quando necessario, liberando risorse appena escono dallo schermo.

    Indexing Multi-Thread: Uno scanner asincrono parallelo analizza file e metadati EXIF senza bloccare l'interfaccia.

    Cache Dinamica: Miniature generate al volo e gestite tramite una cache LRU (Least Recently Used) per una navigazione fluida.

    Interfaccia Frameless: Design moderno con integrazione nativa delle API Windows per il trascinamento e i controlli di sistema.

🛠️ Stack Tecnologico & Sviluppo

Alice sfrutta un'architettura ibrida per unire stabilità e flessibilità:

    Backend: Python 3 (Logica di sistema e I/O).

    Database: SQLite3 con modalità WAL (Write-Ahead Logging).

    Frontend: Vanilla JavaScript, HTML5 e CSS3 (Zero framework per la massima leggerezza).

    Iconografia: Lucide Icons (utilizzate sotto licenza libera ISC).

    Debugging: Il processo di ottimizzazione e debugging è stato supportato dall'intelligenza artificiale Claude (Anthropic).

⚖️ Note Legali e Distribuzione

    No Profit: Alice non ha alcuno scopo di lucro e viene distribuito gratuitamente.

    Divieto di Vendita: È severamente vietata la commercializzazione o la vendita di questo software.

    Restrizioni alla Distribuzione: Il software non può essere condiviso o ripubblicato su altri portali senza autorizzazione. È destinato esclusivamente all'uso individuale.

🤝 Contribuire

Le Pull Request sono benvenute, specialmente se mirate a ottimizzare ulteriormente il caricamento. L'unica regola: il thread principale della UI deve rimanere sempre libero per garantire il Flusso.
