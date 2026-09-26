# frozenjune.github.io
About me

# Analysis: City of Vancouver Homeless Shelter
 Here are two blog posts analyzing the City of Vancouver Homeless Shelter Locations dataset: one analysis using Python and one using R.

## Requirements
The website requires:
- Quarto
- uv
- Python 3.14
- R 4.6
- renv

Python dependencies are recorded in `pyproject.toml` and `uv.lock`.
R dependencies are recorded in `renv.lock`.

## Build the Website
Clone the repository:

```bash
git clone https://github.com/frozenjune/frozenjune.github.io.git
cd frozenjune.github.io
```

Install the Python environment:
```bash
uv sync
```
Restore the R environment:
```bash
R
```

Then, inside R:
```r
renv::restore()
q()
```

Render the website:
```bash
uv run quarto render
```

The rendered website is created in the `docs/` directory. Open `docs/index.html` in a web browser to view the local website.

## Data Source
The computational posts use the City of Vancouver Open Data Portal **Homeless Shelter Locations** dataset.

The dataset is included in the repository in the `data/` directory, so an internet connection is not required to access the data when rebuilding the website.

**Licence:** Open Government Licence - Vancouver

**Source:** https://opendata.vancouver.ca/explore/dataset/homeless-shelter-locations/