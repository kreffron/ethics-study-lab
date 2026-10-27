# Ethics Study Lab

Study games for the Ethics unit test, covering Virtue Ethics, Social Contract Theory, Deontology, and Utilitarianism. Students can use it on their own or in small groups, on a laptop or a phone.

## Stations

| Station | Test section | Mode |
| --- | --- | --- |
| Flashcards | Word Definitions (12 pts) | Solo |
| Practice Quiz | Multiple Choice (19 pts) | Solo |
| Theory Sort | Multiple Choice warm-up | Solo or pairs |
| Mean Builder | Key Ideas: Doctrine of the Mean | Solo |
| Key Ideas | Key Ideas (9 pts) and Short Answer (10 pts) | Solo |
| Case Lab | Case Study Analysis (10 pts) | Solo or group |
| Describe It | Word Definitions | Group (teams) |

Each station has its own link, for example `.../#quiz` or `.../#cases`, so you can send students straight to one activity.

Progress (known flashcards, best quiz score, and so on) is saved in each student's own browser. Nothing is collected or sent anywhere.

## Publish with GitHub Pages

1. Create a new **public** repository on GitHub, for example `ethics-study-lab`.
2. Click **Add file → Upload files**, drag in `index.html` and `README.md`, then click **Commit changes**.
3. Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the **main** branch and the **/ (root)** folder, and click **Save**.
4. After a minute or two, the site is live at `https://YOUR-USERNAME.github.io/ethics-study-lab/`.

## Editing the content

All of the questions and answers are near the top of the `<script>` section in `index.html`:

- `TERMS`: flashcard terms, definitions, and the "don't say" words for Describe It
- `QUIZ`: multiple-choice questions. The first option listed is the correct one; the order is shuffled when students play.
- `SORT`: Theory Sort phrases and their theories
- `MEAN`: Doctrine of the Mean rows (deficiency, virtue, excess)
- `IDEAS`: key ideas with a model definition, explanation, and example
- `CASES`: case studies with the key moral issue and model responses for each stance

Theory codes: `ve` Virtue Ethics, `sct` Social Contract, `deon` Deontology, `util` Utilitarianism, `gen` across theories.

To edit, open `index.html` on GitHub, click the pencil icon, make your changes, and commit. The site updates within a minute or two.
