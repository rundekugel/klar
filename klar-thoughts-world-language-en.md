# Klar — Thoughts Toward a World Language

**Version:** 1.0 · **As of:** 2026-08-06
*Book 1 of a planned series: (1) Why, (2) Draft/Specification, (3) Dictionaries, (4) Experiments. This document explains the reasoning behind the rules in the draft document — see there for details.*

## Changelog

| Version | Date | Change |
|---|---|---|
| 1.0 | 2026-08-06 | First version: motivation, historical context, design philosophy, scientific background (with counter-positions), open questions for discussion |

---

## 1. Why a new planned language at all?

Anyone designing a planned language today has to face an uncomfortable fact: there are already more than 900 documented attempts to build a better language (Okrent 2009). Almost all of them failed, measured against their own ambition — to become an international lingua franca. After nearly 140 years, Esperanto is the only one with a meaningful speaker community and genuine native speakers.

"Klar" does not claim to break this pattern. Its value lies elsewhere: in the **method** by which the language is built, and in the question of whether that method teaches us something — about language, about language acquisition, about the limits of what design can achieve at all.

## 2. What has been tried historically — and why it mostly failed

Three broad waves of planned languages can be distinguished (Okrent 2009):

- **Philosophical languages** (17th century, e.g. John Wilkins) tried to classify the world itself logically and derive language directly from that classification — impressive as a thought experiment, unusably complex in practice.
- **Schematic auxlangs** (Volapük 1879, Esperanto 1887, Ido, Interlingua) aimed for a neutral, easily learnable lingua franca for international exchange. Esperanto was the most successful of these — but its success cannot be attributed to grammatical superiority. Volapük had more followers at one point and did not collapse because of the language itself, but because of a dispute over reform authority.
- **Logical languages** (Loglan, later Lojban) pursued radical unambiguity modeled on formal logic — with the result that they are linguistically fascinating but too difficult for most people to actually learn.

"Klar" tries to take something from all three traditions without repeating each one's particular trap: the regularity of the auxlangs, the unambiguity of the logical languages — but bounded by what a child can learn incidentally (see the draft document, Principles 1–4).

## 3. The real design decision: method over intuition

Most historical planned languages were written by a single person, often in a relatively short time, and only tested against reality afterward (if at all). "Klar" deliberately reverses that order — every rule was checked against real example sentences before being considered "done" (draft document, Section 1a), and an automated validation script prevents new words from silently violating the language's own phonotactics or uniqueness constraints (Section 7.1).

This is not a language-design dogma, just the transfer of a method from software development (iterative testing, automated regression checking) to a field traditionally handled more intuitively. Whether this ultimately produces a *better* language is an open question — what it certainly produces is a more *traceable* one: every rule can be traced back to a concrete test case, not just to taste.

## 4. Scientific context — and the counter-positions

To keep this project from drifting into pure speculation, several design decisions lean on existing research. It's important to include the criticism of these theories too — none of it is uncontested:

**Bioprogram hypothesis (Bickerton 1981, *Roots of Language*).** Creole languages, which arise from heavily simplified pidgin input, show strikingly similar grammatical features worldwide (fixed SVO order, preverbal tense/mood marking). Bickerton's claim: children fill in missing structure from an innate "bioprogram." "Klar" shares some of these features (draft document, 1b) — not because we consider the hypothesis proven, but because the overlap is at least a suggestive sign. **Counter-position:** Michel DeGraff has sharply criticized this form of "creole exceptionalism" (DeGraff 1999, 2005) — in his view, creole languages are not fundamentally different grammatically from other naturally arisen languages, and the supposed similarity is partly colonial ideology rather than a neutral finding. This debate remains unsettled.

**Frequency code (Ohala 1983, 1984).** High pitch is cross-linguistically associated with smallness, non-threat, and politeness; low pitch with dominance — derived from the correlation between body size and voice pitch across many animal species. The intonation rule in Section 5.7 of the draft rests on this. Ohala's model is influential, but here too there is criticism of its empirical reach (e.g. Grawunder & Winter, who question some of the proposed correlations).

**Propaedeutic effect of Esperanto.** Several independent studies (among them Szerdahelyi in Hungary in the 1960s; the *Springboard to Languages* project at the University of Manchester, roughly 2005–2011) found evidence that learning Esperanto first speeds up the later acquisition of further foreign languages — presumably because its regular grammar builds metalinguistic awareness early on. If that holds, it would suggest that an *even more* regular, deliberately child-oriented language like "Klar" could have a similar or larger effect — pure speculation so far, untested.

## 5. Open questions for discussion

These points are deliberately left unresolved — meant to invite disagreement and hands-on experimentation, not quiet agreement:

1. **Can design quality drive adoption at all?** The historical evidence argues against it (Esperanto vs. network effects, see draft document Chapter 8). Does "build a better language" even make sense as a project goal then — or is it only justifiable as a source of insight, independent of adoption?
2. **Double negation as redundancy or as baggage?** Creole languages often use it; "Klar" currently does not. Would this be a genuine error-robustness improvement, or just an unnecessary complication that contradicts the project's own minimalism principle (open point, draft document Chapter 9)?
3. **How much of the creole resemblance is coincidence?** Given DeGraff's critique: are the structural parallels between "Klar" and creole languages a sign of children's learning preferences — or simply what happens when *anyone* simplifies radically, regardless of cognition?
4. **Does "channel robustness" (whispering, articulation limitations) justify its own linguistic niche?** No major auxlang has deliberately pursued this so far. Is this a real gap — or a niche problem not worth the effort of an entire language?
5. **What would it even mean for "Klar" to "work"?** Esperanto measures success by speaker numbers. If adoption is explicitly not the goal (see point 1) — what would success for this experiment be measured by instead?

## 6. Invitation

In its current form, "Klar" is a tool for thinking about language, not primarily a means of communication. Its value comes from experimentation — building sentences that strain the grammar, writing poems that trip over the stress pattern, inventing words that the validation script rejects. Every discovered fracture is more interesting than any confirmed rule.

---

## References

- Bickerton, Derek (1981). *Roots of Language*. Ann Arbor: Karoma Press.
- DeGraff, Michel (1999, 2005). Critique of "creole exceptionalism" — among others in: *Language Creation and Language Change: Creolization, Diachrony, and Development* (ed. DeGraff), MIT Press.
- Ohala, John J. (1983). Cross-language use of pitch: An ethological view. *Phonetica* 40, 1–18.
- Ohala, John J. (1984). An ethological perspective on common cross-language utilization of F0 of voice. *Phonetica* 41, 1–16.
- Okrent, Arika (2009). *In the Land of Invented Languages*. New York: Spiegel & Grau.
- Roehr-Brackin, K. / Tellier, A. et al. Findings from the *Springboard to Languages* project, University of Manchester (ca. 2005–2012).
- Szerdahelyi, István (1960s). Hungarian comparative study on the propaedeutic effect of Esperanto, University of Budapest.

*Note: These references come from research conducted during this conversation and should be checked against the original sources before any actual publication (exact page numbers, possibly later editions).*
