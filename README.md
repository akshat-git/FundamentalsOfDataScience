# FundamentalsOfDataScience
Fundamentals Of Data Science - West Valley College course

## Notebooks & Activities

- `Week1/Math 80 Lab Week 1.ipynb`: `Lab 1` — learn how to work with Jupyter notebooks (text vs. code cells, kernels) and evaluate basic Python `expressions` (numbers and arithmetic).
- `Week1/Math 80 HW Week 1-1.ipynb`: `Homework 1: Causality and Expressions` — complete exercises on expressions and related scenarios, including `Scary Arithmetic`, `Characters in Little Women`, `Names and Assignment Statements`, `Differences Between Majors`, `Nearsightedness Study`, and `Studying the Survivors`.

## Week 2 — implementation (`Week2/`)

Week 2 centers on **NumPy-style arrays**, the **`datascience`** package **`Table`**, and loading **CSV** data with `Table.read_table`.

### Lab notebooks

- **`Week2/Math 80 Lab Week  2.ipynb`** (`Lab 2: Table Operations`): Reviews Python building blocks and importing libraries, then implements **`Table` inspection and manipulation** on real data: `num_columns`, `num_rows`, `select`, `drop`, `sort`, and `where`. The primary dataset is **`farmers_markets.csv`** (USDA farmers’ markets, one row per market). The notebook also includes exercises that load **`imdb.csv`** when that file is available locally.
- **`Week2/Math 80 Lab week 2 Sample.ipynb`**: Same lab structure with **worked / example paths** (often absolute paths under a user `Downloads` folder); use the main lab notebook for **relative paths** next to the CSV in `Week2/`.

### Homework notebooks

- **`Week2/Math 80 HW Week  2.ipynb`** (`Homework 2: Arrays and Tables`): Implements **`make_array`**, array **creation**, **indexing**, and **elementwise arithmetic**; uses **`np.round`**, **`np.diff`**, and **string `join`** on arrays; converts **Fahrenheit to Celsius** on temperature arrays; analyzes **Old Faithful** waiting times from **`old_faithful.csv`** and related **`eruptions.csv`**; builds and combines **`Table`** objects for a **fruit stand** scenario using **`inventory.csv`** and **`sales.csv`**; loads **`president_births.csv`** for table practice.
- **`Week2/Math 80 HW Week  2 sample.ipynb`**: Same homework with **filled-in sample answers** and **absolute file paths** in places; pair with the blank HW notebook for submission vs. reference.

### Data files in `Week2/`

| File | Role |
|------|------|
| `farmers_markets.csv` | Lab — USDA farmers’ markets |
| `president_births-1.csv`, `old_faithful-1.csv`, `inventory-1.csv`, `sales-1.csv` | Homework sources (notebooks expect names **`president_births.csv`**, **`old_faithful.csv`**, **`inventory.csv`**, **`sales.csv`** — rename or adjust paths as needed) |
| `temperatures.csv` | Daily max/min Fahrenheit columns (supports temperature-style exercises) |
| `world_population.csv` | Yearly population series (extra dataset in the folder) |

**Note:** Some assignments reference **`imdb.csv`** or **`eruptions.csv`**, which are **not** in this folder by default; add those files next to the notebook or update `Table.read_table(...)` paths when you run those cells.

## Week 3 — implementation (`Week3/`)

Week 3 builds on **`Table`** workflows with **strings**, **NumPy arrays**, and richer table methods. **`Week3/Math 80 Lab Week 3 -1.ipynb`** (`Lab 3: Data Types and Arrays`) covers string methods and conversions, array creation with **`np.arange`**, indexing and elementwise arithmetic, building tables with **`with_columns`**, and operations such as **`column`**, **`take`**, **`where`** (with **`are`** predicates), and **`mean`**—using **`world_population.csv`**, **`imdb.csv`**, and **`more_restaurant_bills.csv`**. **`Week3/Math 80 HW Week 3.ipynb`** (`Homework 3: Table Manipulation and Visualization`) loads **`unemployment.csv`** for sorting, derived columns, and line plots over time; filters and relabels Census-style population data for birth/migration analysis; and plots ride-time distributions from **`boston.csv`** and **`manila.csv`** with **matplotlib** histograms, then interprets histogram shape and median bins. Sample notebooks (**`Math 80 Lab Week 3 sample.ipynb`**, **`Math 80 HW Week 3 Sample.ipynb`**) mirror the same work with filled answers and often absolute file paths. Homework section 2 expects **`nst-est2016-alldata.csv`**, which is not bundled in this folder—add it locally or adjust paths before running those cells.

## Week 4 — implementation (`Week4 - Exam 1/`)

