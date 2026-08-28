# Kunstsprache-Entwurf (Arbeitstitel: „Klar")

**Version:** 2.3 · **Stand:** 2026-08-06

## Änderungshistorie

| Version | Datum | Änderung |
|---|---|---|
| 2.3 | 2026-08-06 | Reorganisation nach Einführung von Buch 1 „Gedanken zu einer Weltsprache": Kapitel 1/1a/1b und Kapitel 8 gestrafft — ausführliche Begründungen, historischer Kontext (Bickerton/DeGraff) und die „lohnt sich Verbreitung"-Diskussion wandern per Verweis zu Buch 1, hier bleiben nur die Regeln und die für die Spezifikation direkt relevanten Befunde |
| 2.2 | 2026-08-06 | Onomatopoesie als neuer Abschnitt 6.4a (8 lautmalerische Wurzeln, geprüft). Eigenständige Kurzantwort „nein" auf `nono` (Reduplikation) geändert — zusätzliche Silbenzahl-Unterscheidung von „ja" (`pa`), da Dauer/Timing eine der robustesten akustischen Eigenschaften überhaupt ist (7.1); klauselinterne Verneinung bleibt `no` |
| 2.1 | 2026-08-06 | Wurzel „pom" (Apfel) offiziell im Kernwortschatz nachgetragen — wurde seit Version 1.0 durchgängig in Beispielsätzen benutzt, war aber nie formal aufgenommen. Neues Begleitdokument „Klar-Englisch-Wörterbuch" mit ~94 alltäglichen Wurzeln erstellt (mit Prüfskript validiert) |
| 2.0 | 2026-08-06 | Prüfskript für neue Wurzeln entwickelt (Phonotaktik, Kollisionen, Stimmhaftigkeits-/r-l-Minimalpaare) — deckte sofort weitere Fehler auf: **„h" war nie im 13-Konsonanten-Inventar enthalten**, aber in `ho`(und), `ha`(ja), `hunda`(100) verwendet — korrigiert zu `ko`, `pa`, `sena`. Ziffern 3/4/6/9 enthielten Cluster bzw. den unerlaubten Laut „v" — `tri`→`fin`, `kwar`→`fer`, `seks`→`sik`, `nov`→`nom`. Alle Stellen systemweit aktualisiert |
| 1.9 | 2026-08-06 | Abschnittsnummerierung in Kapitel 5 korrigiert (5.3–5.8 waren durch frühere Einfügungen nicht mehr in Lesereihenfolge) — alle internen Verweise entsprechend aktualisiert |
| 1.8 | 2026-08-06 | Neues Prinzip 6 „Kanalrobustheit" (Flüstern, körperliche Einschränkungen) plus Abschnitt 7.1: zwei Stimmhaftigkeits-Minimalpaare gefunden und korrigiert (`da`→`ma" Zeit, `dek`→`lek` zehn); r→l als sanktionierte Ausweichform für eingeschränkte Aussprache dokumentiert (kollisionsfrei geprüft); Intonations-Design rückwirkend bestätigt. Dedizierter Abschnitt „Verneinung — Übersicht" fasst alle bisherigen Verwendungen von `no` erstmals an einer Stelle zusammen |
| 1.7 | 2026-08-06 | **Fehler behoben:** Wurzeln „ven", „vid", „vol", „var" enthielten den Konsonanten „v", der nicht im 13-Konsonanten-Inventar (Abschnitt 2) enthalten ist — umbenannt zu „ben" (kommen), „fid" (sehen), „bol" (wollen), „war" (warm), systemweit korrigiert. Ja/Nein als Antwortpartikel ergänzt (5.4): „nein"=`no` (Wiederverwendung), „ja"=`ha` (maximaler Lautabstand zu „no", da höchste Fehlerquote im System) |
| 1.6 | 2026-08-06 | Serialverbkonstruktionen getestet (5.3): Mitnahme-Fall eindeutig als informelle Kurzform, Zweck-Fall braucht neuen Verknüpfer „po" (um...zu) für Eindeutigkeit — folgt dem Sprech-/Schreib-Muster aus 5.6. Neue Wurzel „tek" (nehmen) |
| 1.5 | 2026-08-06 | Testkorpus v3: zusammenhängender Dialog (6.8) — bestätigt W-Fragen in situ (`kel`-Stamm) ohne neue Grammatik. Featurales Alternativ-Alphabet als konkreter Entwurf ausgearbeitet (3.2: Grundform nach Artikulationsort + Manier-Markierung, Vokale bilden das IPA-Vokaltrapez ab). Neuer Abschnitt 1b: Abgleich mit Kreolsprachen bestätigt TAM-Slot-Prinzip und (K)V-Phonotaktik unabhängig; liefert zwei neue offene Punkte (Serialverbkonstruktionen, doppelte Verneinung als Redundanz). Neue Wurzeln „kel" (Interrogativstamm), „poi" (später) |
| 1.4 | 2026-08-06 | Interjektionsfrage aus 6.7 gelöst: formelhafte Äußerungen (Gruß, Dank, Wunsch) sind Ellipsen vollständiger Sätze, kein Verstoß gegen Prinzip 1 (5.1a erweitert). Eigennamen/Bezeichnungen von allgemeiner Neuwortbildung getrennt: Aussprache bleibt erhalten, nur Transliteration (6.3). Ausspracheentwurf mit IPA und englischen Beispielen ergänzt (3.1). Neue Wurzeln „wud" (wünschen), „din" (Tag) |
| 1.3 | 2026-08-06 | Testkorpus v2 mit 15 alltagsnahen Sätzen (6.7: Begrüßung, Bitte, Besitz, Vergleich, Gefühl, Small Talk, Imperativ ...). Neu entdeckt und ergänzt: Imperativ-Partikel „we" (TAM-Slot), kopula-lose Prädikation, Possessiv über Adjektiv-Endung, Komparativ-Konstruktion, Wort-Konjunktion mit „ho" (alles in 5.8). Wurzel „rest"→„res" korrigiert (Cluster-Verstoß). Kernwortschatz um 11 Wurzeln erweitert. Offene Frage zu Interjektionen vs. Prinzip 1 vermerkt |
| 1.2 | 2026-08-06 | Prioritätsregel geklärt: Alltagstauglichkeit hat Vorrang vor formaler/IT-Eleganz; Kompositionalität (Prinzip 3) als Prüfwerkzeug statt Designziel umformuliert; BNF-Grammatik im Ausblick entsprechend eingeordnet |
| 1.1 | 2026-08-06 | Wurzelbildungsregel präzisiert (keine Konsonantenhäufungen); „stad"→„sat" korrigiert (verletzte eigene Phonotaktik); TAM-Partikel-Stellung geklärt (li/pe/ke exklusiv, me satzfinal, te vor Nomen); Kernwortschatz-Entwurf (6.5, ~30 Wurzeln) und erstes Testkorpus (6.6, 7 Sätze) ergänzt |
| 1.0 | 2026-08-06 | Versionierung eingeführt. Dokumentstand zu diesem Zeitpunkt: Designprinzipien inkl. Fehlerrobustheit, Entwicklungsmethode, Phonologie, Schrift (ASCII-Begründung, b/d-Designvorgabe), Morphologie, Syntax (Rollen-Partikel, Klitisierung, Logik-Klammern, Sprech-/Schreib-Grammatik, Intonation), Wortschatzsystem (inkl. Lautsymbolik), Testprotokoll Fehlerrobustheit, Verbreitungsstrategie |

