# Platzhalter

## Tutorial

<!--
Um ein Zitat in den Text aufzunehmen, füge einfach den in der references.bib-Datei gezeigten Zitatschlüssel hinzu.
-->

Aufnahme mit "[@Referenz]"

kursiv: * auf beiden Seiten des Textes -> *kursiv*
fett: ** -> **fett**
kursiv und fett: *** --> ***fett und kursiv***


Aenean nec dapibus in mL/min^-1^. Mathematical formula can be inserted using Latex:

(@ref_for_eqn1) $f(x) = ax^3 + bx^2 + cx + d$


<!-- Eine ungeordnete Liste -->

- erstes Element der Liste
- zweites Element der Liste
- drittes Element der Liste

<!-- eine geordnete Liste -->
1. erstes Element
2. zweites Element
3. drittes Element


Syntaxhervorhebung in Codeblöcken erreicht man mit drei "`" Zeichen vor und nach dem Codeblock.

```python
mood = 'happy'
if mood == 'happy':
    print("I am a happy robot")
```

<!--
Bilder können mit der folgenden Syntax eingefügt werden:
![Bildunterschrift \label{mein_label}](source/figures/beispielbild.jpg){ width=50% }

Details zu den Attributen wie width und height gibt es unter:
http://pandoc.org/MANUAL.html#extension-link_attributes
-->

Die Tabelle \ref{tabellenreferenz} zeigt uns wie man eine Tabelle hinzufügt. Integer tincidunt sed nisl eget pellentesque. Mauris eleifend, nisl non lobortis fringilla, sapien eros aliquet orci, vitae pretium massa neque eu turpis. Pellentesque tincidunt aliquet volutpat. Ut ornare dui id ex sodales laoreet.

<!-- Erzwingt eine neue Seite -->

\newpage

---------------------------------------------------------------------------
Spalte 1            Spalte 2                Spalte 3
--------------      -------------------     -------------------
Zeile 1               0.1                     0.2

Zeile 2               0.3                     0.3

Zeile 3               0.4                     0.4      

Zeile 4               0.5                     0.6

---------------------------------------------------------------------------

Table: Das ist die Tabellenbeschriftung. Suspendisse blandit dolor sed tellus venenatis, venenatis fringilla turpis pretium. \label{tabellenreferenz}

