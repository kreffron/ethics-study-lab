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
| Elevator Pitch Practice | The three questions, a quick check on the notes, a 3–5 minute timer, filler-word counter, and rubric self-score | Solo |

The elevator pitch station contains only class material and does not generate or suggest content, in keeping with the assignment's no-AI rule.

**Quick checks.** The Elevator Pitch and Virtue Case Lab stations can estimate a score from what a student wrote. The checks run in the browser with fixed rules (no AI). They note what is thin or missing, such as "Connect this answer to ideas from class" or "Raise a fair objection and respond to it," and never suggest what to write. They can't judge the quality of reasoning, so the estimate is not a grade.

### Unit 2: Virtue Ethics

| Station | What it practices | Mode |
| --- | --- | --- |
| Virtue Case Lab | The four-step case study method on twelve cases, including the four class practice cases, with model answers and a quick check that estimates the essay rubric | Step by step, pairs, or timed blue book |
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
| Class Jeopardy | Multiple Choice and review; three games plus Shuffle | Group or whole class |

## Direct links

Add these to the end of the site address to send students straight to a unit or station:

- The plain site address opens a landing page where students pick a unit.
- Units: `#unit1`, `#unit2`, `#unit3`
- Unit 1 stations: `#mlang`, `#mcalc`, `#mquiz`, `#mcode`, `#pitch`
- Unit 2 stations: `#vlab`, `#defs`, `#traits`, `#spot`, `#toolkit`
- Unit 3 stations: `#flashcards`, `#quiz`, `#sort`, `#mean`, `#ideas`, `#cases`, `#describe`
- Class Jeopardy is its own page: `jeopardy.html` (designed for a projector or shared screen)

Progress and written answers are saved in each student's own browser. Nothing is collected or sent anywhere.

## Notes-first locks and the teacher key

Some answers stay locked until students do their own work first, so the site supports note-taking instead of replacing it:

- **Flashcards (Units 1 and 3):** students write the definition from memory before a card flips. Once their attempt is in the right ballpark, that card stays unlocked. The Unit 1 glossary shows only unlocked terms.
- **Virtue Toolkit:** each virtue opens after the student writes its class definition and two essential characteristics.
- **Virtue Case Lab:** the model answer opens after the student writes enough for all four steps (in pairs mode, after the pair checks a box saying they wrote theirs).
- **Moral Calculus Lab, Key Ideas, and the Unit 3 Case Lab:** students write their reasoning before comparing with the model.
- **Definition Drill:** the class definition shows only after a real attempt.

The locks are a speed bump, not security: they run in the student's browser.

**Teacher key.** Nothing on the student pages links to it. Add `#teacher` to the end of the site address and enter the teacher code to open every lock on that device. While the key is on, a small line at the bottom of the landing page says so and offers "Turn off."

**Adjusting the locks.** In `index.html`, find `const GATES` near the bottom of the `<script>` section. Set `on: false` to turn every lock off, or change the word counts. The teacher code is stored only as a number (`teacherHash`), so the code itself is not in the page. To change it, open the site, open the browser console (F12), type `hashCode("YourNewCode")`, and paste the number it returns in place of the old `teacherHash` value. Capitalization does not matter.

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

Class Jeopardy has three complete games (Game 1, Game 2, Game 3) with the same six categories, plus a Shuffle option that builds each board square from a random one of the three games. The two Daily Doubles land in different random squares every new game. The clues are in `jeopardy.html`, near the top of its `<script>` section: `DATA` is Game 1, `GAME2` is Game 2, and `GAME3` is Game 3. Each clue has `q` (the clue), `a` (the correct response), and `n` (a teaching note), and each game has a `final` for Final Jeopardy. Keep the category names and their order the same in all three games so Shuffle lines up.

Theory codes: `ve` Virtue Ethics, `sct` Social Contract, `deon` Deontology, `util` Utilitarianism, `gen` across theories. Virtue codes: `pru` Prudence, `jus` Justice, `tem` Temperance, `for` Fortitude.

To edit, open `index.html` on GitHub, click the pencil icon, make your changes, and commit. The site updates within a minute or two.
