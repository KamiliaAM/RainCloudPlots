# Raincloud Plots

[![Binder](https://img.shields.io/badge/R%20package-ggrain-brightgreen)](https://github.com/njudd/ggrain)
[![Binder](https://img.shields.io/badge/Python%20package-PtitPrince-red)](https://github.com/pog87/PtitPrince)
[![DOI](https://zenodo.org/badge/144041501.svg)](https://zenodo.org/badge/latestdoi/144041501)


***Code and tutorials to visualise your data in a way that is both beautiful *and* statistically valid.***
### Table of contents


* [Making Rainclouds in R with ggrain](#making-rainclouds-in-r)
* [Making Rainclouds in Python with PtitPrince](#making-rainclouds-in-python)
* [Attribution](#attribution)
* [Feedback](#feedback)


![](images/10repanvplot_cropped.jpg)

## Making Rainclouds in R

### R package - `ggrain`

Check out the [Github](https://github.com/njudd/ggrain) and the [vignette](https://www.njudd.com/raincloud-ggrain/) for more details!

#### Install
```install.packages('ggrain')```

#### Plot
```
library(ggrain)

ggplot(iris, aes(Species, Sepal.Length, fill = Species)) + 
	geom_rain()
```

## Making Rainclouds in Python


### Python package - `PtitPrince`

Check out the [Github](https://github.com/pog87/PtitPrince) and the [tutorial](https://github.com/pog87/PtitPrince/blob/master/tutorial_python/raincloud_tutorial_python.ipynb) for more details!

#### Install
```pip install ptitprince```

#### Plot
```
import sys
sys.path.append('../ptitprince/')
import PtitPrince as pt

pt.RainCloud(x = dx, y = dy, data = df, palette = pal, bw = sigma,
                 width_viol = .6, ax = ax, orient = ort)
```


## Attribution

We really hope you find these tutorials helpful and want to use the code in your next paper or presentation!

This repository is made available under the [MIT license](LICENSE) which means you're welcome to use and remix the contents so long as you credit the creators: [Micah Allen](https://twitter.com/micahgallen?lang=en), [Davide Poggiali](https://twitter.com/dav1d3p0g?lang=en), [Kirstie Whitaker](https://twitter.com/kirstie_j?lang=en), [Tom Rhys Marshall](https://twitter.com/tomrhysmarshall?lang=en), [Jordy van Langen](https://twitter.com/jordyvanlangen?lang=en), [Nicholas Judd](https://njudd.com) and [Rogier Kievit](https://www.rogierkievit.com/).

If you use rainclouds please cite us!

#### Preprint

> Allen M, Poggiali D, Whitaker K et al. Raincloud plots: a multi-platform tool for robust data visualization [version 2; peer review: 2 approved]. Wellcome Open Res 2021, 4:63. DOI: [10.12688/wellcomeopenres.15191.2](https://doi.org/10.12688/wellcomeopenres.15191.2)

#### ggrain package

> Judd, N., van Langen, J., Allen, M., & Kievit, R.A.
    <i>ggrain: A Rainclouds Geom for 'ggplot2'.</i>
    R package version 0.0.3.
    <b>CRAN</b> 2023,
    <a href="https://CRAN.R-project.org/package=ggrain">https://CRAN.R-project.org/package=ggrain</a>



## Feedback

We'd love to hear your thoughts and any feedback you have.
The best place to leave comments on the paper and the project in general is at the [Wellcome Open Research preprint](https://doi.org/10.12688/wellcomeopenres.15191.2).
Just scroll to the bottom of that page (or click on the link at the side) and leave us feedback or ask a question.

You can also open an issue or submit a pull request to this repository if you find a bug! If it is a package specific question please make an issue on the [`ggrain`](https://github.com/njudd/ggrain/issues) or [`PtitPrince`](https://github.com/pog87/PtitPrince/issues) repositories.

Just check out our [contributing guidelines](CONTRIBUTING.md) for help getting started.