Ziel: eine Plansprache, die Kinder schnell lernen, die logisch regelmäßig ist (möglichst keine Ausnahmen), und die trotzdem komplexe/technische Sachverhalte eindeutig ausdrücken kann.

---

## 1. Designprinzipien

*Ausführliche Begründungen, historischer Kontext und offene Diskussionsfragen: siehe Buch 1 „Gedanken zu einer Weltsprache". Hier nur die Regeln selbst, als Referenz für den Rest dieses Dokuments.*

1. **Eine Regel, keine Ausnahme.** Jede grammatische Regel gilt immer, ohne Sonderfälle.
2. **Explizit statt implizit.** Struktur wird durch feste Marker sichtbar gemacht, nicht durch Wortstellung erraten.
3. **Kompositionalität als Werkzeug, nicht als Ziel.** Formale/IT-Verträglichkeit ist zweitrangig gegenüber Alltagstauglichkeit — wo beides in Konflikt gerät, entscheidet, was Menschen leicht sprechen und verstehen (Beispiel: Sprech-/Schreib-Grammatik-Trennung, 5.6).
4. **Kleiner Kern, große Reichweite.** Wenige hundert Grundwurzeln, alles andere durch Komposition.
5. **Fehlerrobustheit.** Der Sinn eines Satzes soll nicht zu stark von exakt korrekter Grammatik/Wortwahl abhängen (Testprotokoll: Abschnitt 7).
6. **Kanalrobustheit.** Verständlichkeit soll auch unter eingeschränkten Übertragungsbedingungen erhalten bleiben — Flüstern, körperliche Einschränkungen, Störgeräusch (Abschnitt 7.1).

---

## 1a. Entwicklungsmethode

1. **Kern-Skelett** (Phonologie, Wortarten, Partikelsystem) — bewusst minimal halten.
2. **Testkorpus** aufbauen: echte Alltagssätze übersetzen, nicht nur konstruierte Beispielsätze.
3. Überall dort, wo sich eine Übersetzung falsch, zu lang oder mehrdeutig anfühlt: **Regel anpassen statt Ausnahme einführen.**
4. Erst nach mehreren Testrunden Richtung „Standard" fixieren.

### 1b Parallelen zu Kreolsprachen — Befunde für die Spezifikation

*Theoretischer Hintergrund (Bickerton-Hypothese, DeGraff-Kritik) und Einordnung: siehe Buch 1. Hier nur die daraus abgeleiteten, in die Grammatik übernommenen Ergebnisse:*

- **Bestätigt:** Kreolsprachen nutzen typischerweise feste SVO-Stellung und präverbale Tempus-/Modus-Markierung — deckt sich mit dem TAM-Slot-Prinzip (4.2/5.1: `li`/`pe`/`ke`/`we` vor dem Verb, `no` direkt danach) und der (K)V-Phonotaktik (Abschnitt 2).
- **Übernommen:** Serialverbkonstruktionen ohne Konjunktion — ausgearbeitet in 5.3.
- **Noch offen:** Doppelte Verneinung als mögliche Redundanzebene (Kapitel 9).

## 2. Phonologie (Lautsystem)

**Vokale (5):** a e i o u
**Konsonanten (13):** m n p t k b d g f s l r w

- Silbenstruktur: immer (K)V — Konsonant optional, dann ein Vokal. Keine Konsonantenhäufungen, keine geschlossenen Silben.
- Betonung: immer auf der vorletzten Silbe. Keine Ausnahme.
- Keine Töne, keine Vokal-/Konsonantenlänge als Bedeutungsunterschied.

Diese 18 Laute sind bewusst so gewählt, dass sie sich akustisch stark unterscheiden (kein p/b, kein s/z-Kontrast) — das reduziert Verwechslungen bei Kindern und Nicht-Muttersprachlern.

## 3. Schrift

Lateinisches Alphabet, **streng phonemisch**: ein Buchstabe = genau ein Laut, ein Laut = genau ein Buchstabe. Keine Digraphen, keine stummen Buchstaben, keine Groß-/Kleinschreibungsregeln außer Satzanfang. Bewusst **reines ASCII**, keine Buchstaben aus anderen Alphabeten (z. B. kyrillisch) beigemischt:

- **Homoglyphen-Risiko:** Buchstaben wie kyrillisch „Р", „В", „Н", „С" sehen optisch identisch zu lateinischem R, B, H, C aus, stehen aber für andere Laute. Das würde unsichtbare Verwechslungsfehler einführen — genau das, was Abschnitt 3 („ein Buchstabe = ein Laut") und die Fehlerrobustheit (Abschnitt 7) verhindern sollen.
- **Akzeptanz hängt nicht am Alphabet.** Sprachverbreitung folgt Netzwerkeffekten (Abschnitt 8), nicht kosmetischen Gesten — einzelne fremde Buchstaben einzustreuen gewinnt kaum echte Akzeptanz, kostet aber Konsistenz.
- **Neutralität als Feature:** ein Alphabet, das keine bestehende Schrifttradition bevorzugt, vermeidet die Frage „warum dieses Schriftsystem und nicht ein anderes" — historisch einer der Gründe, warum Esperanto in manchen Regionen (u. a. China, Abschnitt 8.2) als neutrales Werkzeug akzeptiert wurde.
- Für Inklusion einzelner Schriftgemeinschaften eignen sich stattdessen optionale **Transliterationsschemata** (wie Pinyin fürs Chinesische) als separate, klar getrennte Zusatzebene — nicht als Vermischung im Kernalphabet.

Vorteil: sofort tastatur- und unicode-kompatibel, keine Sonderzeichen nötig, leicht maschinenlesbar (wichtig für IT-Anwendungen wie Sprachsynthese/-erkennung).

*(Alternative für später: ein featurales Alphabet nach Hangul-Vorbild, bei dem die Buchstabenform die Artikulationsart zeigt — z. B. alle Nasale mit gemeinsamem Grundelement. Aufwendiger, aber didaktisch noch stärker selbsterklärend. Design-Vorgabe für dieses Alphabet: b und d dürfen **keine** spiegelbildlichen Glyphen erhalten — der bekannte b/d-Umkehrfehler beim frühen Schrifterwerb ist ein reines Schriftproblem des lateinischen Alphabets, kein phonologisches, da /b/ und /d/ akustisch klar unterscheidbar sind und daher als Phonem-Kontrast erhalten bleiben.)*

### 3.1 Ausspracheentwurf

Referenzaussprachen mit IPA und englischen Näherungsbeispielen (Englisch als am weitesten verbreitete Referenzsprache gewählt — nicht, weil Englisch phonetisch ideal wäre, im Gegenteil: viele englische Laute sind selbst keine reinen Monophthonge, siehe Anmerkungen).

**Vokale:**

| Buchstabe | IPA | Englisches Beispiel | Anmerkung |
|---|---|---|---|
| a | /a/ | father (britisch) | offener, zentraler Vokal |
| e | /e/ | (kein reines Englisch-Äquivalent) | wie in Deutsch „See" oder Französisch „été", nicht wie engl. „bay" (das ein Diphthong /eɪ/ ist) |
| i | /i/ | see, machine | geschlossen, ungespannt kurz wie in „bit" vermeiden |
| o | /o/ | (kein reines Englisch-Äquivalent) | wie in Deutsch „so" oder Spanisch „no", nicht wie engl. „go" (das ein Diphthong /oʊ/ ist) |
| u | /u/ | food, moon | geschlossen, rund |

**Konsonanten:**

| Buchstabe | IPA | Englisches Beispiel | Anmerkung |
|---|---|---|---|
| m | /m/ | man | |
| n | /n/ | no | |
| p | /p/ | spin | unbehaucht — engl. wortinitiales „p" (wie in „pin") ist behaucht [pʰ], das vermeiden |
| t | /t/ | stop | unbehaucht, wie oben bei p |
| k | /k/ | skip | unbehaucht, wie oben bei p |
| b | /b/ | bed | |
| d | /d/ | dog | |
| g | /g/ | go | |
| f | /f/ | fun | |
| s | /s/ | sun | |
| l | /l/ | light | |
| r | /r/ oder /ɾ/ | Spanisch „pero" (getippt) | bewusst als Zungenspitzen-r/Tap definiert, nicht wie engl. „red" (Approximant) — international leichter erlernbar und unterscheidbarer von /l/ |
| w | /w/ | we | |

