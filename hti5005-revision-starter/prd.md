# HTI5005 Revision Starter: Product Requirements

## 1. Goal
A quick revision page for the HTI5005 multiple-choice test on Thursday 19 November 2026, built from the Week 1–3 2026 lecture slides, with sample questions to practise on. It also prepares the user for the lifeboat debate and the group report that follow the test.

## 2. Artifact type
`html-app`: a single self-contained page. All content is built in, nothing is loaded when it opens, and nothing is saved between visits.

## 3. Data model
The page reads no data at run time. Its content is drawn from the sources below.

**Lecture slides, Weeks 1–3 (2026)**: 201 slide pages (51, 75 and 75).

| Field | Meaning |
|---|---|
| week | 1, 2 or 3 |
| page | slide page number |
| text | text of the slide |
| image note | content read from a picture-only slide, where there is one |
| check status | whether that reading was confirmed against the slide text or read from the picture only |
| same as | the earlier slide this one repeats, where it is a repeat |

Sample rows:

| week | page | text (shortened) | check status |
|---|---|---|---|
| 1 | 28 | Distributive justice is the proper allocation of resources in a manner that is fair and just; not necessarily equal; triage is a common example | text |
| 2 | 64 | Golden mean: cowardice (deficiency), courage (mean), recklessness (excess) | confirmed from the slide picture |
| 3 | 35 | Seven principles of research ethics: valuable question, valid methodology, fair subject selection, favourable risk-benefit, independent review, informed consent, respect for enrolled subjects | text |
| 3 | 12 | Pragmatism slide | repeat of Week 2 page 74 |

**Subject Assessment Guidelines (2026)**: 3 pages.

| Item | Content |
|---|---|
| Group report parts | (a) role and duty; (b) contribution assessed in terms of Pragmatism; (c) Moral Diversity found or not, and why; (d) summary: each member's role and the virtue of the decision-making |
| Marking grid | proper use of terms 5; comprehension and application of concept/theory 10; logical flow of decision-making 10; references 5; writing 5; total 35 |
| Test format | one hour, 60 multiple-choice questions, 60% of the grade |
| Report | 40% of the grade; deadline 29 Nov 2026, 24:00 |
| Appendix | list of nine bioethical issues |

**Course announcement**

| Item | Content |
|---|---|
| Test | Thu 19 Nov 2026, room Z504, arrive before 6:40 pm, multiple-choice, about 40 minutes, number of questions not stated |
| Group work | worksheet after the test; up to 10 members, 4–6 suggested, at most 2 students per role |
| Individual participation form | due 9:30 pm the same day |
| Group report | due Sun 22 Nov 2026, 23:59, by email, signed worksheet scanned as the cover page |

**Outside references**: background only, not course material.

| Topic | Content (shortened) |
|---|---|
| Lifeboat ethics | A 1974 metaphor for distributing scarce resources: a lifeboat with 50 aboard, room for 10 more, and 100 swimmers around it |
| Moral diversity | The observed fact that people and cultures hold differing moral values |

## 4. Functional requirements
1. Present short revision notes covering Weeks 1–3, quick to get through with limited study time.
2. Take every fact from the slides. Anything from another source carries a visible "not from the slides" label.
3. Show a slide that is repeated across weeks only once.
4. Mark three details as read from the slide picture rather than text-checked:
   - the 3–6 year pre-clinical stage (Week 3, page 22);
   - two of the five Patients' Charter headings, medical treatment and choices (Week 2, page 13);
   - the 1–6 numbering of the six data protection principles (Week 2, page 37).
5. Provide 30 sample multiple-choice questions, about ten per week of slides. State that they are newly written from the slides and are not official or past-paper questions.
6. Reveal answers one question at a time, never all at once.
7. Explain each answer in plain prose, with the keywords in bold.
8. Make all text on the page searchable.
9. Show the test and submission logistics from the announcement.
10. Show both versions of the test format and flag the conflict: "about 40 minutes" (announcement) against "60 questions in one hour" (assessment guidelines). Treat neither as confirmed, and leave the number of questions open.
11. Show both group-report deadlines and flag the conflict: Sun 22 Nov 2026, 23:59 (announcement) against 29 Nov 2026, 24:00 (assessment guidelines). Present the earlier one as the safe one until the lecturer confirms.
12. Show both sets of figures from the two drug-development charts and flag the difference without choosing one:
    - Week 3, page 22: Phase 2 has 100–500 volunteers and Phase 3 has 1,000–5,000;
    - Week 3, page 61: Phase 2 has 100–200 and Phase 3 has 1,000–6,000.
13. State that coverage is Weeks 1–3 only, and that the nine appendix topics are covered only as far as those slides go.
14. Include preparation for the lifeboat debate built on slide concepts: the four principles, fair allocation and triage, Rawls, the three ethical theories, Pragmatism and the trolley problem.
15. State that the slides do not describe the debate, and that the real scenario and roles are unknown until the night. Keep the debate preparation general enough for any role.
16. Label any lifeboat background taken from the outside reference as not from the slides.
17. Include preparation for the four group-report questions, together with the marking grid.
18. Explain "Moral Diversity" with the general outside meaning, labelled as not from the slides, and state that the slides do not define the term.

## 5. UI/UX requirements
- Light-coloured theme.
- Comfortable to read and operate on an iPad, by touch.
- One page with clearly separated parts: test logistics, revision notes by week, sample questions, debate preparation, group-report preparation.
- A search control that works across the whole page.
- Each sample question has its own control to reveal its answer and explanation.
- Conflict flags, "not from the slides" labels and "read from the slide picture" marks are visually distinct from ordinary notes.
- All text is in English.