Week 4 is organized as **Exam 1** in **`Week4 - Exam 1/`**, with a single notebook **`exam1.ipynb`** that shifts from the course **`datascience`** `Table` API to **pandas** for tabular work. The implementation loads the Museum of Modern Art collection from **`Artworks MOMA-1-1-1.csv`** (with **`ISO-8859-1`** encoding), then cleans the dataset by dropping rows with missing **`Title`**, **`Artist`**, or **`DateAcquired`**. It filters the **`Photography`** department to count works and compute their **percentage** of the cleaned collection. Additional analysis uses **boolean indexing** and **string methods** (`str.contains`, case-insensitive) to count **untitled** works, and to compare how often **`paper`** vs. **`canvas`** appear in the **`Medium`** column (ratio of counts). The CSV is referenced by the notebook but is **not** included in this repository—place the file next to **`exam1.ipynb`** or update the path before running the cells.

## Week 5–6 — implementation (`Week5-6/`)

Weeks 5–6 focus on **probability, simulation, and hypothesis testing** with **`datascience`** tables and NumPy random tools. **`Week5-6/Math 80 Lab Week 6.ipynb`** (`Lab 6: Examining the Therapeutic Touch`) uses **`sample_proportions`** to simulate coin flips and Emily Rosa’s 210 hand-guess trials, runs repeated simulations with custom functions, and compares an observed statistic to a null distribution via histograms and tail-area **p-value** reasoning. **`Week5-6/Math 80 HW week 6.ipynb`** (`Homework 6: Probability, Simulation, Estimation, and Assessing Models`) simulates **roulette** outcomes from **`roulette_wheel-1-1.csv`**, contrasts **`Table.sample`**, **`np.random.choice`**, and **`sample_proportions`**, and tests **Jade’s card-deck model** with thousands of simulated draws. Practice notebooks **`simpractice.ipynb`** (pandas sampling on **`top_movies_2017-1-1.csv`**, word counts from **`Austen_PrideAndPrejudice-1-1.txt`**) and **`classes.ipynb`** (pandas/plotly on **`united_summer2015-1-1.csv`**, delay histograms with mean, median, and percentiles) extend the same ideas. Sample lab and homework notebooks mirror the main work with filled answers; several CSVs use **`*-1-1`** filenames—rename or adjust paths to match what each notebook expects.

## Week 7 — implementation (`Week7/`)

Week 7 extends **hypothesis testing** with simulation-based **p-values**, **total variation distance (TVD)**, and **permutation tests**. **`Week7/HW week 7.ipynb`** (`Homework 7: Testing Hypotheses`) simulates a vaccination coin-flip null model with **`sample_proportions`**, compares the observed Vaccine 1 share to 60%, and computes an empirical **p-value** from a null histogram. Section 2 loads **`happiness_scores-1-1.csv`** and **`us_happiness_factors-1-1.csv`**, implements **`calculate_tvd`** to compare observed vs. expected happiness-factor distributions, and runs 10,000 simulated TVDs to assess whether US factor proportions match a null model. Section 3 uses **`age-1-1.csv`** for a **permutation test** on gender labels, shuffling male/female assignments and comparing average age differences to test whether sampled males are older than females. **`Week7/HT Practice.ipynb`** and **`Week7/classes.ipynb`** rehearse the same ideas (vaccination null distributions, jury **`sample_proportions`** simulations). **`Week7/HW week 7 Sample.ipynb`** provides filled answers; saved plots include **`null_distribution_histogram.png`**, **`simulated_tvds.png`**, and **`simulations_age_diff.png`**.

## Week 8 — implementation (`Week8/`)

Week 8 focuses on **A/B testing** (permutation tests): comparing two groups under a null hypothesis by **shuffling labels**, using the **difference in means** as a test statistic, and estimating **empirical p-values** from thousands of simulations. **`Week8/Lab Week 7.ipynb`** (`Lab 7: Great British Bake Off`) loads **`star_bakers-1.csv`** and tests whether winners and non-winners differ in **Star Baker** awards, with a reusable shuffle-and-statistic workflow and 5,000 simulated label permutations. **`Week8/DS- AB Testing part 1.ipynb`** and **`Week8/DS- AB Testing part 2.ipynb`** apply the same method to **`baby-2.csv`**, comparing **birth weight** and **maternal age** between smokers and non-smokers via grouped histograms, `difference_of_means`, and repeated shuffles of the **`Maternal Smoker`** label. **`Week8/DS- Causality.ipynb`** ties permutation tests to **causality and randomized controlled trials**, running **`permutation_test_means`** on infant birth weights and on **`bta-1.csv`** (treatment vs. control back-pain outcomes) to contrast association with causal claims under random assignment. Part 2 still references **`baby.csv`** in one cell—use **`baby-2.csv`** locally or update the path before running.
