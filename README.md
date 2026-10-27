# Franco

Piattaforma web peer-to-peer per il noleggio di attrezzi tra privati: chi ha un attrezzo lo mette a disposizione, chi ne ha bisogno lo trova sulla mappa e lo noleggia.

> Progetto in sviluppo. Nasce da un prototipo no-code (Base44), poi migrato su uno stack React.

🌐 Demo: [franco-web.vercel.app](https://franco-web.vercel.app)

## Stack

- React + Vite
- Supabase (database, autenticazione, storage)
- Leaflet (mappa e geolocalizzazione degli attrezzi)

## Requisiti

- Node.js 18 o superiore
- Un progetto Supabase (gratuito) con URL e chiave anon

## Installazione

Il codice dell'applicazione si trova nella cartella `web/`.

```bash
git clone https://github.com/urbvni/franco-web.git
cd franco-web/web
npm install
```

## Configurazione

Dentro `web/`, copia il file di esempio e inserisci le tue credenziali Supabase:

```bash
cp .env.example .env
```

```env
VITE_SUPABASE_URL=la-tua-url-supabase
VITE_SUPABASE_ANON_KEY=la-tua-chiave-anon
```

Non committare mai il file `.env` e non usare mai la chiave `service_role` nel frontend.

## Avvio

```bash
npm run dev
```

L'app sarà disponibile su `http://localhost:5173`.

## Build di produzione

```bash
npm run build
npm run preview
```

## Documentazione

- Stack Deployment Blueprint (v1.1)
- Documento di handover operativo

## Licenza

MIT (da confermare)

## Autore

Matteo Urbani (Frango): [github.com/urbvni](https://github.com/urbvni)
