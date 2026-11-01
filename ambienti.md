# Guida agli ambienti

Tutti gli ambienti sotto sono definiti in `template/preambolo.tex`. Gli ambienti di tipo teorema sono numerati **per sezione**; ciascuna tipologia possiede il proprio contatore (ad esempio: Definizione 1.1, Teorema 1.1).

## Definizione

Usa `definizione` per l'enunciato preciso di un termine o oggetto matematico.

```latex
\begin{definizione}[Media campionaria]
Siano $x_1,\ldots,x_n$ dati reali. Si definisce
\[
\overline{x}=\frac{1}{n}\sum_{i=1}^{n}x_i.
\]
\end{definizione}
```

## Teorema

Usa `teorema` per un risultato che deve essere enunciato come tale. Se hai una dimostrazione, puoi scriverla subito dopo con l'ambiente standard `proof`, fornito da `amsthm`.

```latex
\begin{teorema}
Se $X_1,\ldots,X_n$ hanno lo stesso valore atteso $\mu$,
allora $\mathbb{E}[\overline{X}]=\mu$.
\end{teorema}

\begin{proof}
Per linearità del valore atteso, ...
\end{proof}
```

## Esempio

Usa `esempio` quando si mostra come funziona un concetto già introdotto.

```latex
\begin{esempio}
La media dei dati $2,4,6$ è $4$.
\end{esempio}
```

## Esercizio

Usa `esercizio` per una consegna da risolvere. Puoi inserire di seguito i passaggi risolutivi quando sono parte degli appunti.

```latex
\begin{esercizio}
Calcolare la media dei dati $1,3,5,7$.
\end{esercizio}
```

## Approfondimento personale

Usa `approfondimento` **solo per materiale integrativo personale**: il riquadro grigio lo distingue dal contenuto originario della lezione.

```latex
\begin{approfondimento}
Qui inserisco una spiegazione aggiuntiva.
\end{approfondimento}
\fineapprofondimento
```

L'ambiente accetta anche opzioni di `tcolorbox`, per esempio `\begin{approfondimento}[title={Approfondimento: media}]`.

## Altri ambienti disponibili

- `proposizione`, `lemma` e `corollario`: risultati matematici classificati come tali nel materiale.
- `nota`: riquadro azzurro per mettere in evidenza un'osservazione.

## Fine della lezione

Al termine di una lezione scrivi `\finelezione`. Non è un ambiente e non richiede `\begin`/`\end`.

## Regola essenziale

**Non trasformare arbitrariamente un esempio in un esercizio, o un risultato in un teorema.** Segui la classificazione del docente; gli approfondimenti personali restano separati.
