# 📓 Personal Reflection — Data Analytics with Python (SECP3233)
---

## Assignment 2 — Retail Sales Analysis with Pandas & MultiIndexing

### Reflection

This assignment reinforced my understanding of how pandas organizes hierarchical data. Setting a three-level MultiIndex across `Region`, `City`, and `Category` and then slicing it using `.xs()` was something I had not done confidently before — it made me realize how useful MultiIndexing is when navigating complex datasets without losing structure.

The `Performance` column in Question 3 was also a good reminder of how `apply()` and simple conditional logic translate to real-world labeling tasks, which is essentially what feature engineering often looks like in practice.

One honest challenge: the MultiIndex filtering in Question 2.2 initially used `|` (OR) instead of `&` (AND), which produced wider results than expected. Catching that kind of subtle logic error matters a lot because wrong filtering silently produces plausible-looking but incorrect output.

Working with a small, controlled dataset was actually very useful at this stage. It forced me to understand the operations clearly before scaling up. If I were to redo this, I would have added a second month to the dataset to make the temporal filtering in Question 5.2 more meaningful and realistic.

---

## Assignment 3 — Rainfall Data Analysis

### Reflection

The data loading step in this assignment was unexpectedly instructive. The CSV required parsing the first column as a delimited string (`str.split(',', expand=True)`) and manually reassigning column names — something that happens frequently when working with exported or malformed files in the real world. It was a reminder that data rarely arrives clean.

The groupby operations became increasingly layered throughout Part 2, moving from single-column aggregation (per station) to multi-key combinations (Month × Region) with multi-function `.agg()`. Structuring the code cleanly at each level required deliberate thinking about what question was being answered and what granularity the output needed to be.

Part 3 — the visualization section — highlighted a skill gap I want to actively close. While I understand the syntax for each chart type, designing visualizations that actually communicate something meaningful requires more than correct code. Choosing appropriate color schemes, annotating key data points, and deciding when a boxplot versus a scatter plot is more honest to the data are judgment calls that develop through practice, not just instruction.

The bonus section asked us to annotate plots and write a data insight summary, which I think is the most transferable skill in the whole assignment — being able to look at an aggregation result and articulate what it actually means in plain language. I would invest more time here if I repeated this assignment. Technical accuracy matters, but the ability to narrate findings is what makes analysis useful.

---

## Group Project — Vehicle CO₂ Emissions Analysis

### Reflection

This project taught me that data analytics is not a linear process. We revisited the data cleaning step multiple times as the ML phase revealed issues — outlier rows in CO₂ emissions exceeding 600 g/km, for instance, were only filtered when they started distorting visualizations and model predictions. Good data preparation is iterative, not a one-time step at the start.

Working as a group also showed me the importance of consistent conventions early on. When teammates work independently on different phases, small inconsistencies in column naming or data types can cause downstream errors that take time to trace. Establishing a shared data contract at the start of a project would have saved us some debugging time.

---

## Overall Takeaways

Across all these tasks, a few themes stand out clearly:

The gap between writing correct code and doing good analysis is real and significant. Code can be syntactically valid and logically flawed, or technically correct but poorly communicated. I want to get better at being intentional — choosing the right aggregation, the right chart, the right model — not just the one I know how to implement.

I also want to become more comfortable with the full stack of a data project: from messy raw files, through cleaning and transformation, to visualization and finally to the kind of narrative summary that makes results useful to someone who did not run the code. Each of those stages requires a different kind of thinking, and I am still developing fluency in all of them.

These assignments have been a meaningful foundation. The work gets harder and more open-ended as the datasets grow and the questions become less structured — and that is exactly the direction I want to keep moving in.

---


