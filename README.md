# Aaron Price

**Founder, Anima Audire, LLC.** Environmental data intelligence for agriculture, ecology, and natural resources.

I grew up working a Sand Hills cattle ranch, spent twelve years as a USDA NASS agricultural statistician, and now build AI-driven research pipelines from Lincoln, Nebraska. Fifteen-plus years of watching the Sandhill Crane migration on the Platte River is the field intuition underneath most of what's here. I bring the thing most data and computer-science engineers lack: a working life in the natural world. My specialty is seeing data where others don't: audio, archives, imagery, field notes, regulatory paperwork. If your group has questions and no data arm, that is the gap I like to fill.

Lincoln, NE
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

### [GRUS](https://github.com/RobotWhiteBread/GRUS): crane bioacoustics
An active research program on North American crane vocalizations, covering the full path from original field recording through annotation to analysis. Methods and results are held for peer review and deliberately not described in detail here. A small public demo of the general annotation workflow, built on openly licensed audio and textbook methods, lives in [crane-annotation-demo](https://github.com/RobotWhiteBread/crane-annotation-demo).

### GINGER: computational taxonomy
What began as the reproducible deep-learning taxonomy pipeline in [the public GINGER repo](https://github.com/RobotWhiteBread/GINGER) has grown into a full discovery-and-validation platform: multi-method feature extraction, statistical review, benchmark harnesses against public botanical datasets, and a defensibility layer (claims ledger, blind locks, negative controls, power analysis, release gates) built so a taxonomic claim has to earn its way out of the pipeline. Applied casework is underway with university collaborators; results held for peer review.

### WildEcho
An audio-coaching application that scores user-produced game calls against reference recordings: music-lesson feedback loops applied to waterfowl and wildlife calling. Built with the UNL Senior Design Program; presented at Techstars Founder Catalyst.

### Document intelligence: [NEXUS](https://github.com/RobotWhiteBread/NEXUS) and [ZodiacDeCode](https://github.com/RobotWhiteBread/ZodiacDeCode)
The same architecture pointed at large public document corpora instead of audio. A bulk records release is a dataset, not a reading assignment, and measurement scales in a way close reading does not.

Both are exploratory instruments in private development. Methods and findings are not published, and hypotheses stay private until they are defensible. ZodiacDeCode in particular concerns a case with real victims and real families; it names no persons of interest, now or later.

## Tools

Two pieces of the working method, generalized and published on their own:

- **[research-defensibility-kit](https://github.com/RobotWhiteBread/research-defensibility-kit)** is the claims-and-gates harness described above, extracted from the research pipelines and made domain-neutral. A claims registry, fail-closed release gates, blind locks for holdout sets, and negative controls. Runs in CI.
- **[field-data-utils](https://github.com/RobotWhiteBread/field-data-utils)** handles the messy first hour with a new data drop: content hashing and manifests, duplicate detection by content rather than name, and filename checks that catch the problems which surface three weeks later.

## Stack

`Python` · `R` · `PyTorch` · `scikit-learn` · `librosa` · `pandas` · `Postgres/Parquet` · `Docker` · `GitHub Actions` · `AWS` · `SAS` · `SQL`

---

*Code and results land here as they clear validation and peer review. If you're working on conservation data, bioacoustics, or environmental data infrastructure, or your team has the questions but not the data arm, reach out.*
