# La Bibbia del Branding

Sito interno del team branding Lemonade Partytrip.

## Messa online
1. Carica tutti i file di questa cartella nella radice del repo.
2. Settings -> Pages -> Source: "Deploy from a branch", branch `main`, cartella `/ (root)`. Salva.
3. Dopo un minuto il sito e' online su https://nicologiacometti.github.io/La-Bibbia-del-Branding/

## Come si gestisce
- Icona ingranaggio in alto a destra -> password + token GitHub (fine-grained, Contents: read and write, senza scadenza).
- Da li' si aggiungono mete, locali, piani con planimetria, punti di montaggio e materiali.
- Il pulsante SALVA scrive su `data.json` in questo repo. Online per tutti dopo circa un minuto.

## File
- `index.html` - il sito (unico file, tutto incluso). Per aggiornare la grafica si sostituisce solo questo.
- `data.json` - i dati. Non sostituirlo mai a mano dopo la prima volta.
- `planimetrie/`, `foto/` - immagini caricate dal pannello.

## Aggiungere alla home dell'iPhone
Safari -> Condividi -> "Aggiungi a Home". L'icona apre il sito a schermo pieno, senza barre del browser.
Serve che siano nel repo anche `manifest.webmanifest`, `icon-180.png` e `icon-512.png`.
