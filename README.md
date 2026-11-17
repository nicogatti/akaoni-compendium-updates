# Akaoni D&D Compendium — Aggiornamenti

Canale pubblico di distribuzione dell'interfaccia di Akaoni D&D Compendium.

Il codice sorgente dell'app macOS rimane nel repository privato `nicogatti/akaoni-dnd-compendium`.

## Stato
Canale inizializzato. **Nessun aggiornamento installabile è ancora pubblicato.**

## Protocollo supportato dall'app v0.3.1
L'app legge un manifest JSON via HTTPS con tre campi:
- `version`: versione dell'interfaccia
- `url`: URL HTTPS del file `index.html`
- `sha256`: digest SHA-256 esadecimale del file HTML

Il manifest e il file HTML devono essere serviti dallo **stesso host**. Un manifest non deve essere pubblicato prima che il file HTML corrispondente sia disponibile e verificato.

## Sicurezza
Non pubblicare personaggi, salvataggi, credenziali o contenuti protetti da copyright. L'app attuale verifica SHA-256 ma non la firma crittografica del manifest; la verifica dell'autenticità della pubblicazione va migliorata in una versione futura.
