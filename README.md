# Nutri / Cycle

Single Page Application statica, senza dipendenze o build step.

## Pubblicazione su GitHub Pages

1. Carica **il contenuto di questa cartella** nella root di un repository GitHub.
2. In GitHub apri **Settings → Pages**.
3. Seleziona la branch `main` e la cartella `/(root)`, quindi salva.

`index.html` carica i dati da `public/config.json` e `public/recipes.json`; mantieni quindi la struttura delle cartelle invariata. Le ricette aggiunte e lo storico dei pasti rimangono esclusivamente nel `localStorage` del browser dell'utente.

Per provarla localmente, avvia un piccolo server dalla cartella del progetto (ad esempio `python -m http.server`) e apri l'indirizzo restituito: il `fetch` dei file JSON richiede un server HTTP, non l'apertura diretta del file HTML.
