---
title: openalexPro
description: An R ecosystem for large-scale, on-disk access to OpenAlex
---

# openalexPro

An R ecosystem for large-scale, on-disk access to [OpenAlex](https://openalex.org) — the open catalogue of global scholarly work.

OpenAlex provides free, comprehensive metadata on over 250 million scholarly works, authors, institutions, and concepts. The **openalexPro** ecosystem is built around a single design principle: process data on disk rather than in memory, so workflows scale to millions of records without hitting RAM limits.

## Packages

<table>
<thead>
<tr><th>Package</th><th>Description</th><th>CI</th><th>Docs</th><th>Install</th></tr>
</thead>
<tbody>
<tr>
  <td><a href="https://github.com/openalexPro/openalexPro"><strong>openalexPro</strong></a></td>
  <td>Core API client — query OpenAlex, page through results, and store everything in Parquet files for efficient downstream use</td>
  <td><a href="https://github.com/openalexPro/openalexPro/actions/workflows/R-CMD-check.yaml"><img src="https://github.com/openalexPro/openalexPro/actions/workflows/R-CMD-check.yaml/badge.svg" height="22" alt="CI"></a></td>
  <td><a href="https://openalexpro.github.io/openalexPro/"><img src="https://img.shields.io/badge/docs-📖-blue" height="22" alt="Docs"></a></td>
  <td><a href="https://openalexpro.r-universe.dev/openalexPro"><img src="https://openalexpro.r-universe.dev/openalexPro/badges/version" height="22" alt="r-universe"></a></td>
</tr>
<tr>
  <td><a href="https://github.com/openalexPro/openalexSnowball"><strong>openalexSnowball</strong></a></td>
  <td>Snowball citation searches — iteratively expand a seed set by following forward and backward citations across the graph</td>
  <td><a href="https://github.com/openalexPro/openalexSnowball/actions/workflows/R-CMD-check.yaml"><img src="https://github.com/openalexPro/openalexSnowball/actions/workflows/R-CMD-check.yaml/badge.svg" height="22" alt="CI"></a></td>
  <td><a href="https://openalexpro.github.io/openalexSnowball/"><img src="https://img.shields.io/badge/docs-📖-blue" height="22" alt="Docs"></a></td>
  <td><a href="https://openalexpro.r-universe.dev/openalexSnowball"><img src="https://openalexpro.r-universe.dev/openalexSnowball/badges/version" height="22" alt="r-universe"></a></td>
</tr>
<tr>
  <td><a href="https://github.com/openalexPro/openalexConvert"><strong>openalexConvert</strong></a></td>
  <td>Export a Parquet corpus to BibTeX, BibLaTeX, CSL JSON, Markdown, LaTeX, HTML, or PDF via Pandoc</td>
  <td><a href="https://github.com/openalexPro/openalexConvert/actions/workflows/R-CMD-check.yaml"><img src="https://github.com/openalexPro/openalexConvert/actions/workflows/R-CMD-check.yaml/badge.svg" height="22" alt="CI"></a></td>
  <td><a href="https://openalexpro.github.io/openalexConvert/"><img src="https://img.shields.io/badge/docs-📖-blue" height="22" alt="Docs"></a></td>
  <td><a href="https://openalexpro.r-universe.dev/openalexConvert"><img src="https://openalexpro.r-universe.dev/openalexConvert/badges/version" height="22" alt="r-universe"></a></td>
</tr>
<tr>
  <td><a href="https://github.com/openalexPro/openalexSnapshot"><strong>openalexSnapshot</strong></a></td>
  <td>Bulk snapshot tools — convert the full OpenAlex JSON.GZ snapshot to Parquet, build ID-lookup indexes, and extract records at scale using a Rust back-end</td>
  <td><a href="https://github.com/openalexPro/openalexSnapshot/actions/workflows/R-CMD-check.yaml"><img src="https://github.com/openalexPro/openalexSnapshot/actions/workflows/R-CMD-check.yaml/badge.svg" height="22" alt="CI"></a></td>
  <td><a href="https://openalexpro.github.io/openalexSnapshot/"><img src="https://img.shields.io/badge/docs-📖-blue" height="22" alt="Docs"></a></td>
  <td><a href="https://openalexpro.r-universe.dev/openalexSnapshot"><img src="https://openalexpro.r-universe.dev/openalexSnapshot/badges/version" height="22" alt="r-universe"></a></td>
</tr>
<tr>
  <td><a href="https://github.com/openalexPro/openalexVectorComp"><strong>openalexVectorComp</strong></a></td>
  <td>Text embedding, cosine-distance scoring, and threshold calibration — backend-neutral (HuggingFace, OpenAI, TEI)</td>
  <td><a href="https://github.com/openalexPro/openalexVectorComp/actions/workflows/pr-checks.yml"><img src="https://github.com/openalexPro/openalexVectorComp/actions/workflows/pr-checks.yml/badge.svg" height="22" alt="CI"></a></td>
  <td><a href="https://openalexpro.github.io/openalexVectorComp/"><img src="https://img.shields.io/badge/docs-📖-blue" height="22" alt="Docs"></a></td>
  <td><a href="https://openalexpro.r-universe.dev/openalexVectorComp"><img src="https://openalexpro.r-universe.dev/openalexVectorComp/badges/version" height="22" alt="r-universe"></a></td>
</tr>
</tbody>
</table>

## Rust core

<table>
<thead>
<tr><th>Package</th><th>Description</th><th>CI</th><th>Docs</th><th>Release</th></tr>
</thead>
<tbody>
<tr>
  <td><a href="https://github.com/openalexPro/openalex-snapshot"><strong>openalex-snapshot</strong></a></td>
  <td>Compiled Rust CLI and library powering <code>openalexSnapshot</code>'s hot path (JSON→Parquet conversion, indexing, ID extraction). Downloaded automatically as a pre-built static library on install — no manual Rust setup required for most users.</td>
  <td><a href="https://github.com/openalexPro/openalex-snapshot/actions/workflows/ci.yml"><img src="https://github.com/openalexPro/openalex-snapshot/actions/workflows/ci.yml/badge.svg" height="22" alt="CI"></a></td>
  <td><a href="https://openalexpro.github.io/openalex-snapshot/"><img src="https://img.shields.io/badge/docs-📖-blue" height="22" alt="Docs"></a></td>
  <td><a href="https://github.com/openalexPro/openalex-snapshot/releases/latest"><img src="https://img.shields.io/github/v/release/openalexPro/openalex-snapshot" height="22" alt="Release"></a></td>
</tr>
</tbody>
</table>

## Installation

All R packages are available from the openalexPro r-universe:

```r
install.packages(
  c("openalexPro", "openalexSnowball", "openalexConvert",
    "openalexSnapshot", "openalexVectorComp"),
  repos = c("https://openalexpro.r-universe.dev", "https://cloud.r-project.org")
)
```

## Typical workflow

```r
library(openalexPro)

# 1. Query OpenAlex and store results as Parquet
fetch_works(
  query = '"biodiversity" AND "ecosystem services"',
  output = "my_corpus"
)

# 2. Or work directly with the bulk OpenAlex snapshot
library(openalexSnapshot)
oa_snapshot_to_parquet(
  snapshot_dir = "/data/openalex-snapshot",
  parquet_dir  = "/data/openalex-parquet"
)

# 3. Snowball-expand a seed set (optional)
library(openalexSnowball)
snowball(corpus = "my_corpus", depth = 1, output = "my_corpus_expanded")

# 4. Export to BibTeX, CSL JSON, etc.
library(openalexConvert)
corpus_to_csljson("my_corpus", output = "csl/")
csljson_convert_pandoc("csl/", "refs/", to = "bibtex")
```

## Design principles

- **On-disk processing** — results are paged and written to Parquet; memory use stays flat regardless of corpus size.
- **Arrow / DuckDB throughout** — all data manipulation uses columnar formats; SQL queries run in-process.
- **Composable** — each package has a single responsibility and speaks the same Parquet dialect, so they chain naturally.
- **Rust where it matters** — the bulk snapshot converter delegates hot-path work to a compiled Rust back-end ([openalex-snapshot](https://github.com/openalexPro/openalex-snapshot)), with a pure-R/DuckDB fallback for environments without a Rust toolchain.

## Contributing

Issues and pull requests are welcome on the individual package repositories. Please open an issue before starting large changes.

## Acknowledgements

This ecosystem builds on the excellent [openalexR](https://github.com/ropensci/openalexR) package and the [OpenAlex](https://openalex.org) team's commitment to open scholarly infrastructure.

## Disclaimer

The packages are provided **as is**. The authors are not affiliated with OpenAlex.
