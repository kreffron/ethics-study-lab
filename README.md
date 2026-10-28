# Ethics Study Lab

Study games for the Ethics course, covering three units:

- **Unit 1: Foundations of Ethics**: the language of morality, the moral calculus, natural law, and the "Why Ethics?" elevator pitch
- **Unit 2: Virtue Ethics**: the four cardinal virtues and the four-step case study method
- **Unit 3: Normative Theories**: Virtue Ethics, Social Contract Theory, Deontology, and Utilitarianism

Students can use it on their own or in small groups, on a laptop or a phone. The site opens on a landing page where students pick a unit, and each unit page has a switch to the others.

## Stations

### Unit 1: Foundations of Ethics

| Station | What it practices | Mode |
| --- | --- | --- |
| Moral Language Flashcards | Unit 1 terms by topic, with where each returns in later units; filter to core moral language; glossary view | Solo |
| Moral Calculus Lab | Action + Intention + Circumstance = Moral Culpability, on ten cases | Solo or pairs |
| Moral Language Quiz | Definition matching plus applied questions, 15 per round | Solo |
| Build Your Moral Code | The six Week 4 questions, answered and saved by the student | Solo |
| Elevator Pitch Practice | The three questions, a 3–5 minute timer, filler-word counter, and rubric self-score | Solo |

The elevator pitch station contains only class material and does not generate or suggest content, in keeping with the assignment's no-AI rule.

### Unit 2: Virtue Ethics

| Station | What it practices | Mode |
| --- | --- | --- |
| Virtue Case Lab | The four-step case study method, with model answers | Step by step, pairs, or timed blue book |
| Definition Drill | The four cardinal virtue definitions (and virtue itself), matched and then written from memory | Solo |
| Characteristics Sort | The elements, vices, and roles of each cardinal virtue | Solo or pairs |
| Spot the Virtue | Naming the virtue at stake in short real-life moments | Solo or pairs |
| Virtue Toolkit | Reference page for all four virtues | Reference |

### Unit 3: Normative Theories

| Station | Test section | Mode |
| --- | --- | --- |
| Flashcards | Word Definitions (12 pts) | Solo |
| Practice Quiz | Multiple Choice (19 pts) | Solo |
| Theory Sort | Multiple Choice warm-up | Solo or pairs |
| Mean Builder | Key Ideas: Doctrine of the Mean | Solo |
| Key Ideas | Key Ideas (9 pts) and Short Answer (10 pts) | Solo |
| Case Lab | Case Study Analysis (10 pts) | Solo or group |
| Describe It | Word Definitions | Group (teams) |
| Class Jeopardy | Multiple Choice and review | Group or whole class |

## Direct links

Add these to the end of the site address to send students straight to a unit or station:

- The plain site address opens a landing page where students pick a unit.
- Units: `#unit1`, `#unit2`, `#unit3`
- Unit 1 stations: `#mlang`, `#mcalc`, `#mquiz`, `#mcode`, `#pitch`
- Unit 2 stations: `#vlab`, `#defs`, `#traits`, `#spot`, `#toolkit`
- Unit 3 stations: `#flashcards`, `#quiz`, `#sort`, `#mean`, `#ideas`, `#cases`, `#describe`
- Class Jeopardy is its own page: `jeopardy.html` (designed for a projector or shared screen)

Progress and written answers are saved in each student's own browser. Nothing is collected or sent anywhere.

## Publish with GitHub Pages

1. Create a new **public** repository on GitHub, for example `ethics-study-lab`.
2. Click **Add file → Upload files**, drag in `index.html`, `jeopardy.html`, and `README.md`, then click **Commit changes**.
3. Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the **main** branch and the **/ (root)** folder, and click **Save**.
4. After a minute or two, the site is live at `https://YOUR-USERNAME.github.io/ethics-study-lab/`.

## Editing the content

All of the content is near the top of the `<script>` section in `index.html`.

Unit 1:

- `MTERMS`: moral language terms. `c` is the topic, `core: 1` marks core moral language, and `r` is where the term returns in later units
- `MCQ`: the applied quiz questions (the first-listed option is not necessarily correct here; `a` gives the correct option's position, starting from 0)
- `MCALC`: moral calculus cases. In `m`, `a`/`i`/`c`/`k` are the model's choices for action, intention, circumstances, and culpability, counted from 0 in the option lists `ACTQ`, `INTQ`, `CIRQ`, `CULQ`
- `MCODE`: the six moral code questions and their help text
- `PITCH_QS` and `PITCH_RUBRIC`: the elevator pitch questions, self-check prompts, and rubric

Unit 2:

- `VIRTUES`: each cardinal virtue's definition, essential characteristics, vices, notes, and quotes
- `VCASES`: case studies and their model answers (Step 1 issues and stakeholders, Step 2, Step 3, Step 4)
- `RECALL`: the definitions students write from memory, and the key words the checker looks for
- `TRAITS`: Characteristics Sort items and the virtue each belongs to
- `SPOTS`: Spot the Virtue moments and their explanations
- `RUBRIC`: the self-check list shown after a case study

Unit 3:

- `TERMS`: flashcard terms, definitions, and the "don't say" words for Describe It
- `QUIZ`: multiple-choice questions. The first option listed is the correct one; the order is shuffled when students play.
- `SORT`: Theory Sort phrases and their theories
- `MEAN`: Doctrine of the Mean rows (deficiency, virtue, excess)
- `IDEAS`: key ideas with a model definition, explanation, and example
- `CASES`: case studies with the key moral issue and model responses for each stance

Jeopardy clues are in `jeopardy.html`, in the `DATA` object near the top of its `<script>` section. Each clue has `q` (the clue), `a` (the correct response), and `n` (a teaching note). The two Daily Doubles are set in the `DAILY` line just below it.

Theory codes: `ve` Virtue Ethics, `sct` Social Contract, `deon` Deontology, `util` Utilitarianism, `gen` across theories. Virtue codes: `pru` Prudence, `jus` Justice, `tem` Temperance, `for` Fortitude.

To edit, open `index.html` on GitHub, click the pencil icon, make your changes, and commit. The site updates within a minute or two.
