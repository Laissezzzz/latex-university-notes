# LaTeX University Notes

Un riferimento personale per scrivere appunti universitari in LaTeX mantenendo **lo stesso preambolo** e una struttura coerente tra diversi corsi (Analisi, Statistica, Probabilità, Matematica finanziaria, ecc.).

## Come iniziare

1. Copia i due file da [`template/`](template/) in una nuova cartella dedicata al corso.
2. Apri `main.tex` in VS Code con LaTeX Workshop (o in un altro editor LaTeX).
3. Compila `main.tex` con **pdfLaTeX**. I pacchetti richiesti sono quelli elencati nel preambolo, inclusi TikZ, PGFPlots e tcolorbox.
4. Sostituisci gli esempi dimostrativi con i contenuti della tua lezione.
5. Non modificare `preambolo.tex` se non è necessario: serve a mantenere uniformità tra corsi.

## Struttura dei contenuti

| Ambiente | Quando utilizzarlo |
| --- | --- |
| `definizione` | Per definire formalmente un oggetto o un concetto |
| `teorema` | Per enunciare un risultato matematico |
| `esempio` | Per illustrare una definizione o un risultato |
| `esercizio` | Per un problema, con eventuale soluzione |
| `approfondimento` | Per integrare materiale personale, distinto dalla lezione |

Sono inoltre disponibili `proposizione`, `lemma`, `corollario` e `nota`.

**Regola editoriale:** riportare fedelmente quanto presente negli appunti della lezione. Non introdurre spiegazioni, enunciati o formule extra senza una scelta esplicita; eventuali aggiunte personali vanno nell'ambiente `approfondimento`.

## Documentazione

- [Guida agli ambienti e alle regole di utilizzo](guida/ambienti.md)
- [Comandi e struttura del preambolo](guida/preambolo.md)
- [Compilazione e riuso per un nuovo corso](guida/nuovo-corso.md)
- [Esempi LaTeX](esempi/esempi-ambienti.tex)

## Comandi di separazione

- `\finelezione` chiude visivamente gli appunti di una lezione.
- `\fineapprofondimento` chiude visivamente un approfondimento personale.

## Licenza

Il progetto è predisposto per uso personale. Aggiungi una licenza se decidi di distribuirlo pubblicamente con permessi espliciti di riutilizzo.
