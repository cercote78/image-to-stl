# Immagine in STL

App web in italiano per convertire fotografie e disegni in rilievi 3D esportabili in STL.

## Avvio

Apri `index.html` con un browser moderno e una connessione Internet. Per i moduli JavaScript è consigliato un server statico (GitHub Pages oppure `python -m http.server 8000`) invece di `file://`.

## Uso

1. Seleziona o trascina un PNG, JPG o WEBP. L’immagine viene elaborata localmente nel browser: non viene caricata online.
2. Imposta larghezza (10–250 mm), spessore base, altezza del rilievo e dettaglio.
3. Ruota l’anteprima 3D trascinando; usa la rotella per lo zoom. Attiva “Inverti rilievo” per scambiare chiaro e scuro.
4. Scarica lo STL binario e importalo nel tuo slicer.

La mesh include superficie superiore, fondo e pareti laterali. La luminosità dell’immagine controlla l’altezza; le proporzioni originali sono mantenute. Il dettaglio massimo è 180 punti sul lato maggiore. Lo STL non conserva il colore. Verifica scala, orientamento e supporti nello slicer prima di stampare. Three.js e l’esportatore STL sono caricati da jsDelivr; la conversione dell’immagine avviene sul dispositivo.