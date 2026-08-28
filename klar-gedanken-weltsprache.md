# Klar — Gedanken zu einer Weltsprache

**Version:** 1.0 · **Stand:** 2026-08-06
*Buch 1 einer geplanten Reihe: (1) Warum, (2) Entwurf/Spezifikation, (3) Wörterbücher, (4) Experimente. Dieses Dokument erklärt die Beweggründe hinter den Regeln aus dem Entwurfsdokument — für Details siehe dort.*

## Änderungshistorie

| Version | Datum | Änderung |
|---|---|---|
| 1.0 | 2026-08-06 | Erste Fassung: Motivation, historische Einordnung, Designphilosophie, wissenschaftlicher Kontext (mit Gegenpositionen), offene Fragen zur Diskussion |

---

## 1. Warum überhaupt eine neue Plansprache?

Wer heute eine Plansprache entwirft, muss sich einer unbequemen Tatsache stellen: Es gibt bereits über 900 dokumentierte Versuche, eine bessere Sprache zu bauen (Okrent 2009). Fast alle sind gescheitert, gemessen an ihrem eigenen Anspruch — eine internationale Verkehrssprache zu werden. Esperanto ist nach fast 140 Jahren die einzige mit einer nennenswerten Sprechergemeinschaft und echten Muttersprachlern.

„Klar" tritt nicht mit dem Anspruch an, dieses Muster zu durchbrechen. Der Wert liegt woanders: in der **Methode**, mit der die Sprache entsteht, und in der Frage, ob sich damit etwas lernen lässt — über Sprache, über Spracherwerb, über die Grenzen dessen, was Design überhaupt leisten kann.

## 2. Was historisch versucht wurde — und woran es meist scheiterte

Drei grobe Wellen von Plansprachen lassen sich unterscheiden (Okrent 2009):

- **Philosophische Sprachen** (17. Jh., z. B. John Wilkins) wollten die Welt selbst logisch klassifizieren und die Sprache direkt daraus ableiten — beeindruckend als Gedankenexperiment, in der Praxis unbenutzbar komplex.
- **Schematische Auxlangs** (Volapük 1879, Esperanto 1887, Ido, Interlingua) wollten eine neutrale, leicht lernbare Verkehrssprache für den internationalen Austausch. Esperanto war darin am erfolgreichsten — aber sein Erfolg lässt sich nicht auf grammatische Überlegenheit zurückführen. Volapük hatte zeitweise mehr Anhänger und zerbrach nicht an der Sprache selbst, sondern an einem Streit um Reformautorität.
- **Logische Sprachen** (Loglan, später Lojban) wollten radikale Eindeutigkeit nach dem Vorbild formaler Logik erreichen — mit dem Ergebnis, dass sie sprachwissenschaftlich hoch interessant, aber für die allermeisten Menschen zu schwer erlernbar sind.

„Klar" versucht, aus allen drei Traditionen etwas mitzunehmen, ohne deren jeweilige Falle zu wiederholen: die Regelmäßigkeit der Auxlangs, die Eindeutigkeit der logischen Sprachen — aber begrenzt auf das, was ein Kind beiläufig lernen kann (siehe Entwurfsdokument, Prinzip 1–4).

## 3. Die eigentliche Designentscheidung: Methode statt Intuition

Die meisten historischen Plansprachen entstanden aus der Feder einer einzelnen Person, oft in relativ kurzer Zeit, und wurden erst danach an der Realität getestet (wenn überhaupt). „Klar" kehrt diese Reihenfolge bewusst um — jede Regel wurde gegen echte Beispielsätze geprüft, bevor sie als „fertig" galt (Entwurfsdokument, Abschnitt 1a), und ein automatisiertes Prüfskript verhindert, dass neue Wörter unbemerkt gegen die eigene Phonotaktik oder Kollisionsfreiheit verstoßen (Abschnitt 7.1).

Das ist kein Sprachdesign-Dogma, sondern schlicht die Übertragung einer Methode aus der Softwareentwicklung (iteratives Testen, automatisierte Regressionsprüfung) auf ein Gebiet, das traditionell eher intuitiv bearbeitet wurde. Ob das am Ende zu einer *besseren* Sprache führt, ist offen — sicher ist nur, dass es zu einer *nachvollziehbareren* führt: Jede Regel lässt sich auf einen konkreten Testfall zurückführen, nicht nur auf Geschmack.

## 4. Wissenschaftlicher Kontext — und die Gegenpositionen

Damit dieses Projekt nicht in reiner Spekulation verharrt, sind einige der Designentscheidungen an bestehende Forschung angelehnt. Wichtig ist dabei, auch die Kritik an diesen Theorien mitzuliefern — nichts davon ist unumstritten:

**Bioprogramm-Hypothese (Bickerton 1981, *Roots of Language*).** Kreolsprachen, die aus stark vereinfachtem Pidgin-Input entstehen, zeigen weltweit auffällig ähnliche Grammatikmerkmale (feste SVO-Stellung, präverbale Tempus-/Modus-Markierung). Bickertons These: Kinder füllen fehlende Struktur aus einem angeborenen „Bioprogramm" auf. „Klar" teilt einige dieser Merkmale (Entwurfsdokument, 1b) — nicht weil wir die Hypothese für bewiesen halten, sondern weil die Übereinstimmung zumindest ein Indiz ist. **Gegenposition:** Michel DeGraff hat diese Form des „Kreol-Exzeptionalismus" scharf kritisiert (DeGraff 1999, 2005) — seiner Ansicht nach unterscheiden sich Kreolsprachen grammatisch nicht grundsätzlich von anderen natürlich entstandenen Sprachen, und die vermeintliche Ähnlichkeit sei teils koloniale Ideologie statt neutraler Befund. Diese Debatte ist bis heute nicht entschieden.

