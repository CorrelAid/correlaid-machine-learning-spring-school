# CorrelAid Machine Learning Spring School

Welcome to the CorrelAid ML Spring School!

In this repository you can find the slides and other files for the CorrelAid ML Spring School.
The following sections become relevant as the course progresses.

## Task

The problem we want to solve is to classify trees in Roosevelt National Forest.

## Setup

Please make sure you have a modern Python 3 installation. We recommend the Python distribution [Miniconda](https://docs.conda.io/en/latest/miniconda.html) that is available for all OS.

The easiest way to get started is with a clean virtual environment. You can do so by running the following commands, assuming that you have installed Miniconda or Anaconda.

```Bash
$ conda create -n spring-school python=3.9
$ conda activate spring-school
(spring-school) $ pip install -r requirements.txt
(spring-school) $ python -m ipykernel install --user --name spring-school --display-name "Python 3.9 (spring-school)"
```

The first command will create a new environment with Python 3.9. To use this environment, you call `conda activate <name>` with the name of the environment as second step. Once activated, you can install packages as usual with the `pip` package manager. You will install all listed requirements from the provided `requirements.txt` as a third step. Finally, to actually make your new environment available as kernel within a Jupyter notebook, you need to run `ipykernel install`, which is the fourth command.

Once the setup is complete, you can run any notebook by calling

```Bash
(spring-school) $ <jupyter-lab|jupyter notebook>
```

`jupyter lab` is opening your browser with a local version of [JupyterLab](https://jupyter.org/), which is a web-based interactive development environment that is somewhat more powerful and more modern than the older Jupyter Notebook. Both work fine, so you can choose the tool that is more to your liking. We recommend to go with Jupyter Lab as it provides a file browser, among other improvements.

###

If you encounter any difficulties while installing, please contact Daniel, Pia or Flo.

## Data

The data to be analyzed is one of the classic data sets from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php), the [Forest Cover Type Dataset](https://archive.ics.uci.edu/ml/datasets/Covertype).

The dataset contains tree observations from four areas of the Roosevelt National Forest in Colorado. All observations are cartographic variables (no remote sensing) from 30 meter x 30 meter sections of forest. There are over half a million measurements total!

The dataset includes information on tree type, shadow coverage, distance to nearby landmarks (roads etcetera), soil type, and local topography.

**Note**: We provide the data set as it can be downloaded from [kaggle](https://www.kaggle.com/uciml/forest-cover-type-dataset) and not in its original form from the UCI repository.

### Attribute Information:

Given is the attribute name, attribute type, the measurement unit and a brief description. The forest cover type is the classification problem. The order of this listing corresponds to the order of numerals along the rows of the database.

Name / Data Type / Measurement / Description

- Elevation / quantitative /meters / Elevation in meters
- Aspect / quantitative / azimuth / Aspect in degrees azimuth
- Slope / quantitative / degrees / Slope in degrees
- Horizontal_Distance_To_Hydrology / quantitative / meters / Horz Dist to nearest surface water features
- Vertical_Distance_To_Hydrology / quantitative / meters / Vert Dist to nearest surface water features
- Horizontal_Distance_To_Roadways / quantitative / meters / Horz Dist to nearest roadway
- Hillshade_9am / quantitative / 0 to 255 index / Hillshade index at 9am, summer solstice
- Hillshade_Noon / quantitative / 0 to 255 index / Hillshade index at noon, summer soltice
- Hillshade_3pm / quantitative / 0 to 255 index / Hillshade index at 3pm, summer solstice
- Horizontal_Distance_To_Fire_Points / quantitative / meters / Horz Dist to nearest wildfire ignition points
- Wilderness_Area (4 binary columns) / qualitative / 0 (absence) or 1 (presence) / Wilderness area designation
- Soil_Type (40 binary columns) / qualitative / 0 (absence) or 1 (presence) / Soil Type designation
- Cover_Type (7 types) / integer / 1 to 7 / Forest Cover Type designation

[![CC BY 4.0](https://img.shields.io/badge/license-cc%20by%204.0-lightgrey.svg)](http://creativecommons.org/licenses/by/4.0/)
