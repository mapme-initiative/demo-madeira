# demo-madeira

This repository contains the source code of a quarto project showcasing
the usage of `mapme.biodiversity` to estimate changes in forest cover
caused by flooding as a consequence of dam building at the Madeira river in
Rondônia, Brazil.

The R dependecies are tracked via `renv`. After cloning the repository
you will need to restore the develeopment environment, e.g. with:


```shell
$ git clone https://github.com/mapme-initiative/demo-madeira.git
$ cd deom-madeira
$ Rscript -e "renv::restore()"
```

Then to preview the project:

```shell
$ quarto preview
```

Note, that due to the size of the required data for this tutorial,
the site is not automatically build with GitHub actions. Instead,
after commiting your changes, the site must be built locally and pushed
to the `gh-pages` branch via:

```shell
$ quarto publish gh-pages
```