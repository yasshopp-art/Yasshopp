# yasshop12 – sito catalogo

Sito statico pubblicato su Cloudflare Workers (progetto `polished-waterfall-bb9e`), che si aggiorna da solo a ogni push su `main`.

- `public/index.html` – tutto il sito (HTML, CSS e JS in un file)
- `public/products.js` – elenco prodotti (`window.PRODUCTS`), oltre 700 voci: campi n, b, g, t, d, imgs
- `public/images/` – foto dei prodotti
- `wrangler.jsonc` – configurazione Cloudflare, non rinominare il progetto

Regole:
- Non modificare `public/products.js` né `public/images/` durante i lavori di grafica.
- Per restyling lavora su un ramo separato, non su `main`: `main` è il sito online.
- Il proprietario lavora da iPad e parla italiano: spiegazioni semplici, in italiano.
- Funzioni da mantenere: categorie, ricerca, filtri Marca/Genere, galleria foto scorrevole con frecce e miniature, foto intere (object-fit: contain), pulsante "Richiedi taglia e disponibilità" con messaggio per Instagram, logo cromato, scritta CATALOGO animata con contorno luminoso.
- Strumenti di design: skill `ui-ux-pro-max` in `.claude/skills/` e MCP server 21st.dev Magic in `.mcp.json` (la chiave è un network secret dell'ambiente cloud).
