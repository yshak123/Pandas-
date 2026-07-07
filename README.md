# Pandas Revision

A hands-on, runnable revision notebook covering core-to-intermediate **pandas** for data
analysis — built for fresher/graduate-level interview prep, but useful as a general reference
too.

Every cell has a one-line explanation above it, the code is bug-fixed and tested end-to-end,
and all sample data is bundled locally, so the whole notebook runs anywhere (no Google Colab
paths required).

## Contents

`Pandas_Revision.ipynb` walks through:

1. NumPy & Series basics
2. DataFrame basics & inspection (`head`, `info`, `describe`, `dtypes`, ...)
3. Selecting data — `.loc`, `.iloc`, `.at`, `.iat`
4. Sorting & iterating
5. Filtering — boolean conditions, string ops, regex, `.query()`
6. Adding / removing / transforming columns
7. Datetime operations
8. Custom logic with `.apply()` and lambdas
9. Merging & concatenating data
10. Handling missing values (`fillna`, `interpolate`, `dropna`)
11. Aggregating data — `value_counts`, `groupby`, `.agg()`, pivot tables
12. Duplicates & replacing values, `pd.crosstab()`
13. Window functions — `rolling`, `expanding`, `shift`, `diff`
14. Method chaining with `.pipe()`
15. Performance notes — `.iterrows()` vs vectorization, `category` dtype
16. Quick plotting with `.plot()`
17. Summary & next steps

## Getting started

```bash
git clone <this-repo-url>
cd pandas-revision
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter notebook Pandas_Revision.ipynb
```

## Project structure

```
pandas-revision/
├── Pandas_Revision.ipynb   # the main notebook
├── data/                   # small sample CSVs used throughout the notebook
│   ├── pokemon_data.csv
│   ├── bios.csv
│   ├── coffee.csv
│   └── noc_regions.csv
├── requirements.txt
├── .gitignore
└── README.md
```

## Notes

- Sample datasets are small, synthetic stand-ins (a handful of Pokémon, athlete bios, and
  coffee sales rows) — enough to demonstrate every operation without needing an external
  download.
- Cells that write files put output into an `output/` folder (git-ignored) so the repo stays
  clean.
