# Creare gli appunti di un nuovo corso

1. Crea una cartella per il corso (es. `statistica-avanzata/`).
2. Copia `template/main.tex` e `template/preambolo.tex` nella stessa cartella.
3. Modifica titolo, autore e data in `main.tex`.
4. Inserisci una nuova `\section{...}` per il capitolo o la struttura effettiva del corso.
5. Usa gli ambienti documentati in [ambienti.md](ambienti.md): definizione, teorema, esempio, esercizio e approfondimento.
6. Inserisci `\finelezione` al termine della lezione.
7. Compila `main.tex` con pdfLaTeX (due compilazioni se vuoi aggiornare correttamente l'indice).

> `preambolo.tex` contiene dichiarazioni `\usepackage` e deve essere richiamato **prima** di `\begin{document}`.

Il template è intenzionalmente indipendente da qualunque materia: si può usare per Statistica senza cambiare gli ambienti già definiti.
