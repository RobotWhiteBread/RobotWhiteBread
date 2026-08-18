# Aaron Price

**Founder, Anima Audire, LLC** — environmental data intelligence for agriculture, ecology, and natural resources.

I grew up working a Sand Hills cattle ranch, spent twelve years as a USDA NASS agricultural statistician, and now build AI-driven research pipelines from Lincoln, Nebraska. Fifteen-plus years of watching the Sandhill Crane migration on the Platte River is the field intuition underneath most of what's here.

📍 Lincoln, NE · 🎓 MPA, Columbia SIPA · UNL School of Natural Resources Research Affiliate
🔗 [LinkedIn](https://www.linkedin.com/in/aaron-price-983a208) · ✉️ aaronprice@ganimaaudire.com

---

## How I build

Every pipeline in this shop follows the same discipline, whether it's pointed at crane audio, plant taxonomy, or a million pages of government records:

- **Documentation first.** Governance docs are written before code and read before every session; architecture and methods docs live beside the pipeline, not after it.
- **No silent failures.** Every stage validates its inputs and outputs; anything unexpected halts loudly and gets logged.
- **Claims are audited.** Findings go into a claims registry and must survive negative controls, blind-lock validation, and release gates before anyone including me gets to believe them.
- **Platform over project.** One architecture, many domains. A component built for one pipeline has to justify itself as a generalizable pattern.

## Active work

Results from active research are deliberately **not** posted here — they're held for peer review and publication. What follows is what the systems do, not what they've found.

### 🎶 GRUS — Sandhill Crane bioacoustics
An end-to-end bioacoustic analysis pipeline for the Platte River crane migration: field recording, vocalization annotation (onsets/offsets, call types, liftoff events), feature extraction, and statistical analysis across a multi-million-frame audio corpus. Grounded in annotated field sessions at Rowe Sanctuary and a research partnership with the Crane Trust, with a public-listening installation concept ("Voices of the Platte") in development. Manuscripts in preparation.

### 🌿 GINGER — computational taxonomy
What began as the reproducible deep-learning taxonomy pipeline in [the public GINGER repo](https://github.com/RobotWhiteBread/GINGER) has grown into a full discovery-and-validation platform: multi-method feature extraction, statistical review, benchmark harnesses against public botanical datasets, and a defensibility layer (claims ledger, blind locks, negative controls, power analysis, release gates) built so that a taxonomic claim has to earn its way out of the pipeline. Applied casework is underway with university collaborators; results held for peer review.

### 🦆 WildEcho
An audio-coaching application that scores user-produced game calls against reference recordings — think music-lesson feedback loops, applied to waterfowl and wildlife calling. Built with the UNL Senior Design Program; presented at Techstars Founder Catalyst.

### 🛸📜 Document intelligence — NEXUS & ZodiacDeCode
The same pipeline architecture pointed at large public document corpora instead of audio:

- **NEXUS** ingests and analyzes the 2026 UAP records release — autonomous document acquisition, OCR and structured extraction into a relational schema, then spatial statistics, time-series decomposition, anomaly detection, and redaction-pattern analysis over the corpus.
- **ZodiacDeCode** applies archival cross-referencing and cipher-structure analysis to the Zodiac case's public record, including period government registers and the cipher corpus.

Both are exploratory research instruments. Hypotheses stay private until they're defensible.

## Stack

`Python` · `R` · `PyTorch` · `scikit-learn` · `librosa` · `Raven` · `pandas` · `Postgres/Parquet` · `Docker` · `GitHub Actions` · `AWS` · `SAS` · `SQL`

---
