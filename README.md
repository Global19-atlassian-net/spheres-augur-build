# SPHERES augur builds

## About

This repository analyzes viral genomes using [Nextstrain](https://nextstrain.org) to understand how SARS-CoV-2, the virus that is responsible for the COVID-19 pandemic, evolves and spreads.
This is a copy of [the original Nextstrain ncov repository](https://github.com/nextstrain/ncov/).

## Usage

Clone this repository.

```bash
git clone https://github.com/nextstrain/spheres-augur-build.git
cd spheres-augur-build/
```

Modify build definitions, as needed, in `spheres_profile/builds.yaml`.
Modify general Snakemake configuration (e.g., how the workflow is parallelized, distributed to a cluster, etc.) in `spheres_profile/config.yaml`.
Run the workflow.

```bash
snakemake --profile spheres_profile/
```

View the resulting builds with auspice from a local machine.

```bash
auspice view
```
