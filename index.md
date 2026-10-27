---
title: openalexPro
description: An R ecosystem for large-scale, on-disk access to OpenAlex
---

# openalexPro

An R ecosystem for large-scale, on-disk access to [OpenAlex](https://openalex.org) — the open catalogue of global scholarly work.

OpenAlex provides free, comprehensive metadata on over 250 million scholarly works, authors, institutions, and concepts. The **openalexPro** ecosystem is built around a single design principle: process data on disk rather than in memory, so workflows scale to millions of records without hitting RAM limits.

## Packages

**Version:** `r-universe` is the released version, which `install.packages()` gives you (built from `main`); `main` and `dev` are the versions in each branch's `DESCRIPTION`, read live from GitHub. **Checks:** R CMD check and test coverage of `main`.

<style>
/* badges keep their natural size; only the description column wraps */
.main-content table td img { max-width: none; }
.main-content table td:not(:nth-child(2)) { white-space: nowrap; }
</style>

<table>
<thead>
<tr><th>Package</th><th>Description</th><th>Version</th><th>Checks</th></tr>
</thead>
<tbody>
<tr>
  <td><a href="https://github.com/openalexPro/openalexPro"><strong>openalexPro</strong></a><br><a href="https://openalexpro.github.io/openalexPro/"><img src="https://img.shields.io/badge/docs-📖-blue" alt="Docs"></a><br><a href="https://doi.org/10.5281/zenodo.17453180"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.17453180.svg" alt="DOI"></a></td>
  <td>Core API client — build queries (classic filters or OpenAlex's query language, OQL), page through the results, and store them as Parquet; resumes interrupted downloads</td>
  <td><a href="https://openalexpro.r-universe.dev/openalexPro"><img src="https://openalexpro.r-universe.dev/openalexPro/badges/version" alt="r-universe version"></a><br><a href="https://github.com/openalexPro/openalexPro/tree/main"><img src="https://img.shields.io/github/r-package/v/openalexPro/openalexPro/main?label=main" alt="main version"></a><br><a href="https://github.com/openalexPro/openalexPro/tree/dev"><img src="https://img.shields.io/github/r-package/v/openalexPro/openalexPro/dev?label=dev" alt="dev version"></a></td>
  <td><a href="https://github.com/openalexPro/openalexPro/actions/workflows/R-CMD-check.yaml"><img src="https://img.shields.io/github/actions/workflow/status/openalexPro/openalexPro/R-CMD-check.yaml?label=CI" alt="CI"></a><br><a href="https://app.codecov.io/gh/openalexPro/openalexPro"><img src="https://codecov.io/gh/openalexPro/openalexPro/graph/badge.svg" alt="Codecov"></a></td>
</tr>
<tr>
  <td><a href="https://github.com/openalexPro/openalexSnowball"><strong>openalexSnowball</strong></a><br><a href="https://openalexpro.github.io/openalexSnowball/"><img src="https://img.shields.io/badge/docs-📖-blue" alt="Docs"></a><br><a href="https://doi.org/10.5281/zenodo.20448982"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.20448982.svg" alt="DOI"></a></td>
  <td>Snowball citation searches — expand seed papers by the works citing them and the works they cite, live via the API or offline against a snapshot</td>
  <td><a href="https://openalexpro.r-universe.dev/openalexSnowball"><img src="https://openalexpro.r-universe.dev/openalexSnowball/badges/version" alt="r-universe version"></a><br><a href="https://github.com/openalexPro/openalexSnowball/tree/main"><img src="https://img.shields.io/github/r-package/v/openalexPro/openalexSnowball/main?label=main" alt="main version"></a><br><a href="https://github.com/openalexPro/openalexSnowball/tree/dev"><img src="https://img.shields.io/github/r-package/v/openalexPro/openalexSnowball/dev?label=dev" alt="dev version"></a></td>
  <td><a href="https://github.com/openalexPro/openalexSnowball/actions/workflows/R-CMD-check.yaml"><img src="https://img.shields.io/github/actions/workflow/status/openalexPro/openalexSnowball/R-CMD-check.yaml?label=CI" alt="CI"></a><br><a href="https://app.codecov.io/gh/openalexPro/openalexSnowball"><img src="https://codecov.io/gh/openalexPro/openalexSnowball/graph/badge.svg" alt="Codecov"></a></td>
</tr>
<tr>
  <td><a href="https://github.com/openalexPro/openalexConvert"><strong>openalexConvert</strong></a><br><a href="https://openalexpro.github.io/openalexConvert/"><img src="https://img.shields.io/badge/docs-📖-blue" alt="Docs"></a><br><a href="https://doi.org/10.5281/zenodo.20448988"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.20448988.svg" alt="DOI"></a></td>
  <td>Export a Parquet corpus to BibTeX, BibLaTeX, CSL JSON, Markdown, LaTeX, HTML or PDF via Pandoc, or straight into Zotero (collections and tags included)</td>
  <td><a href="https://openalexpro.r-universe.dev/openalexConvert"><img src="https://openalexpro.r-universe.dev/openalexConvert/badges/version" alt="r-universe version"></a><br><a href="https://github.com/openalexPro/openalexConvert/tree/main"><img src="https://img.shields.io/github/r-package/v/openalexPro/openalexConvert/main?label=main" alt="main version"></a><br><a href="https://github.com/openalexPro/openalexConvert/tree/dev"><img src="https://img.shields.io/github/r-package/v/openalexPro/openalexConvert/dev?label=dev" alt="dev version"></a></td>
  <td><a href="https://github.com/openalexPro/openalexConvert/actions/workflows/R-CMD-check.yaml"><img src="https://img.shields.io/github/actions/workflow/status/openalexPro/openalexConvert/R-CMD-check.yaml?label=CI" alt="CI"></a><br><a href="https://app.codecov.io/gh/openalexPro/openalexConvert"><img src="https://codecov.io/gh/openalexPro/openalexConvert/graph/badge.svg" alt="Codecov"></a></td>
</tr>
<tr>
  <td><a href="https://github.com/openalexPro/openalexSnapshot"><strong>openalexSnapshot</strong></a><br><a href="https://openalexpro.github.io/openalexSnapshot/"><img src="https://img.shields.io/badge/docs-📖-blue" alt="Docs"></a><br><a href="https://doi.org/10.5281/zenodo.20448992"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.20448992.svg" alt="DOI"></a></td>
  <td>Offline work with a local OpenAlex snapshot — ID, DOI and citation indexes, record extraction by ID or DOI at scale, and an offline citation graph; pure R over DuckDB</td>
  <td><a href="https://openalexpro.r-universe.dev/openalexSnapshot"><img src="https://openalexpro.r-universe.dev/openalexSnapshot/badges/version" alt="r-universe version"></a><br><a href="https://github.com/openalexPro/openalexSnapshot/tree/main"><img src="https://img.shields.io/github/r-package/v/openalexPro/openalexSnapshot/main?label=main" alt="main version"></a><br><a href="https://github.com/openalexPro/openalexSnapshot/tree/dev"><img src="https://img.shields.io/github/r-package/v/openalexPro/openalexSnapshot/dev?label=dev" alt="dev version"></a></td>
  <td><a href="https://github.com/openalexPro/openalexSnapshot/actions/workflows/R-CMD-check.yaml"><img src="https://img.shields.io/github/actions/workflow/status/openalexPro/openalexSnapshot/R-CMD-check.yaml?label=CI" alt="CI"></a><br><a href="https://app.codecov.io/gh/openalexPro/openalexSnapshot"><img src="https://codecov.io/gh/openalexPro/openalexSnapshot/graph/badge.svg" alt="Codecov"></a></td>
</tr>
<tr>
  <td><a href="https://github.com/openalexPro/openalexVectorComp"><strong>openalexVectorComp</strong></a><br><a href="https://openalexpro.github.io/openalexVectorComp/"><img src="https://img.shields.io/badge/docs-📖-blue" alt="Docs"></a><br><a href="https://doi.org/10.5281/zenodo.19607514"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.19607514.svg" alt="DOI"></a></td>
  <td>Text embedding, cosine-distance scoring, and threshold calibration — backend-neutral (HuggingFace, OpenAI, TEI)</td>
  <td><a href="https://openalexpro.r-universe.dev/openalexVectorComp"><img src="https://openalexpro.r-universe.dev/openalexVectorComp/badges/version" alt="r-universe version"></a><br><a href="https://github.com/openalexPro/openalexVectorComp/tree/main"><img src="https://img.shields.io/github/r-package/v/openalexPro/openalexVectorComp/main?label=main" alt="main version"></a><br><a href="https://github.com/openalexPro/openalexVectorComp/tree/dev"><img src="https://img.shields.io/github/r-package/v/openalexPro/openalexVectorComp/dev?label=dev" alt="dev version"></a></td>
  <td><a href="https://github.com/openalexPro/openalexVectorComp/actions/workflows/pr-checks.yml"><img src="https://img.shields.io/github/actions/workflow/status/openalexPro/openalexVectorComp/pr-checks.yml?label=CI" alt="CI"></a><br><a href="https://app.codecov.io/gh/openalexPro/openalexVectorComp"><img src="https://codecov.io/gh/openalexPro/openalexVectorComp/graph/badge.svg" alt="Codecov"></a></td>
</tr>
</tbody>
</table>

## Installation

**Released versions** come from the openalexPro r-universe, which builds them from each package's `main` branch. Install the packages you need; their openalexPro dependencies come along automatically:

```r
install.packages(
  c("openalexPro", "openalexSnowball", "openalexConvert",
    "openalexSnapshot", "openalexVectorComp"),
  repos = c("https://openalexpro.r-universe.dev", "https://cloud.r-project.org")
)
```

**Development versions** (the `dev` branch: newest features, not yet released) install from GitHub:

```r
# install.packages("remotes")
remotes::install_github("openalexPro/openalexPro", ref = "dev")
```

## Typical workflow

```r
# 1. Query OpenAlex and store the results as Parquet in my_project/parquet
library(openalexPro)
url <- pro_query(search = '"biodiversity" AND "ecosystem services"')
pro_fetch(url, project_folder = "my_project")

# 2. Or work offline with a local OpenAlex snapshot
library(openalexSnapshot)
build_corpus_index(root_dir = "/data/openalex")  # once per snapshot
lookup_by_id(root_dir = "/data/openalex", ids = "W2741809807")

# 3. Snowball-expand a set of seed papers (optional)
library(openalexSnowball)
pro_snowball(identifier = "W2741809807", output = "my_project/snowball")

# 4. Export to BibTeX, or into Zotero
library(openalexConvert)
corpus_export_via_pandoc("my_project/parquet", "my_project/refs.bib", to = "bibtex")
corpus_to_zotero("my_project")  # into the collection my_project > parquet
```

## Design principles

- **On-disk processing** — results are paged and written to Parquet; memory use stays flat regardless of corpus size.
- **Arrow / DuckDB throughout** — all data manipulation uses columnar formats; SQL queries run in-process.
- **Composable** — each package has a single responsibility and speaks the same Parquet dialect, so they chain naturally.
- **Pure R** — none of the packages has compiled code of its own, so nothing needs a toolchain to install.

## Contributing

Issues and pull requests are welcome on the individual package repositories. Please open an issue before starting large changes.

## Acknowledgements

This ecosystem builds on the excellent [openalexR](https://github.com/ropensci/openalexR) package and the [OpenAlex](https://openalex.org) team's commitment to open scholarly infrastructure.

## Disclaimer

The packages are provided **as is**. The authors are not affiliated with OpenAlex.
