# CorrelAid Machine Learning Winter School

Welcome to the CorrelAid ML Winter School!

## Task

The problem we want to solve is to classify a mushroom either as eatable or poisonous. 

## Setup

Please make sure you have a modern Python 3 installation. We recommend the Python distribution [Miniconda](https://docs.conda.io/en/latest/miniconda.html) that is available for all OS.   

The easiest way to get started is with a clean virtual environment. You can do so by running the following commands, assuming that you have installed Miniconda or Anaconda.

```Bash
$ conda create -n winter-school python=3.9
$ conda activate winter-school
(winter-school) $ pip install -r requirements.txt
(winter-school) $ python -m ipykernel install --user --name winter-school --display-name "Python 3.9 (winter-school)"
```

The first command will create a new environment with Python 3.9. To use this environment, you call `conda activate <name>` with the name of the environment as second step. Once activated, you can install packages as usual with the `pip` package manager. You will install all listed requirements from the provided `requirements.txt` as a third step. Finally, to actually make your new environment available as kernel within a Jupyter notebook, you need to run `ipykernel install`, which is the fourth command. 

Once the setup is complete, you can run any notebook by calling 

```Bash
(winter-school) $ <jupyter-lab|jupyter notebook>
```

`jupyter lab` is opening your browser with a local version of [JupyterLab](https://jupyter.org/), which is a web-based interactive development environment that is somewhat more powerful and more modern than the older Jupyter Notebook. Both work fine, so you can choose the tool that is more to your liking. We recommend to go with Jupyter Lab as it provides a file browser, among other improvements.

## Data

The data to be analyzed is one of the classic data sets from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php), the [Mushroom Data Set](https://archive.ics.uci.edu/ml/datasets/mushroom).

It's a multivariate data set with 22 attributes and 8124 observations, donated in the year 1987. Mushroom records are drawn from The Audubon Society Field Guide to North American Mushrooms (1981). G. H. Lincoff (Pres.), New York: Alfred A. Knopf 

This data set includes descriptions of hypothetical samples corresponding to 23 species of gilled mushrooms in the Agaricus and Lepiota Family (pp. 500-525). Each species is identified as definitely edible, definitely poisonous, or of unknown edibility and not recommended. This latter class was combined with the poisonous one. The Guide clearly states that there is no simple rule for determining the edibility of a mushroom; no rule like ``leaflets three, let it be'' for Poisonous Oak and Ivy.

**Note**: We provide the data set as it can be downloaded from [kaggle](https://www.kaggle.com/uciml/mushroom-classification) and not in its original form from the UCI repository.

### Attribute Information:

1. cap-shape: bell=b, conical=c, convex=x, flat=f, knobbed=k, sunken=s
2. cap-surface: fibrous=f, grooves=g, scaly=y, smooth=s
3. cap-color: brown=n, buff=b, cinnamon=c, gray=g, green=r, pink=p, purple=u, red=e, white=w, yellow=y
4. bruises?: bruises=t, no=f
5. odor: almond=a, anise=l, creosote=c, fishy=y, foul=f, musty=m, none=n, pungent=p, spicy=s
6. gill-attachment: attached=a, descending=d, free=f, notched=n
7. gill-spacing: close=c, crowded=w, distant=d
8. gill-size: broad=b, narrow=n
9. gill-color: black=k, brown=n, buff=b, chocolate=h, gray=g, green=r, orange=o, pink=p, purple=u, red=e, white=w, yellow=y
10. stalk-shape: enlarging=e, tapering=t
11. stalk-root: bulbous=b, club=c, cup=u, equal=e, rhizomorphs=z, rooted=r, missing=?
12. stalk-surface-above-ring: fibrous=f, scaly=y, silky=k, smooth=s
13. stalk-surface-below-ring: fibrous=f, scaly=y, silky=k, smooth=s
14. stalk-color-above-ring: brown=n, buff=b, cinnamon=c, gray=g, orange=o, pink=p, red=e, white=w, yellow=y
15. stalk-color-below-ring: brown=n, buff=b, cinnamon=c, gray=g, orange=o, pink=p, red=e, white=w, yellow=y
16. veil-type: partial=p, universal=u
17. veil-color: brown=n, orange=o, white=w, yellow=y
18. ring-number: none=n, one=o, two=t
19. ring-type: cobwebby=c, evanescent=e, flaring=f, large=l, none=n, pendant=p, sheathing=s, zone=z
20. spore-print-color: black=k, brown=n, buff=b, chocolate=h, green=r, orange=o, purple=u, white=w, yellow=y
21. population: abundant=a, clustered=c, numerous=n, scattered=s, several=v, solitary=y
22. habitat: grasses=g, leaves=l, meadows=m, paths=p, urban=u, waste=w, woods=d


