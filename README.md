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
For more details about modifying builds, [see the SPHERES profile README](spheres_profile/README.md).
Run the workflow.

```bash
snakemake --profile spheres_profile/
```

View the resulting builds with auspice from a local machine.

```bash
auspice view
```
