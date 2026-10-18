# Immagine in STL

App in italiano per convertire fotografie e disegni in rilievi 3D esportabili in STL. Le immagini vengono elaborate localmente, senza upload.

## App online

Apri https://cercote78.github.io/image-to-stl/ con una connessione Internet.

## App desktop Windows

Scarica l’installer `.exe` dalla pagina [Releases](https://github.com/cercote78/image-to-stl/releases), eseguilo e avvia **Immagine in STL** dal menu Start o dal collegamento sul desktop. Il pacchetto include l’app e le dipendenze 3D: dopo l’installazione la conversione funziona anche offline.

## Uso

1. Seleziona o trascina un PNG, JPG o WEBP. Il file resta sul dispositivo.
2. Imposta larghezza (10–250 mm), base, altezza del rilievo e dettaglio.
3. Trascina l’anteprima 3D per ruotarla; usa la rotella per lo zoom. “Inverti rilievo” scambia chiaro e scuro.
4. Scarica lo STL binario e importalo nel tuo slicer.

La mesh include superficie, fondo e pareti laterali; le proporzioni originali sono mantenute. Lo STL non conserva il colore. Verifica scala e orientamento nel tuo slicer prima di stampare.

## Build desktop da sorgente

Richiede Node.js 22 o successivo e npm. Esegui `npm install`, poi `npm run dev` per lo sviluppo o `npm run dist:win` per creare l’installer Windows x64 in `release/`. Il workflow GitHub Actions compila e allega automaticamente l’installer a una Release per ogni tag `v*`.