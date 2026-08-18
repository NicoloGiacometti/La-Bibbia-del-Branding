# La Bibbia del Branding

Sito interno del team branding Lemonade Partytrip: dove e come montare banner, vele e tondi nei locali di ogni meta.

## Cosa fa

**Parte pubblica (sola lettura)**
- Elenco delle mete, con ricerca per meta o locale.
- Per ogni meta la lista dei locali, con numero di piani e di punti di montaggio.
- Per ogni locale: indirizzo, materiale da portare, planimetria per ogni piano, punti numerati cliccabili sulla piantina e note logistiche.
- Toccando un punto si apre la scheda: tipo e quantità di materiale, priorità, come si fissa, note di montaggio e foto di riferimento.

**Area gestione (password + token GitHub)**
- Aggiunta e modifica di mete, locali, piani, materiali e punti.
- Caricamento delle planimetrie e delle foto dei punti direttamente dal telefono.
- I punti si posizionano toccando la piantina nel punto esatto.
- Il pulsante SALVA scrive nel repo: online per tutti dopo circa un minuto.
- I salvataggi vengono **fusi**, non sovrascritti: se più persone lavorano su mete diverse nello stesso momento, nessuno perde il proprio lavoro.

**Da telefono**
- Interfaccia pensata per l'uso in piedi in un locale, a una mano.
- Si aggiunge alla home dell'iPhone e si apre a schermo pieno come un'app (Safari → Condividi → Aggiungi a Home).
- Tira giù dall'alto per aggiornare i dati, scorri verso destra per tornare indietro.

## Messa online
1. Carica il contenuto di questa cartella nella radice del repo.
2. Settings → Pages → Source "Deploy from a branch", branch `main`, cartella `/ (root)`.
3. Il sito è su https://nicologiacometti.github.io/La-Bibbia-del-Branding/

## Accesso alla gestione
Servono **entrambi**: la password del team e un token GitHub *fine-grained* con permesso `Contents: Read and write` su questo repo, senza scadenza. Il token si incolla una volta e resta salvato sul dispositivo. Quando cambia il responsabile branding, si revoca il token e se ne genera uno nuovo.

## File
- `index.html` — il sito, unico file con tutto incluso. Per aggiornare grafica o funzioni si sostituisce solo questo.
- `data.json` — tutti i dati. Non sostituirlo mai a mano: lo gestisce il pannello.
- `planimetrie/`, `foto/` — immagini caricate dall'area gestione.
- `manifest.webmanifest`, `icon-180.png`, `icon-512.png` — icona e modalità app su iPhone.
- `.nojekyll` — necessario a GitHub Pages per servire i file così come sono.
