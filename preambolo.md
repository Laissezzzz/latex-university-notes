# Il preambolo condiviso

`template/preambolo.tex` contiene le configurazioni **originali**, da riutilizzare per ogni corso tramite `\input{preambolo.tex}` nel documento principale.

## Pacchetti

- `inputenc`, `fontenc`, `babel`: testo in italiano e codifica.
- `lmodern`, `microtype`: resa tipografica.
- `amsmath`, `amssymb`, `amsthm`, `mathtools`: matematica e ambienti numerati.
- `graphicx`, `float`: immagini e posizionamento.
- `tikz`, `pgfplots`: disegni e grafici matematici.
- `tcolorbox`: riquadri per note e approfondimenti.
- `geometry`, `enumitem`: impaginazione ed elenchi.
- `hyperref`: collegamenti navigabili.

## Comandi veloci

| Comando | Significato |
| --- | --- |
| `\N`, `\Z`, `\Q`, `\R`, `\C` | Insiemi numerici |
| `\abs{x}` | Valore assoluto di `x` |
| `\norm{v}` | Norma di `v` |
| `\finelezione` | Separatore di fine lezione |
| `\fineapprofondimento` | Separatore di fine approfondimento |

## Nota sulla numerazione

Definizioni, teoremi, esempi ed esercizi hanno contatori separati che si azzerano a ogni nuova `\section`. Questo corrisponde esattamente alle dichiarazioni presenti nel preambolo; non viene introdotta una numerazione comune.

## Modifiche future

Aggiungi nuovi comandi solo quando un insegnamento li richiede davvero. Prima di modificare il preambolo comune, verifica se la modifica è compatibile con i documenti esistenti.
