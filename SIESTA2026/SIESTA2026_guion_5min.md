# SIESTA 2026 — guion de 5 minutos

Presentación: `SIESTA2026_Alegre.bento.html`
Idioma recomendado: inglés
Objetivo: presentar una trayectoria doctoral coherente y terminar solicitando feedback sobre las líneas futuras.

## Diapositiva 1 — Cover (0:00–0:25)

Good afternoon. I’m Ricardo Hidalgo-Aragón, from Universidad Rey Juan Carlos. My research began by asking how we can measure novice programming competence from code. My thesis studied this at scale, using more than two million public Scratch projects. Now this path leads to a new question: what changes when part of the code is written by a machine?

[Avanza a la diapositiva 2]

## Diapositiva 2 — The roadmap (0:25–0:55)

I will describe this path in four moves. First, diagnose where learning stalls. Second, explain a diagnosis so that it becomes useful feedback. Third, build an instrument that separates genuine quality from a major confounder: project size. And fourth, use that representation to investigate authorship—human, AI, or mixed. These are not four disconnected projects. They all ask where size ends and meaningful structure begins.

[Avanza a la diapositiva 3]

## Diapositiva 3 — The thesis (0:55–2:35)

The thesis produced three connected diagnoses.

First, programming competence can be assessed at scale. Using fuzzy clustering, I organized Scratch projects into six CEFR-inspired levels, from A1 to C2, while preserving uncertainty. The distribution revealed a bottleneck around B2: only 13.3 percent of the projects were assigned to that level.

Second, competence is not the same as good software design. We compared nine dimensions of computational thinking with thirty-four code smells. Their apparent association was minus point three four two, but 95.9 percent of that association was mediated by project size. In other words, larger projects can look both more competent and more problematic. If size is not controlled, we may mistake volume for skill—or for poor design.

Third, procedural abstraction appears to be a key gate. Duplicated code persists at every level, even among advanced learners. But most frequent clones are abstractable: eighty-three of the hundred most common clones already appear as custom blocks in other projects, and manual inspection found that fifteen of the remaining seventeen were also readily abstractable.

So the thesis does not support a single-cause story. The evidence converges on several interacting explanations—project size, design choices, and the cost of abstraction. That is why the final studies use retrospective quasi-experiments rather than treating correlation as causation.

[Avanza a la diapositiva 4]

## Diapositiva 4 — Beyond the thesis (2:35–4:40)

This leads to the work I am developing now.

The first direction is explanation. A label such as “B1” is not yet useful feedback. A learner or teacher needs to know why the project received that assessment and what realistic change could move it forward. Experts should then judge whether the explanation is faithful, understandable, and actionable.

The second direction is instrumentation. I am exploring a conditional variational autoencoder in which project size is an explicit condition. The goal is to learn a representation where variation due to size is separated, as far as the evidence allows, from variation associated with quality. This is not a magic causal solution. It is a reusable measurement instrument that can make later comparisons more honest and testable.

The third direction asks: who wrote the code? Existing detectors often assume that a program is entirely human- or entirely AI-generated. Real development is messier: a human may create the structure, an LLM may complete part of it, and the human may then revise the result. Mixed authorship is therefore the critical blind spot.

My working hypothesis is not that there is one universal AI fingerprint. It is that some structural signals may survive editing and partial collaboration better than surface-level style. The challenge is to test that hypothesis without simply rediscovering project size, language, task, or developer experience.

Across these directions, the principle is the same: control the confounder, quantify uncertainty, and retain a qualitative layer so that the measurement remains trustworthy.

[Avanza a la diapositiva 5]

## Diapositiva 5 — Closing (4:40–5:00)

To close, I would value your feedback on one question: what evidence would you trust to distinguish human, AI, and mixed-authorship code without penalizing larger projects? Thank you. I’m happy to discuss the methods, datasets, or possible collaborations during SIESTA.

## Ensayo y entrega

- Ensaya a un ritmo conversacional, no acelerado.
- Haz una pausa breve después de “project size” en las diapositivas 2 y 3: es el hilo conductor.
- En la diapositiva 3, enfatiza solo tres cifras: **2 million**, **95.9%** y **83 + 15**.
- Si vas con retraso, omite la frase sobre “minus point three four two” y conserva el 95.9%.
- Si vas con adelanto, no añadas otro resultado: amplía la pregunta final y mira al público.
- No presentes la detección de autoría como un resultado logrado; descríbela como hipótesis y línea futura.