### 3.2 Featurales Alternativ-Alphabet (Entwurf)

Systematischer Aufbau nach zwei unabhängigen Parametern — konsequent nach Prinzip 1 („eine Regel, keine Ausnahme"), keine Glyphe wird frei erfunden:

**Grundform nach Artikulationsort:**

| Ort | Grundform | Laute |
|---|---|---|
| Labial (bilabial/labiodental) | Kreis ○ | m, p, b, f, w |
| Alveolar | senkrechter Strich │ | n, t, d, s, l, r |
| Velar | Keil ∧ | k, g |

**Zusatzmarkierung nach Artikulationsart** (wird der Grundform hinzugefügt):

| Art | Markierung | Beispiel |
|---|---|---|
| Nasal | Querbalken durch die Form | m, n |
| Stimmloser Verschlusslaut | keine (Grundform pur) | p, t, k |
| Stimmhafter Verschlusslaut | Punkt an der Form | b, d, g |
| Frikativ | Diagonale an der Form | f, s |
| Liquid | Haken (oben=l, unten=r — bewusst keine Spiegelbilder, siehe b/d-Lehre aus 3) | l, r |
| Glide | Bogen an der Form | w |

**Vokale — Glyphe bildet das Vokaltrapez direkt ab:** Ein Punkt auf einer Grundlinie markiert die Zungenposition an genau der Stelle, wo sie im IPA-Vokaltrapez auch steht — die Schrift *ist* hier die Artikulationskarte:

| Vokal | Position im Vokaltrapez |
|---|---|
| i | hoch, vorne (oben links) |
| e | mittel, vorne (mitte links) |
| a | tief, zentral (unten mitte) |
| o | mittel, hinten (mitte rechts) |
| u | hoch, hinten (oben rechts) |

Damit lässt sich jeder der 18 Laute aus zwei einfachen, unabhängig lernbaren Regeln ableiten, statt 18 Glyphen einzeln auswendig zu lernen — genau das Prinzip, das Hangul für Koreanisch so schnell erlernbar macht.

---

## 4. Morphologie

### 4.1 Wortarten durch Endung

**Wurzelbildung:** Eine Wurzel besteht aus einer oder mehreren vollständigen (K)V-Silben plus höchstens einem „hängenden" Konsonanten am Ende (z. B. „kal", „tun", „pom"). Dieser hängende Konsonant wird beim Anhängen der Wortart-Endung automatisch zur Onset des letzten Silbenschlags — die Wurzel selbst ist nie eigenständig aussprechbar, nur die Wurzel+Endung-Form. Konsonantenhäufungen (wie „st") sind in Wurzeln **nicht** erlaubt, auch nicht am Silbenanfang — sonst würde die Wurzel die eigene Phonotaktik (Abschnitt 2) verletzen.

| Endung | Wortart | Beispiel (Wurzel „kal" = groß) |
|---|---|---|
| -a | Nomen | kala = die Größe |
| -e | Adjektiv | kale = groß |
| -i | Verb (Grundform) | kali = größer machen |
| -o | Adverb | kalo = auf große Weise |

Jede Wurzel kann so in jede Wortart überführt werden — keine Ausnahmen, keine unregelmäßigen Formen.

### 4.2 Grammatische Partikel (unveränderlich, vor dem Wort, das sie betreffen)

Jede semantische Kategorie hat einen eigenen festen Vokal — so unterscheiden sich Partikel verschiedener Kategorien (wo Verwechslung die Satzbedeutung stark verändern würde) immer in mindestens zwei Lauten, während Partikel derselben Kategorie (wo Verwechslung weniger schadet) sich zumindest im Konsonanten unterscheiden. Begründung und Testergebnisse: Abschnitt 7.

**TAM/Satztyp (Vokal e):**

| Partikel | Funktion |
|---|---|
| pe | Vergangenheit |
| ke | Zukunft |
| we | Imperativ |
| me | Frage |
| te | Plural |

**Stellung:** `li` (unmarkiert/Präsens), `pe`, `ke` und `we` (Imperativ) besetzen denselben Platz direkt vor dem Verb und schließen sich gegenseitig aus — es steht immer genau eines davon. `no` (Verneinung) folgt direkt danach, ebenfalls vor dem Verb. `me` (Frage) markiert dagegen den ganzen Satz und steht satzfinal (wie im Mandarin „吗" oder Japanischen „か"), nicht im Prädikats-Slot. `te` (Plural) steht direkt vor dem Nomen, das es pluralisiert (`te tuna` = die Kinder). Beim Imperativ entfällt das Subjekt meist ganz, wie in den meisten natürlichen Sprachen üblich (`we lemi!` = „Geh!").

---

## 5. Syntax

### 5.1 Satzbauplan mit festen Markern

Statt sich auf Wortstellung zu verlassen, markiert je ein Partikel jede Satzrolle. Das macht die Wortstellung frei wählbar (z. B. für Betonung) — **zusätzlich gilt aber eine Standardreihenfolge als Rückfallebene**, falls ein Partikel fehlt oder verwechselt wird (siehe Testprotokoll, Abschnitt 7): Subjekt (unmarkiert) → li → Prädikat → erstes unmarkiertes Nomen danach = direktes Objekt → weitere Rollen-Phrasen.

**Rollen-Partikel (Vokal a):**

| Partikel | Rolle |
|---|---|
| (kein Marker) | Subjekt/Thema |
| li | leitet das Prädikat (Verb) ein |
| e | markiert das direkte Objekt (einziger reiner Vokal-Partikel — strukturell unverwechselbar) |
| ta | markiert Ort |
| ma | markiert Zeit |
| ka | markiert Empfänger (indirektes Objekt) |
| fa | markiert Mittel/Werkzeug |

**Beispiel** (mit Beispielwurzeln, Lexikon noch nicht final: tun=Kind, man=essen, pom=Apfel, kal=groß):

- tuna li mani e poma. → „Das Kind isst einen Apfel."
- kale tuna pe no mani e poma. → „Das große Kind aß keinen Apfel."

Adjektive stehen direkt vor dem Nomen, das sie beschreiben — feste Regel, keine Ausnahme.

### 5.1a Klitisierung im gesprochenen Register

Häufige, kurze Funktionswörter neigen in gesprochener Sprache dazu, mit dem Nachbarwort zu verschmelzen (Grammatikalisierung) — im Türkischen etwa sind die Kasussuffixe (-de, -e, -den) historisch aus solchen Postpositionen entstanden. Für „Klar" wird das als eine einzige generelle Regel erlaubt, statt als Sonderfall pro Partikel:

> Jeder Rollen-Partikel (ta, ma, ka, fa, e) darf im gesprochenen Register direkt und unbetont als Suffix ans vorangehende Nomen angehängt werden, statt als eigenes Wort davorzustehen.

Formal/geschrieben: `ta sata` (zwei Wörter, „zum Bahnhof") ↔ gesprochen/verkürzt: `satata` (ein Wort). Gleiche Bedeutung, nur andere Realisierung — keine neue Ausnahme, sondern eine zweite, gleichwertige Form derselben Regel, die kurze, alltagstaugliche Äußerungen erlaubt.

**Ellipse bei formelhaften Äußerungen:** Grüße, Dankesformeln und Wünsche sind im Alltag fast immer Ellipsen eines vollständigen Satzes — die Langform existiert grammatisch immer, nur ihre tatsächliche Realisierung darf verkürzt werden (Kompetenz vs. Performanz). Das löst die in 6.7 aufgeworfene Frage: Interjektionen sind **keine** Ausnahme von Prinzip 1, weil der zugrundeliegende Satz weiterhin regelkonform ist — nur seine Aussprache wird abgekürzt.

| Vollform | Bedeutung | Alltagskurzform |
|---|---|---|
| mi li sali e si. | Ich grüße dich. | Sala! |
| mi li gani e si. | Ich danke dir. | Gana! |
| mi li wudi ka si e gele dina. | Ich wünsche dir einen guten Tag. | Gele dina! |
| mi ke fidi e si. | Ich werde dich (wieder)sehen. | Fida! |

Auch „Gele dina!" folgt damit demselben Muster wie deutsches „Guten Tag!" — beide sind der stehengebliebene Objekt-Rest eines eigentlich vollständigen Wunschsatzes.

### 5.2 Logische Verknüpfung ohne Vorrangregeln

Statt sich Rangfolgen für „und/oder/nicht" merken zu müssen (wie bei Rechenoperatoren), wird **immer explizit geklammert** — wie Klammern in der Mathematik oder einer Programmiersprache:

**Logische Konnektoren (Vokal o):**

| Partikel | Bedeutung |
|---|---|
| ko | und |
| wo | oder |
| no | nicht (= dieselbe Verneinung wie im Satz allgemein) |
| so | wenn ..., dann ... |
| po | um ... zu (Zweck) — siehe 5.3 |
| pi ... na | öffnet/schließt eine Gruppe (wie runde Klammern) — rein schriftliches Register, siehe 5.6 und 7 |

Beispiel: „(A und B) oder C" → **pi A ko B na wo C**

Dieser eine Mechanismus (pi/na als Klammer) reicht aus, um beliebig verschachtelte, komplexe Aussagen eindeutig zu bilden — ohne dass man neue Regeln lernen muss.

### 5.3 Serialverbkonstruktionen (getestet, aus 1b)

Verbketten ohne Konjunktion, wie in Kreolsprachen üblich, wurden an zwei Fällen getestet:

- **Mitnahme-Fall:** `mi li teki e poma lemi.` (nehmen-gehen) = „ich nehme den Apfel mit" — funktioniert eindeutig, weil gleiches Subjekt + keine Konjunktion konventionell als *ein* zusammenhängendes Ereignis gelesen wird (Objekt bleibt an der gewohnten Position direkt nach dem ersten Verb).
- **Zweck-Fall:** `nu li lemi fidi.` (gehen-sehen) — hier bleibt unklar, ob eine **Abfolge** („er ging, dann sah er") oder ein **Zweck** („er ging, um zu sehen") gemeint ist. Diese Zweideutigkeit ist auch in natürlichen Serialverb-Sprachen dokumentiert, kein Konstruktionsfehler.

**Ergebnis:** Serial-Verb-Ketten sind als **informelle Kurzform** für eng verbundene Ereignisse (wie den Mitnahme-Fall) uneingeschränkt brauchbar — passend zum Sprech-Register (5.6), ohne neue Partikel. Für Zweckangaben, wo Eindeutigkeit wichtiger ist, steht der explizite Verknüpfer `po` zur Verfügung: `nu li lemi po fidi.` = „er ging, um zu sehen" (eindeutig). Damit folgt auch dieser Fall dem etablierten Muster Sprech-/Schreib-Grammatik: kurz und leicht mehrdeutig im Alltag, explizit und eindeutig, wo es zählt.

**Erweiterung (aus dem Märchen-Experiment, Buch 4):** Serialverbketten sind nicht auf zwei Verben begrenzt — beliebig viele Verben mit gleichem Subjekt und gleichem Tempus dürfen sich einen einzigen TAM-Marker teilen: `nu pe lemi ta bera, fidi e biga, sali e biga.` („es ging zum Berg, sah den Vogel, grüßte ihn" — ein `pe` für drei Verben). Die Kette bricht automatisch und vorhersagbar, sobald Subjekt oder Tempus wechseln — keine neue Ausnahme, nur eine konsequente Anwendung derselben Regel auf mehr als zwei Glieder. Löst das in langen Texten störende Muster, jeden Satz einzeln zu markieren.

### 5.4 Ja/Nein als eigenständige Antwort

| Klar | Bedeutung |
|---|---|
| nono | nein (eigenständige Antwort — Reduplikation von `no`) |
| pa | ja |

`pa` wurde bewusst gewählt, nicht `si` (das ist bereits als Pronomen „du" vergeben — eine Kollision zwischen „du" und „ja" wäre besonders riskant) und nicht `ha` (enthält „h", das nicht im 13-Konsonanten-Inventar aus Abschnitt 2 enthalten ist — Korrektur analog zu 7.1). `pa`/`no` unterscheiden sich bereits in **beiden** Lauten (Konsonant und Vokal) — anders als bei den übrigen Partikeln (Abschnitt 4.2/5.2, dort reicht sonst ein Laut Unterschied zwischen verschiedenen Kategorien) verdient das Ja/Nein-Paar den größtmöglichen Abstand, weil eine Verwechslung hier die Satzbedeutung ins glatte Gegenteil kippt — die höchste Fehlerquote im ganzen System.

**Warum die eigenständige Antwort zusätzlich verdoppelt ist:** Als isoliertes Ein-Wort-Antwort fehlt der sonstige Satzkontext, der anderswo als Rückfallebene dient (Abschnitt 7) — hier zählt jede zusätzliche Unterscheidungsebene. Silbenzahl ist akustisch eine der robustesten Eigenschaften überhaupt (reine Dauer-/Timing-Information, unabhängig von Stimmhaftigkeit, Tonhöhe oder Klangfarbe — bleibt auch unter Flüstern oder starkem Störgeräusch erhalten, Abschnitt 7.1). `nono` (zwei Silben) vs. `pa` (eine Silbe) unterscheiden sich damit zusätzlich in der Silbenzahl, nicht nur in Konsonant und Vokal — die maximal mögliche Absicherung für den höchsten Fehlerfall im System. Die Reduplikation selbst ist keine neue Regel, sondern in vielen Sprachen ein natürliches Verstärkungsmuster (vgl. informelles Doppel-„nein, nein!"). Die klauselinterne Verneinung bleibt einfaches `no` (5.5) — dort sichert der Satzkontext ohnehin ab.

### 5.5 Verneinung — Übersicht

Verneinung ist über mehrere Abschnitte verteilt eingeführt worden; hier gesammelt an einer Stelle, weil eine falsch verstandene Verneinung die Satzbedeutung ins Gegenteil kippt — der riskanteste Einzelfehler, den die Sprache kennt.

**Eine Form, drei Funktionen** — bewusst dasselbe Wort, kein separates Vokabular (Prinzip 4, kleiner Kern):

| Funktion | Verwendung | Abschnitt |
|---|---|---|
| Satzverneinung | `no` direkt vor dem Verb, nach li/pe/ke/we | 4.2, 5.1 |
| Logisches „nicht" | `no` als Konnektor in geklammerten Aussagen | 5.2 |
| Kurzantwort „nein" | `nono` (Reduplikation von `no`) als eigenständige Antwort auf eine Frage | 5.4 |

**Warum das robust ist:** `no` beginnt mit einem Nasal (n) — nasale Konsonanten bleiben auch unter erschwerten Bedingungen (Flüstern, siehe 7.1) noch über ihre charakteristische Resonanz erkennbar, anders als die Stimmhaftigkeit bei Verschlusslauten. Die Gegenform `pa` (5.4) ist bewusst maximal entfernt gewählt, die Kurzantwort `nono` zusätzlich durch Silbenzahl abgesichert.

**Offene Frage (aus 1b, noch nicht entschieden):** Manche Kreolsprachen verwenden doppelte Verneinung *innerhalb des Satzes* als zusätzliche Verstärkung/Redundanz — zu unterscheiden von der Reduplikation der *eigenständigen Kurzantwort* aus 5.4, die bereits umgesetzt ist. Ob dasselbe Prinzip auch innerhalb ganzer Sätze die Fehlerrobustheit (Abschnitt 7) verbessern würde oder nur unnötige Länge hinzufügt, ist weiterhin offen (Kapitel 9).

### 5.6 Sprech-Grammatik vs. Schreib-Grammatik

Tiefe Verschachtelung (mehrere offene Klammern gleichzeitig) überfordert das menschliche Arbeitsgedächtnis — das ist sprachübergreifend so, unabhängig davon, ob die Klammern nummeriert oder gelabelt sind. In gesprochener Alltagssprache jeder natürlichen Sprache kommt echte Verschachtelung praktisch nie vor; Menschen reihen stattdessen aneinander („ich traf ihn, er sagte X, deshalb tat ich Y" statt echter Einbettung). Das Bedürfnis nach Klammerung entsteht überhaupt erst dort, wo geschrieben und zurückgeblättert werden kann.

Für „Klar" wird diese Beobachtung zur Regel selbst, statt zur Ausnahme:

- **Gesprochene Grammatik:** ausschließlich Verkettung/Sequenzierung von Aussagen. Kein pi/na nötig — deckt jede Alltagsäußerung ab.
- **Geschriebene Grammatik:** pi/na (gelabelt, siehe 5.2) als zusätzliches, rein schriftliches Werkzeug für komplexe/formale/technische Texte — ergänzt um **visuelle Klammerung** (echte grafische Klammern oder Einrückung im Schriftbild, wie in Programmcode), die die Verschachtelungstiefe sofort sichtbar macht, statt sie im Kopf mitzählen zu müssen.

Diese Arbeitsteilung löst den scheinbaren Zielkonflikt zwischen Alltagstauglichkeit und formaler Präzision: Die gesprochene Sprache bleibt kognitiv leicht, weil sie das Problem gar nicht erst hat; die geschriebene Sprache kann beliebig präzise und verschachtelt sein, weil die Schrift selbst die Gedächtnislast übernimmt, die das gesprochene Wort nicht leisten könnte.

### 5.7 Intonation als zusätzliche Redundanzebene

Da „Klar" **kein phonemisches Tonsystem** hat (Tonhöhe verändert nie die Wortbedeutung, anders als z. B. im Mandarin), ist Intonation komplett frei für paralinguistische Funktionen — und lässt sich als **fünfte Fehlerkorrektur-Ebene** neben Partikel, Wortstellung, semantischer Plausibilität und Lautsymbolik (6.4) nutzen:

- **Steigende Endintonation** am Satzende = zusätzliches, redundantes Signal für eine Frage. Der Frage-Partikel `me` bleibt der Hauptmarker, die Intonation sichert ihn ab, falls `me` überhört oder falsch ausgesprochen wird. Das ist sprachübergreifend robust: steigende Frageintonation kommt in den allermeisten Sprachen der Welt vor (Frequenzcode, Ohala) — kollidiert auch nicht mit Tonsprachen wie Mandarin, die trotz Lexikaltönen zusätzlich Satzintonation verwenden.
- **Erhöhtes Tonregister** allgemein = paralinguistischer Marker für Vorsicht/Höflichkeit/Unterordnung, **tieferes Register** für Sicherheit/Nachdruck. Kein Teil der Kerngrammatik (kein Lernaufwand nötig), aber bewusst dokumentiert, damit Lernende wissen: das ist kein Zufall, sondern ein kulturübergreifend geteiltes Muster, auf das man sich verlassen kann.

### 5.8 Weitere Konstruktionen (aus dem Testkorpus entdeckt)

Beim Übersetzen echter Alltagssätze (6.6) fielen mehrere Lücken auf, die sich alle ohne neue Grammatik-Partikel schließen ließen — reine Anwendung bereits bestehender Regeln:

- **Kopula-lose Prädikation:** Adjektive können ohne „sein"-Verb direkt als Prädikat stehen (`mie doma kale` = „mein Haus [ist] groß") — typologisch verbreitet (z. B. Chinesisch, Japanisch), spart ein eigenes Kopula-Wort. Gilt auch für subjektlose Wetterausdrücke (`nuno ware` = „heute [ist es] warm" — kein Scheinsubjekt wie deutsches „es" nötig).
- **Possessiv über Adjektiv-Endung:** Pronomen + Adjektiv-Endung `-e` (Abschnitt 4.1) ergibt die Possessivform: `mi` (ich) → `mie` (mein), `si` (du) → `sie` (dein), `nu` (er/sie/es) → `nue` (sein/ihr). Keine neue Regel nötig, nur Wiederverwendung von 4.1.
- **Komparativ:** Adverb `pulo` (mehr, aus Wurzel „pul") vor dem Adjektiv, gefolgt von `komo` (als/verglichen mit) vor dem Vergleichsobjekt: `nu pulo kale komo mi` = „er [ist] größer als ich".
- **Konjunktion auf Wortebene:** `ko` (und, bisher nur für ganze Aussagen gedacht, 5.2) funktioniert genauso zum Verbinden einzelner Satzglieder: `mama ko nana` = „Mutter und Vater". Keine separate Wort-Konjunktion nötig.

---

## 6. Wortschatzsystem

### 6.1 Kern

Ca. 300–500 konkrete Grundwurzeln (Körper, Familie, Natur, Handlungen, Zahlen, Eigenschaften) — alles Abstrakte/Technische wird durch **Komposition** gebildet, Kopf steht am Ende:

Beispiel: „Dampf" = wera (Wasser) + pira (Feuer/Hitze) → **werapira**

### 6.2 Zahlensystem

Zehn Ziffernwurzeln (0–9), Zahlen werden wie Stellenwerte zusammengesetzt (kein Sonderfall wie „elf/zwölf" im Deutschen):

- 23 = „zwei-zehn-drei" → **dua-leka-fin**
- 100 = **sena**

### 6.3 Neuwortbildung (für Fachbegriffe/IT) und Eigennamen

Zwei unterschiedliche Fälle, zwei unterschiedliche Regeln:

- **Fachbegriffe/allgemeine Lehnwörter** (z. B. IT-Begriffe): feste, dokumentierte Regeln statt freier Übernahme — neue Fachbegriffe werden immer aus vorhandenen Wurzeln komponiert oder nach klaren Lautanpassungsregeln eingedeutscht, nie willkürlich übernommen. Das hält den Wortschatz konsistent lernbar.
- **Eigennamen und Bezeichnungen** (Personennamen, Ortsnamen, Markennamen): **Aussprache bleibt unverändert**, nur die Schreibung wird ans Alphabet angepasst (Transliteration, nicht Übersetzung) — ähnlich wie Pinyin chinesische Namen für lateinische Schrift zugänglich macht, ohne ihren Klang zu verändern. Ein Lautinventar-fremder Laut wird durch den nächstgelegenen Klar-Laut ersetzt, dokumentiert in einer festen Transliterationstabelle (analog zum Ausspracheentwurf, Abschnitt 3.1).

Diese Trennung ist wichtig: Fachbegriffe sollen in die Systematik der Sprache passen (kompositionell, durchschaubar), Namen sollen erkennbar bleiben (Wiedererkennbarkeit hat hier Vorrang vor Systemkonsistenz).

### 6.4 Lautsymbolik als Vokabular-Prinzip

Auch wenn sprachliche Zeichen über den gesamten Wortschatz hinweg beliebig sind, gibt es einen gut belegten Ausnahmebereich (Bouba-Kiki-Effekt, Frequenzcode nach Ohala): Runde, weiche Laute (m, n, l, r + o, u) werden sprachübergreifend konsistent mit „rund, weich, groß, sanft" assoziiert; scharfe, harte Laute (p, t, k + i) mit „spitz, hart, klein, schnell". Das ist einer der wenigen wirklich universellen Befunde der Lautsymbolik-Forschung.

Regel für den Kernwortschatz: Wurzeln für weiche/sanfte/große Konzepte (Wasser, Mutter, ruhen, Liebe) bevorzugt mit Sonoranten (m, n, l, r) und Rundvokalen (o, u) bilden; Wurzeln für harte/scharfe/schnelle/gefährliche Konzepte (Stein, brechen, schneiden, Gefahr) bevorzugt mit stimmlosen Verschlusslauten (p, t, k) und dem Vokal i. Das gibt eine **sechste Redundanzebene** (neben Rollen-Partikeln und Standardreihenfolge aus 5.1, semantischer Plausibilität aus Abschnitt 7, und Intonation aus 5.7): selbst ein unbekanntes Wort lässt sich grob in die richtige Gefühlsrichtung einordnen, bevor die exakte Bedeutung bekannt ist.

### 6.4a Onomatopoesie (Lautmalerei)

Verwandt mit, aber nicht identisch zur Lautsymbolik aus 6.4: Lautsymbolik verknüpft Laute mit *abstrakten* Bedeutungen (weich/hart), Onomatopoesie ahmt *konkrete Geräusche* direkt nach. Wie überall im Lexikon gilt die (K)V-Phonotaktik (Abschnitt 2) auch hier ohne Ausnahme — echte Cluster wie im deutschen „Knall" oder „Plumps" sind nicht nachbildbar, nur die Klangqualität wird über Konsonant- und Vokalwahl angenähert. Alle Wurzeln unten mit dem Prüfskript (7.1) validiert:

| Wurzel | Bedeutung | Lautqualität |
|---|---|---|
| bum | Bumm/dumpfer Knall | Nasal + Rundvokal — dumpf, tief |
| rak | Krach | harter Verschlusslaut + a — schroff |
| tak | Knall (kurz, scharf) | stimmloser Verschlusslaut beidseitig — abrupt |
| ris | Kratzen | Frikativ s — schleifend |
| dum | dumpf | Nasal + Rundvokal, wie „bum" — passend redundant |
| pos | Plumps | stimmloser Anlaut + Rundvokal — weiches Auftreffen |
| bat | laut | stimmhafter Anlaut + a — offen, voll |
| sil | leise | Frikativ + i + l — gedämpft, eng |

„bat"/„sil" (laut/leise) sind kein reiner Nachhall eines Geräuschs, sondern nutzen bewusst dasselbe Lautsymbolik-Prinzip aus 6.4 (offener/harter Laut vs. enger/weicher Laut) — ein Grenzfall zwischen Onomatopoesie und Lautsymbolik, der zeigt, dass beide Phänomene ineinander übergehen.

### 6.5 Kernwortschatz — erste Fassung (Entwurf, ~30 Wurzeln)

Erster Ausschnitt zum Testen, noch nicht vollständig. Lautsymbolik (6.4) wo sinnvoll angewendet.

**Pronomen** (Plural über Partikel „te", keine eigenen Wurzeln nötig — Prinzip 4: kleiner Kern):
mi = ich · si = du · nu = er/sie/es

**Personen/Familie** (weich, Sonoranten): mam = Mutter · nan = Vater · tun = Kind

**Natur** (gemischt je nach Charakter): wer = Wasser (weich) · pir = Feuer (hart, scharf) · sat = Ort/Bahnhof-artiger Ort · lun = Mond (weich) · kal = groß · pom = Apfel (fehlte bisher trotz durchgängiger Verwendung in Beispielsätzen)

**Handlungen**: man = essen · lem = gehen · pak = brechen (hart, passend zur Bedeutung) · lor = ruhen/schlafen (weich, passend) · fid = sehen · dik = sagen · ben = kommen · don = geben · res = bleiben · bol = wollen · sal = grüßen · gan = danken · fen = fühlen · tek = nehmen

**Eigenschaften**: kal = groß · pik = klein/spitz (hart) · mol = weich/rund (weich, lautmalerisch passend) · rop = schnell · mil = freundlich · gel = froh/glücklich · war = warm

**Sonstiges**: dom = Haus · pul = mehr (Komparativ, 5.8) · kom = Vergleich (Komparativ, 5.8) · nun = jetzt/heute · wud = wünschen · din = Tag · kel = Interrogativ-Stamm (was/wer/welch-, 6.8) · poi = später/danach

**Ziffern 0–9** (Abschnitt 6.2): nul · un · dua · fin · fer · pen · sik · sep · ok · nom

### 6.6 Testkorpus v1

Erste Beispielsätze zum Prüfen der Grammatik an echten Alltagsäußerungen (Methode: Abschnitt 1a).

| Deutsch | Klar |
|---|---|
| Ich esse einen Apfel. | mi li mani e poma. |
| Die Mutter geht zum Bahnhof. | mama li lemi ta sata. |
| Das Kind schläft nicht. | tuna li no lori. |
| Wirst du kommen? | si ke beni me? |
| Ich gab dem Vater Wasser. | mi pe doni ka nana e wera. |
| Das große Kind aß keinen Apfel. | kale tuna pe no mani e poma. |
| Wenn es regnet, bleibe ich zu Hause. | so pi wera lemi na, mi li resi. |

*(Wurzel „beni"=kommen war hier zusätzlich verwendet, ist inzwischen in 6.5 aufgenommen.)*

### 6.7 Testkorpus v2 — Alltagssituationen

Gezielt über verschiedene Situationen verteilt, um Lücken in der Grammatik zu finden (Methode: Abschnitt 1a). Gefundene Lücken sind in 5.8 bereits als Regeln dokumentiert.

| Situation | Deutsch | Klar |
|---|---|---|
| Begrüßung | Hallo! | Sala! |
| Bitte (Imperativ) | Gib bitte Wasser! | We doni milo e wera! |
| Dank | Danke! | Gana! |
| Besitz | Mein Haus ist groß. | Mie doma kale. |
| Vergleich | Er ist größer als ich. | Nu pulo kale komo mi. |
| Vergleich (verneint) | Ich bin nicht größer als du. | Mi no pulo kale komo si. |
| Gefühl | Ich fühle mich gut. | Mi feni gele. |
| Frage nach Befinden | Fühlst du dich gut? | Si feni gele me? |
| Small Talk (Wetter) | Heute ist es warm. | Nuno ware. |
| Ort + Zeit kombiniert | Ich gehe jetzt zum Bahnhof. | Mi li lemi ta sata ma nuno. |
| Zukunft + Ort | Ich werde zum Bahnhof gehen. | Mi ke lemi ta sata. |
| Vergangenheit + Frage | Bist du gekommen? | Si pe beni me? |
| Verneinter Wunsch | Ich will kein Wasser. | Mi li no boli e wera. |
| Konjunktion von Satzgliedern | Mutter und Vater sind froh. | Mama ko nana gele. |
| Imperativ (einfach) | Geh! | We lemi! |

**Beobachtungen aus diesem Durchgang:**
- Kein einziger Satz brauchte eine neue Grammatik-*Partikel* außer dem Imperativ „we" — alle anderen Lücken (Possessiv, Komparativ, Kopula) ließen sich mit bereits vorhandenen Bausteinen füllen (5.8). Das bestätigt Prinzip 4 („kleiner Kern, große Reichweite") in der Praxis.
- Ein weiterer Phonotaktik-Verstoß in einer älteren Beispielwurzel gefunden und korrigiert: `rest`→`res` (Cluster „st"). Zeigt: der Testkorpus-Prozess (1a) fängt genau solche Fehler zuverlässig ab, bevor sie sich im Lexikon festsetzen.
- Offen: „Sala!" und „Gana!" werden hier als eigenständige Ausrufe benutzt (Nomen ohne Prädikatsrahmen) — noch nicht geklärt, ob Interjektionen generell von der normalen Satzstruktur ausgenommen sein dürfen, ohne Prinzip 1 („keine Ausnahme") zu verletzen. Für die nächste Runde vormerken. *(→ inzwischen gelöst, siehe 5.1a: Ellipse statt Ausnahme.)*

### 6.8 Testkorpus v3 — zusammenhängender Dialog

Ein kurzer Dialog statt Einzelsätze — prüft Pronomen-Referenz, W-Fragen und Sprechbarkeit im Zusammenhang.

| Sprecher | Klar | Deutsch |
|---|---|---|
| A | Sala! | Hallo! |
| B | Sala! Si feni gele me? | Hallo! Geht's dir gut? |
| A | Mi feni gele. Si feni gele me? | Mir geht's gut. Und dir? |
| B | Mi feni gele. | Mir geht's gut. |
| A | Si ke beni ta doma mie ma kela? | Wann kommst du zu meinem Haus? |
| B | Mi ke beni ta doma sie ma poio. | Ich komme später zu deinem Haus. |
| A | Mile! Fida! | Schön! Auf Wiedersehen! |
| B | Fida! | Auf Wiedersehen! |

**Neu entdeckt:** W-Fragen brauchten kein eigenes grammatisches Konstrukt. Der Interrogativ-Stamm `kel` (was/wer/welch-) wird einfach an der Stelle eingesetzt, an der die gesuchte Information stehen würde — kombiniert mit den bereits bestehenden Rollen-Partikeln ergeben sich alle W-Wörter von selbst: `kela` = wer/was, `ta kela` = wo, `ma kela` = wann. Kein Voranstellen nötig (wie im Deutschen „wann kommst du" mit Verb-Zweit), sondern **W-Fragen in situ** — wie im Mandarin oder Japanischen, wo das Fragewort einfach an seiner normalen syntaktischen Position bleibt. Passt zur bestehenden freien Wortstellung (5.1) und braucht keine zusätzliche Bewegungsregel.

Auch bestätigt: `mie`/`sie` (Possessiv, 5.8) und die Ellipsen-Grüße (5.1a) funktionieren im Fließtext genauso wie isoliert — keine neuen Reibungspunkte im Dialogkontext gefunden.

---

## 7. Testprotokoll: Fehlerrobustheit

Methode: kleine Beispielsätze korrekt bilden, dann systematisch „beschädigen" (Partikel weglassen, Reihenfolge ändern) — wie ein Hörfehler oder ein Fehler eines Nicht-Muttersprachlers das tun würde — und prüfen, ob die Bedeutung noch rekonstruierbar bleibt.

**Test 1 — Rollen-Partikel weggelassen, Standardreihenfolge intakt:**
`mi li mani e poma` → `mi li mani poma` (e weggelassen). Bedeutung bleibt erhalten, weil die Position direkt nach dem Prädikat als Rückfallebene für „direktes Objekt" gilt. → bestätigt: Standard-Wortstellung als zweite, unabhängige Kodierung funktioniert.

**Test 2 — Partikel weggelassen, Verb-Bedeutung rettet den Satz:**
`mi li lemi ta sata` → `mi li lemi sata` (ta weggelassen). „Gehen" nimmt normalerweise kein direktes Objekt — die Wortbedeutung selbst schließt die falsche Lesart aus. → dritte Fehlerkorrektur-Ebene neben Partikel und Wortstellung: semantische Plausibilität.

**Test 3 — zwei Fehler gleichzeitig:**
`poma mi mani` (Objekt vorangestellt, li und e fehlen). Nur noch über Weltwissen erratbar („ein Apfel isst nicht"), nicht mehr über Sprachstruktur. → **eine Fehlerebene wird zuverlässig abgefangen, zwei gleichzeitige nicht mehr.** Als Zielgröße für „Klar" festgehalten.

**Test 4 — phonetischer Abstand der Partikel:**
Audit der ursprünglichen Partikelliste ergab mehrere riskante Beinah-Verwechslungen zwischen bedeutungsfernen Kategorien: `no`/`na`, `wo`/`no`, `pe`/`pa`; außerdem verletzte `kin` (Silbenkoda) die eigene Phonotaktik. → behoben durch Kategorie-Vokal-Prinzip (Abschnitt 4.2, 5.1, 5.2): unterschiedliche Kategorien unterscheiden sich immer in mind. zwei Lauten, gleiche Kategorie mindestens im Konsonanten.

**Ergebnis:** Fehlerrobustheit lässt sich nicht durch eine einzelne Regel erreichen, sondern entsteht aus dem Zusammenspiel dreier unabhängiger Rückfallebenen — Partikel, Standardreihenfolge, semantische Plausibilität. Weitere Testsätze sollten diese Redundanz gezielt prüfen, bevor der Kern fixiert wird.

### 7.1 Kanalrobustheit: Flüstern und körperliche Einschränkungen

Zusätzlich zu Hörfehlern (Test 1–4) wurde geprüft, was passiert, wenn der akustische Kanal selbst eingeschränkt ist — nicht nur einzelne Laute falsch ankommen, sondern eine ganze Merkmalsklasse ausfällt.

**Flüstern eliminiert Stimmhaftigkeit vollständig** (keine Stimmbandschwingung, kein Tonhöhensignal) — genau das Merkmal, das unsere stimmhaft/stimmlos-Paare (p/b, t/d, k/g) unterscheidet. Audit auf Wortpaare, die sich **ausschließlich** durch Stimmhaftigkeit unterscheiden, fand zwei bisher unbemerkte Fälle:

- `da` (Zeit) vs. `ta` (Ort) — nur d/t unterschiedlich → korrigiert zu `ma` (Zeit, Abschnitt 5.1)
- `dek` (zehn) vs. `tek` (nehmen) — nur d/t unterschiedlich → korrigiert zu `lek` (zehn, Abschnitt 6.2)

Als Regel für künftige Wortbildung festgehalten: **kein Wortpaar darf sich ausschließlich durch Stimmhaftigkeit unterscheiden**, auch wenn Abschnitt 4.2 das (als Konsonanten-Unterschied innerhalb derselben Kategorie) formal erlauben würde — Stimmhaftigkeit ist der unter Flüstern am wenigsten robuste Kontrast.

**Intonation fällt beim Flüstern ebenfalls weg** (kein Tonhöhenverlauf ohne Stimmbandschwingung) — bestätigt im Nachhinein, dass Abschnitt 5.7 von Anfang an richtig entworfen wurde: die Frage-Intonation ist dort explizit nur **zusätzliches** Signal neben dem Partikel `me`, nicht die einzige Markierung. Beim Flüstern trägt allein `me` die Bedeutung — die Sprache bleibt verständlich, nur eine Redundanzebene weniger.

**Körperliche Einschränkungen** betreffen vor allem den Zungenspitzen-r (Abschnitt 3.1) — ein Laut mit feinmotorischen Anforderungen, den nicht alle Sprecher zuverlässig bilden können (in vielen Sprachen einer der zuletzt erworbenen und am häufigsten betroffenen Laute bei Sprechschwierigkeiten). Prüfung des bisherigen Wortschatzes ergab: **kein einziges Wortpaar unterscheidet sich aktuell nur durch r vs. l** — eine Ersetzung r→l ist also für Sprecher mit eingeschränkter Aussprache gefahrlos möglich, ohne eine andere Bedeutung zu treffen. Als offiziell sanktionierte Ausweichform festgehalten, verbunden mit einer Vorgabe für die künftige Wortbildung: r/l-Minimalpaare sind zu vermeiden, damit diese Ausweichoption dauerhaft kollisionsfrei bleibt.

**Ergebnis:** Die bestehende dreifache Redundanz (Partikel, Wortstellung, Plausibilität, Abschnitt 7) trägt die Bedeutung strukturell weiter, auch wenn einzelne Laute unter Flüstern oder eingeschränkter Aussprache verloren gehen — Kanalrobustheit ist damit größtenteils ein Zusatzcheck auf Wortebene (keine Stimmhaftigkeits-Minimalpaare, keine r/l-Minimalpaare), keine neue Grammatik.

---

## 8. Verbreitungsstrategie

*Die grundsätzliche Frage, ob Design-Qualität überhaupt Verbreitung erzeugen kann und ob das als Projektziel sinnvoll ist, wird in Buch 1 „Gedanken zu einer Weltsprache" als offene Diskussionsfrage behandelt. Hier die praktischen Konsequenzen für „Klar" konkret.*

**Ausgangsbefund, unbequem aber wichtig:** Keine geplante Sprache ist je aus reiner Qualität heraus zur Weltsprache geworden. Esperanto existiert seit 1887, hat Millionen Lerner gehabt, ausgezeichnete Logik, engagierte Communities — und blieb Nische. Grund: Sprachverbreitung folgt einem **Netzwerkeffekt** (man lernt eine Sprache, weil andere sie schon sprechen, mit denen man etwas zu tun hat), nicht der Qualität der Sprache selbst. Englisch ist Weltsprache wegen Empire/Wirtschaft/Technologie/Populärkultur, nicht wegen seiner (eher chaotischen) Grammatik.

### 8.1 Konsequenzen für „Klar"

- **Konkreter Nutzenhaken statt abstraktes Ziel.** „Weltfrieden" (Esperantos Ziel) ist zu abstrakt. Ein konkreter technischer Nutzen — z. B. als **Pivot-Sprache für maschinelle Übersetzung** (Zwischenformat, über das viele Sprachpaare laufen, reduziert n² Übersetzungsrichtungen auf n) — funktioniert unabhängig von kultureller Akzeptanz und passt zu den IT-nahen Designentscheidungen (Abschnitt 3, 8.2).
- **Open-Source-Modell statt Einzelprojekt.** Öffentliches Repository, RFC-Prozess für Grammatikänderungen, offene Lizenz — passt zur bisherigen Entwicklungsmethode (1a: Testkorpus, iterative Regelanpassung) und zieht die Art Mitstreiter an (Linguisten, Entwickler, Lehrer), die technisch mitgestalten statt nur konsumieren.
- **Kinder/Bildung als Einstiegspunkt**, nicht Erwachsene. Sprachen verbreiten sich glaubwürdiger über Bildung als über Erwachsenenwerbung — ein Kinderbuch-Testkorpus oder eine spielerische App wäre ein realistischerer erster Meilenstein als „Weltsprache".

### 8.2 Chinesischsprachige Sprecher einbeziehen

Keine homogene Gruppe mit einem Interesse — aber zwei konkrete Ansatzpunkte:

- **Strukturelle Nähe nutzen:** Mandarin ist isolierend (keine Flexion, keine Kasus, Bedeutung stark aus Position/Partikeln) — strukturell näher an „Klar" (Partikel statt Flexion, Standardreihenfolge als Rückgrat, Abschnitt 5.1) als z. B. Deutsch oder Russisch mit ihrem Kasussystem. Für Mandarin-Sprecher wäre der Umstieg strukturell leichter — das lässt sich in Erklärmaterial gezielt herausstellen.
- **Bestehende Netzwerke:** Esperanto hat in China historisch eine aktive Szene (u. a. weil es in den 1900ern als politisch neutrales Werkzeug gegen westliche Dominanz galt) — realer Ansatzpunkt für erste Kontakte, statt bei null anzufangen.

---

## 9. Offene Punkte für die Vertiefung

- Pronomen-Mehrdeutigkeit bei mehreren dritten Personen (`nu` unterscheidet nicht zwischen mehreren belebten Referenten) — aufgefallen im Märchen-Experiment (Buch 4); mögliche Lösung nach Vorbild der Algonkin-Sprachen (proximate/obviative Unterscheidung), noch nicht ausgearbeitet
- Prüfen, ob doppelte Verneinung *innerhalb des Satzes* als zusätzliche Redundanzebene sinnvoll ist (aus 1b, Abschnitt 7; zu unterscheiden von der bereits umgesetzten Reduplikation der Kurzantwort in 5.4)
- Weitere Testsätze gezielt für Fehlerrobustheit sammeln (Abschnitt 7 ausbauen)
- Vollständiges Kernlexikon (300–500 Wurzeln) ausarbeiten
- Formale Grammatik als BNF niederschreiben — als internes **Prüfwerkzeug** (ist wirklich jeder Satz eindeutig?), nicht als Vorgabe für die Sprachgestaltung selbst (Priorität: Alltagstauglichkeit, siehe Prinzip 3)
- Testen: Wie klingt/schreibt sich ein längerer, verschachtelter Text? *(erster Dialogtest in 6.8 erledigt; erstes zusammenhängendes Märchen in Buch 4 erledigt — Serialverbketten-Erweiterung daraus bereits übernommen, Pronomen-Frage siehe oben)*
- Featurales Alphabet (3.2) grafisch als Glyphen ausarbeiten — bisher nur als Konstruktionsregel beschrieben
- Erste Kontakte zu Linguistik-/Esperanto-Communities für Mitstreiter (Abschnitt 8) knüpfen
