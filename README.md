# Aaron Price

**Founder, Anima Audire, LLC.** Environmental data intelligence for agriculture, ecology, and natural resources.

I grew up working a Sand Hills cattle ranch, spent twelve years as a USDA NASS agricultural statistician, and now build AI-driven research pipelines from Lincoln, Nebraska. Fifteen-plus years of watching the Sandhill Crane migration on the Platte River is the field intuition underneath most of what's here. I bring the thing most data and computer-science engineers lack: a working life in the natural world. My specialty is seeing data where others don't: audio, archives, imagery, field notes, regulatory paperwork. If your group has questions and no data arm, that is the gap I like to fill.

Lincoln, NE · MPA, Columbia SIPA · Research Affiliate, UNL School of Natural Resources
[LinkedIn](https://www.linkedin.com/in/aaron-price-983a208) · aaron.price.unl@gmail.com

---

## How I build

Every pipeline in this shop follows the same discipline, whether it's pointed at crane audio, plant taxonomy, or a million pages of government records:

- **Documentation first.** Governance docs are written before code and read before every session; architecture and methods docs live beside the pipeline, not after it.
- **No silent failures.** Every stage validates its inputs and outputs; anything unexpected halts loudly and gets logged.
- **Claims are audited.** Findings go into a claims registry and must survive negative controls, blind-lock validation, and release gates before anyone, including me, gets to believe them.
- **Platform over project.** One architecture, many domains. A component built for one pipeline has to justify itself as a generalizable pattern.

## Active work

Results from active research are deliberately **not** posted here; they are held for peer review and publication. What follows is what the systems do, not what they've found.

### GRUS: Sandhill Crane bioacoustics
An end-to-end bioacoustic analysis pipeline for the Platte River crane migration: field recording, vocalization annotation (onsets/offsets, call types, liftoff events), feature extraction, and statistical analysis across a multi-million-frame audio corpus. Grounded in annotated field sessions at Rowe Sanctuary, with a public-listening installation concept ("Voices of the Platte") in development. Manuscripts in preparation. A small public demo of the basic annotation workflow, run on an openly licensed recording, lives in [crane-annotation-demo](https://github.com/RobotWhiteBread/crane-annotation-demo).

### GINGER: computational taxonomy
What began as the reproducible deep-learning taxonomy pipeline in [the public GINGER repo](https://github.com/RobotWhiteBread/GINGER) has grown into a full discovery-and-validation platform: multi-method feature extraction, statistical review, benchmark harnesses against public botanical datasets, and a defensibility layer (claims ledger, blind locks, negative controls, power analysis, release gates) built so a taxonomic claim has to earn its way out of the pipeline. Applied casework is underway with university collaborators; results held for peer review.

### WildEcho
An audio-coaching application that scores user-produced game calls against reference recordings: music-lesson feedback loops applied to waterfowl and wildlife calling. Built with the UNL Senior Design Program; presented at Techstars Founder Catalyst.

### Document intelligence: NEXUS and ZodiacDeCode
The same pipeline architecture pointed at large public document corpora instead of audio.

- **NEXUS** ingests and analyzes the 2026 UAP records release: autonomous document acquisition, OCR and structured extraction into a relational schema, then spatial statistics, time-series decomposition, anomaly detection, and redaction-pattern analysis over the corpus.
- **ZodiacDeCode** applies archival cross-referencing and cipher-structure analysis to the Zodiac case's public record, including period government registers and the cipher corpus.

Both are exploratory research instruments. Hypotheses stay private until they're defensible.

## Tools

Two pieces of the working method, generalized and published on their own:

- **[research-defensibility-kit](https://github.com/RobotWhiteBread/research-defensibility-kit)** is the claims-and-gates harness described above, extracted from the research pipelines and made domain-neutral. A claims registry, fail-closed release gates, blind locks for holdout sets, and negative controls. Runs in CI.
- **[field-data-utils](https://github.com/RobotWhiteBread/field-data-utils)** handles the messy first hour with a new data drop: content hashing and manifests, duplicate detection by content rather than name, and filename checks that catch the problems which surface three weeks later.

## Stack

`Python` · `R` · `PyTorch` · `scikit-learn` · `librosa` · `Raven` · `pandas` · `Postgres/Parquet` · `Docker` · `GitHub Actions` · `AWS` · `SAS` · `SQL`

---

*Code and results land here as they clear validation and peer review. If you're working on conservation data, bioacoustics, or environmental data infrastructure, or your team has the questions but not the data arm, reach out.*
