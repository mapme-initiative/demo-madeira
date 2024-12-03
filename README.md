# demo-madeira

This repository contains the source code of a quarto project showcasing
the usage of `mapme.biodiversity` to estimate changes in forest cover
caused by flooding as a consequence of dam building at the Madeira river in
Rondônia, Brazil.

The rendered version can be visited by following this link:

[https://mapme-initiative.github.io/demo-madeira/](https://mapme-initiative.github.io/demo-madeira/)


## For developers

The R dependencies are tracked via `renv`. After cloning the repository
you will need to restore the development environment, e.g. with:

```shell
git clone https://github.com/mapme-initiative/demo-madeira.git
cd demo-madeira
Rscript -e "renv::restore()"
```

Then to preview the project:

```shell
quarto preview
```

Note, that due to the size of the required data for this tutorial,
the site is not automatically build with GitHub actions. Instead,
after commiting your changes, the site must be built locally and pushed
to the `gh-pages` branch via:

```shell
quarto publish gh-pages
```