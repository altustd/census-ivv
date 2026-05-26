# US Census IV&V

*Independent Verification of Census Bureau Data Releases*

Occasional spot-checks of Census Bureau press release figures against raw microdata and the Census API. Each note verifies a headline claim, documents the API call that reproduces it, and logs observations about what the underlying data product can do beyond the press release.

The series doubles as a running tour of the Census API — what endpoints exist, what variables they expose, what geographic granularity is available, and what follow-on analyses are worth pursuing.

---

## Read Online

**[https://altustd.github.io/census-ivv/](https://altustd.github.io/census-ivv/)**

---

## Notes

| # | Release | Survey | Status |
|---|---------|--------|--------|
| 1 | 2024 Education Enrollment | CPS October | In progress |

---

## Run Locally

```bash
pixi install
pixi run render       # HTML → docs/
pixi run render-pdf   # PDF  → docs/
pixi run preview      # live preview
```

## API Key

Requires a Census Bureau API key (free): [api.census.gov/data/key_signup.html](https://api.census.gov/data/key_signup.html)

Key should be available as environment variable `CENSUS_API_KEY`.

## Tech Stack

Quarto · pixi · Python (pandas, requests, plotly)
