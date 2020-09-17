# Custom profile for SPHERES augur builds

## State- and territory-level colors

Each state- and territory-level build has its own custom color profile for display in auspice.
These color profiles use a base color scheme based on [Emma Hodcroft's colors for her Southern USA builds](https://raw.githubusercontent.com/emmahodcroft/south-usa-sarscov2/master/profiles/south-central/colors.tsv).
For each build, the given build's state or territory is given a red color to clearly distinguish that division from other divisions in the auspice view.
To build these custom build-level color schemes, run the following command from the top-level of the repository.

```python
python3 spheres_profile/build_state_colors.py \
    --colors spheres_profile/colors.tsv \
    --builds spheres_profile/builds.yaml \
    --colors-directory spheres_profile/state_colors/ \
    --revised-builds spheres_profile/revised_builds.yaml
```

Then modify the revised builds, as needed, for readability and replace the original builds YAML with this new file.
