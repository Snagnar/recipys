# ReciPys
![example workflow](https://github.com/rvandewater/recipys/actions/workflows/main.yml/badge.svg)
The ReciPys package is a preprocessing framework operating on Pandas dataframes. 
The operation of this package is inspired by the R-package [recipes](https://recipes.tidymodels.org/).
This package allows the user to apply a number of extensible operations for imputation, feature generation/extraction, 
scaling, and encoding. 
It operates on modified Dataframe objects from the established data science package Pandas.
## Installation

```
conda env update -f environment.yml
conda activate recipys
pip install -e .
```
> Note that the last command installs the package called `recipys`.

## Usage
To define preprocessing operations, one has to supply _roles_ to the different columns of the Dataframe. 
This allows the user to create groups of columns which have a particular function.
Then, we provide several "steps" that can be applied to the datasets, among which: Historical accumulation, 
Resampling the time resolution, A number of imputation methods, and a wrapper for any 
[Scikit-learn](https://github.com/scikit-learn/scikit-learn) preprocessing step.
We believe to have covered any basic preprocessing needs for prepared datasets.
Any missing step can be added by following the step interface.





