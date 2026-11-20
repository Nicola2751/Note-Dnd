# Area Master — piano tecnico

## Requisito
Area separata dalla wiki pubblica con autenticazione reale, non una password verificata nel browser.

## Vincolo attuale
Il repository `Nicola2751/Note-Dnd` è pubblico. Qualunque file committato qui è leggibile da chiunque, anche se escluso dalla build. Non inserire contenuti master in questo repository.

## Architettura da completare
- Wiki pubblica: Astro + GitHub Pages.
- Area Master: applicazione/hosting protetto da un identity-aware proxy (ad esempio Cloudflare Access) o backend con autenticazione.
- Contenuti master: archivio privato non versionato nel repository pubblico, oppure repository privato separato.
- Segreti e token: solo variabili d'ambiente/secret store del provider, mai nel codice client.

## Attivazione
Richiede scelta e configurazione del provider, dominio o URL protetto, policy di accesso (email/account autorizzati) e origine privata per i contenuti. GitHub Pages da solo non protegge una singola sezione con password.
