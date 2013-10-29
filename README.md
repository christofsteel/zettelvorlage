zettelvorlage
=============

Vorlage für Übungszettel

Um die Vorlage zu nutzen, muss die `options.tex.sample` zur `options.tex` umbenannt und angepasst werden.

Für jede Aufgabe muss eine `Aufgabe#.tex` angelegt werden (Also z.B. `Aufgabe1.tex`, `Aufgabe2.tex`, etc). 
Innerhalb dieser tex Dateien muss eine `antwort` Umgebung mit möglicher Punktzahl und Name der Aufgabe erstellt werden.
Falls die Aufgabe mehrere Unteraufgaben (`a)`, `b)`, `c)`...) gibt es eine `subantworten` Umgebung, die sich wie eine `enumerate`
Umgebung verhält.

Beispiel (`Antwort1.tex`):

```latex
\begin{antwort}[5]{Beispielaufgabe}
  Dies ist grob etwas zu der Aufgabe
  \begin{subantworten}
    \item Teil a) haben wir garnicht verstanden
    \item Teil b) war uns zu trivial
  \end{subantworten}
\end{antwort}
```

Für nicht nummerierte Zusatzaufgaben, muss eine Datei `Zusatz.tex` mit einer `zusatz` Umgebung, die sich wie eine 
`antwort` Umgebung verhält, angelegt werden.

Zusätzlich gibt es die Möglichkeit Quizfragen, zu beantworten. Dafür muss eine Datei `Quiz.tex` angelegt werden mit 
einer `quiz` Umgebung, die sich wie eine `enumerate` Umgebung verhält.

Zum kompilieren muss die `Vorlage.tex` kompiliert werden.
