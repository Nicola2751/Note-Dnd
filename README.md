# Cronache del Mondo — Wiki D&D

Sito statico realizzato con [Astro](https://astro.build/) e pubblicabile tramite GitHub Pages.

## Sviluppo locale

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
npm run preview
```

## Pubblicazione su GitHub Pages

1. Aprire **Settings → Pages** nel repository.
2. In **Build and deployment**, scegliere **GitHub Actions** come source.
3. Il workflow `.github/workflows/deploy.yml` esegue build e deploy a ogni push su `main`.

URL previsto: https://nicola2751.github.io/Note-Dnd/

## Area Master — sicurezza

Il repository attuale è pubblico. **Non salvare mai qui password, appunti segreti, rivelazioni o materiale riservato.** Escludere una cartella dal sito Astro non la rende privata: i file resterebbero leggibili nella cronologia GitHub.

L'area Master è pianificata come applicazione separata protetta da autenticazione lato server (ad esempio Cloudflare Access con un'origine privata). Per attivarla serviranno configurazione del provider, dominio/URL e credenziali gestite come secrets. Una pagina con password JavaScript o una semplice route nascosta non costituisce protezione.

Fino all'attivazione dell'autenticazione, il sito contiene esclusivamente informazioni destinate ai giocatori.
