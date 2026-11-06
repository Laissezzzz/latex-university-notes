# LaTeX University Notes

Un riferimento personale per studiare e scrivere appunti universitari in LaTeX mantenendo **lo stesso preambolo** e una struttura coerente tra diversi corsi: Analisi, Statistica, Probabilità, Matematica finanziaria e altri.

## Metodo di studio

Il file LaTeX è il risultato finale dello studio personale: raccoglie tutte le spiegazioni e gli esercizi nella forma che considero completa, chiara e adatta al mio modo di studiare.

Una materia di studio personale è considerata **chiusa quando ho completato il file LaTeX con tutte le spiegazioni e gli esercizi come piacciono a me**.

In particolare:

- tutti gli argomenti previsti per quella materia sono presenti;
- le spiegazioni contengono i passaggi necessari alla comprensione;
- gli esercizi previsti sono inclusi, con svolgimenti e soluzioni;
- notazione, struttura, grafici e impaginazione rispettano le mie preferenze;
- non rimangono parti previste da completare o dubbi da chiarire nel testo.

Aver letto una lezione, compreso una spiegazione o svolto alcuni esercizi costituisce un avanzamento, ma non basta a considerare chiusa la materia.

### Completamento degli appunti e preparazione all’esame

Si tengono distinti due aspetti:

| Aspetto | Cosa indica |
| --- | --- |
| **Completamento del file LaTeX** | Quanto manca per chiudere il lavoro di studio personale |
| **Preparazione all’esame** | Capacità di spiegare i concetti e risolvere autonomamente gli esercizi |

Il completamento del file non certifica automaticamente la preparazione all’esame. Allo stesso modo, aver sostenuto un esame non rende automaticamente completo il file.

### Procedura di lavoro

1. Ripassare la lezione seguendo l’ordine e la notazione del professore.
2. Chiarire i passaggi necessari alla comprensione.
3. Trascrivere e correggere il contenuto in LaTeX.
4. Affrontare gli esercizi uno alla volta, correggendoli prima di proseguire.
5. Inserire nel file gli svolgimenti e le soluzioni degli esercizi completati.
6. Verificare che tutti i contenuti previsti siano completi prima di considerare chiusa la materia.

## Come iniziare

1. Copia i due file da [`template/`](https://github.com/Laissezzzz/latex-university-notes/tree/main/template) in una nuova cartella dedicata al corso.
2. Apri `main.tex` in VS Code con LaTeX Workshop o in un altro editor LaTeX.
3. Compila `main.tex` con **pdfLaTeX**. I pacchetti richiesti sono quelli elencati nel preambolo, inclusi TikZ, PGFPlots e tcolorbox.
4. Sostituisci gli esempi dimostrativi con i contenuti delle lezioni.
5. Non modificare `preambolo.tex` se non è necessario: serve a mantenere uniformità tra corsi.

## Struttura delle lezioni

La gerarchia dei contenuti segue queste regole:

| Comando o ambiente | Utilizzo |
| --- | --- |
| `\section{Lezione del ...}` | Una sezione per ogni lezione, con la data nel titolo |
| `\subsection{...}` | Una sottosezione per ogni argomento o esempio della lezione |
| `\finelezione` | Chiusura visiva degli appunti della lezione |
| `approfondimento_personale` | Materiale personale concordato, distinto dal contenuto della lezione |

Ogni argomento o esempio ha quindi una propria `\subsection`. Al suo interno si utilizzano gli ambienti appropriati, come `definizione`, `teorema`, `esempio` ed `esercizio`.

### Separazione delle pagine

- Ogni lezione inizia con `\newpage`.
- Ogni nuovo tema inizia con `\newpage`.
- Ogni nuova sezione di esercizi inizia con `\newpage`.

### Esempio di struttura

```latex
\newpage
\section{Lezione del 10 novembre 2026}

\subsection{Titolo del primo argomento}

\begin{definizione}
Definizione riportata nella lezione.
\end{definizione}

\subsection{Esempio}

\begin{esempio}
Testo dell’esempio e relativo svolgimento.
\end{esempio}

\newpage
\subsection{Titolo del nuovo tema}

\begin{teorema}
Enunciato riportato nella lezione.
\end{teorema}

\newpage
\subsection{Esercizi}

\begin{esercizio}
Testo dell’esercizio.

\medskip
\noindent\textbf{Soluzione.}
Svolgimento completo e risultato.
\end{esercizio}

\finelezione

\begin{approfondimento_personale}
Spiegazioni o esercizi personali concordati.
\end{approfondimento_personale}
```

I comandi e gli ambienti dell’esempio devono essere definiti nel preambolo condiviso.

## Ambienti per i contenuti

| Ambiente | Quando utilizzarlo |
| --- | --- |
| `definizione` | Per definire formalmente un oggetto o un concetto |
| `teorema` | Per enunciare un risultato matematico |
| `proposizione` | Per enunciare una proposizione |
| `lemma` | Per un risultato di supporto |
| `corollario` | Per una conseguenza di un risultato precedente |
| `esempio` | Per illustrare una definizione o un risultato |
| `esercizio` | Per un problema, con svolgimento e soluzione quando completato |
| `nota` | Per un’osservazione relativa al contenuto |
| `approfondimento_personale` | Per integrare materiale personale concordato, distinto dalla lezione |

Per gli approfondimenti personali si usa esattamente:

```latex
\begin{approfondimento_personale}
Contenuto dell’approfondimento.
\end{approfondimento_personale}
```

## Regole editoriali

### Fedeltà alla lezione

Riportare fedelmente quanto presente negli appunti, nelle slide o nelle spiegazioni del professore, rispettandone ordine e notazione.

Non introdurre spiegazioni, enunciati, formule, generalizzazioni o esercizi extra senza una scelta esplicita. Non ampliare automaticamente un risultato oltre la forma trattata dal professore.

Le aggiunte personali concordate vanno nell’ambiente `approfondimento_personale`, in modo che rimangano riconoscibili rispetto al materiale della lezione.

### Spiegazioni ed esercizi

- Esplicitare i passaggi necessari alla comprensione, concordando le integrazioni al materiale originale.
- Presentare gli esercizi guidati uno alla volta, con correzione prima del successivo.
- Inserire nel file finale gli svolgimenti e le soluzioni nella forma desiderata.
- Conservare la notazione del corso e usare LaTeX per formule ed espressioni matematiche.

### Grafici e disegni

Riprodurre in LaTeX/TikZ, quando possibile, i grafici e i diagrammi presenti negli appunti. Concordare gli eventuali disegni aggiuntivi utili alla comprensione.

## Documentazione

- [Guida agli ambienti e alle regole di utilizzo](https://github.com/Laissezzzz/latex-university-notes/blob/main/guida/ambienti.md)
- [Comandi e struttura del preambolo](https://github.com/Laissezzzz/latex-university-notes/blob/main/guida/preambolo.md)
- [Compilazione e riuso per un nuovo corso](https://github.com/Laissezzzz/latex-university-notes/blob/main/guida/nuovo-corso.md)
- [Esempi LaTeX](https://github.com/Laissezzzz/latex-university-notes/blob/main/esempi/esempi-ambienti.tex)

## Licenza

Il progetto è predisposto per uso personale. Aggiungi una licenza se decidi di distribuirlo pubblicamente con permessi espliciti di riutilizzo.
