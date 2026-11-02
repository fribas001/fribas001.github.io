# RF & EMF Lab

A Quarto website by Felipe Oliveira Ribas for Blender, Sionna and reproducible radio simulation workflows.

Website address: https://fribas001.github.io/

## Content

- Software: SionnaRT-Bridge, Mitsuba–Blender compatibility, and local DiffeRT/Mobility development.
- Tutorials: starting with an example scene and publishing a reproducible result.
- Case studies: procedural vegetation, Antwerp mobility, and Sionna/DiffeRT comparisons.
- Talks: the two Blender conference recordings, with the supplied timestamps.
- Research resources: reproducibility guidance, scope and source credits.

## Edit and preview

Install [Quarto](https://quarto.org/docs/get-started/), then run from this repository:

```sh
quarto preview
quarto render
```

Edit the `.qmd` files and put compact media in `assets/`. Site navigation is configured in `_quarto.yml`. Generated `_site/` and `.quarto/` directories stay untracked.

## Deploy

In repository **Settings → Pages**, set **Source: GitHub Actions**. The included workflow builds pull requests and deploys pushes to `main`. It pins Quarto to version 1.10.20 and does not execute simulation code.

Run simulations in their own environments and publish selected results here. Put large reproduction bundles in versioned Releases or a research archive, and link them from the relevant study.

## Credits

The site structure is inspired by [Molecular Nodes](https://bradyajohnston.github.io/MolecularNodes/), with original layout code and project imagery. See [About & credits](about.qmd) for media provenance. Geographic data © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright), ODbL. Source projects and third-party media retain their own licenses.

Local development examples are explicitly labeled; their presence does not imply a public software release or validation outside the described scope.