**Frequency Code (Ohala 1983, 1984).** Hohe Stimmlage wird sprachübergreifend mit Kleinheit, Nicht-Bedrohlichkeit und Höflichkeit assoziiert, tiefe Stimmlage mit Dominanz — abgeleitet aus der Körpergrößen-Korrelation von Stimmtonhöhe bei vielen Tierarten. Darauf stützt sich die Intonationsregel in Abschnitt 5.7 des Entwurfs. Ohalas Modell ist einflussreich, aber auch hier gibt es Kritik an der empirischen Reichweite (z. B. Grawunder & Winter, die einige der postulierten Zusammenhänge in Frage stellen).

**Propädeutischer Effekt von Esperanto.** Mehrere unabhängige Studien (u. a. Szerdahelyi in Ungarn in den 1960ern; das *Springboard to Languages*-Projekt der University of Manchester, ca. 2005–2011) fanden Hinweise darauf, dass vorheriges Esperanto-Lernen den späteren Erwerb weiterer Fremdsprachen beschleunigt — vermutlich, weil die regelmäßige Grammatik früh ein Sprachbewusstsein (metalinguistic awareness) aufbaut. Falls das zutrifft, wäre das ein Argument dafür, dass eine *noch* regelmäßigere, gezielt kindgerechte Sprache wie „Klar" einen ähnlichen oder größeren Effekt haben könnte — bisher reine Spekulation, nicht getestet.

## 5. Offene Fragen zur Diskussion

Diese Punkte sind bewusst nicht entschieden — sie sollen zum Widerspruch und zum eigenen Experimentieren einladen, nicht zur stillen Zustimmung:

1. **Kann Design-Qualität überhaupt Verbreitung erzeugen?** Die historische Evidenz spricht dagegen (Esperanto vs. Netzwerkeffekte, siehe Entwurfsdokument Kapitel 8). Ist „eine bessere Sprache bauen" als Projektziel dann überhaupt sinnvoll — oder nur als Erkenntnisgewinn zu rechtfertigen, unabhängig von Verbreitung?
2. **Doppelte Verneinung als Redundanz oder als Altlast?** Kreolsprachen nutzen sie oft; „Klar" bisher nicht. Wäre das eine echte Fehlerrobustheits-Verbesserung oder nur eine unnötige Komplikation, die dem eigenen Minimalismus-Prinzip widerspricht (offener Punkt, Entwurfsdokument Kapitel 9)?
3. **Wie viel Kreol-Ähnlichkeit ist Zufall?** Angesichts der DeGraff-Kritik: Sind die strukturellen Parallelen zwischen „Klar" und Kreolsprachen ein Hinweis auf kindliche Lernpräferenzen — oder einfach das, was passiert, wenn *irgendjemand* radikal vereinfacht, unabhängig von Kognition?
4. **Rechtfertigt „Kanalrobustheit" (Flüstern, Aussprache-Einschränkungen) eine eigene Sprachnische?** Keine große Auxlang hat das bisher gezielt verfolgt. Ist das eine echte Lücke — oder ein Nischenproblem, für das sich der Aufwand einer ganzen Sprache nicht lohnt?
5. **Was würde es überhaupt heißen, wenn „Klar" „funktioniert"?** Esperanto misst Erfolg an Sprecherzahlen. Wenn Verbreitung explizit nicht das Ziel ist (siehe Punkt 1) — woran würde man den Erfolg dieses Experiments dann festmachen?

## 6. Einladung

„Klar" ist in seiner jetzigen Form ein Werkzeug zum Nachdenken über Sprache, nicht in erster Linie ein Kommunikationsmittel. Der Wert entsteht durch Ausprobieren — Sätze bilden, an denen die Grammatik reibt, Gedichte schreiben, an denen die Betonung stolpert, Wörter erfinden, die das Prüfskript zurückweist. Jeder gefundene Bruch ist interessanter als jede bestätigte Regel.

---

## Literatur

- Bickerton, Derek (1981). *Roots of Language*. Ann Arbor: Karoma Press.
- DeGraff, Michel (1999, 2005). Kritik am „Creole Exceptionalism" — u. a. in: *Language Creation and Language Change: Creolization, Diachrony, and Development* (Hg. DeGraff), MIT Press.
- Ohala, John J. (1983). Cross-language use of pitch: An ethological view. *Phonetica* 40, 1–18.
- Ohala, John J. (1984). An ethological perspective on common cross-language utilization of F0 of voice. *Phonetica* 41, 1–16.
- Okrent, Arika (2009). *In the Land of Invented Languages*. New York: Spiegel & Grau.
- Roehr-Brackin, K. / Tellier, A. u. a. Auswertungen des *Springboard to Languages*-Projekts, University of Manchester (ca. 2005–2012).
- Szerdahelyi, István (1960er). Ungarische Vergleichsstudie zum propädeutischen Effekt von Esperanto, Universität Budapest.

*Hinweis: Diese Angaben stammen aus Recherche im Rahmen dieses Gesprächs und sollten vor einer tatsächlichen Veröffentlichung gegen die Originalquellen geprüft werden (genaue Seitenzahlen, ggf. weitere Auflagen).*
