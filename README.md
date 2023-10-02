# movie_plots_nlp
## Purpose 
* This is an NLP (Natural Language Processing) project focused on movie plots. Different kind of models are going to be created with different objective.

## Tools and Packages
The code was run on [Jupyter](https://jupyter.org/) *(Jupyter Notebook 7.0.3 and Python 3.11.5 will work for sure)*. 

Additional packages required for the project to run are:
* [pandas](https://pandas.pydata.org/)
* [scikit-learn](https://scikit-learn.org/stable/)
* [NumPy](https://numpy.org/)
* [matplotlib](https://matplotlib.org/)
* [SciPy](https://scipy.org/)
* [seaborn](https://seaborn.pydata.org/)
* [nltk](https://www.nltk.org/)
* [spaCy](https://spacy.io/) (also the <code>en_core_web_md</code> model of spaCy must be installed by running <code>python -m spacy download en_core_web_sm</code>)
* [imblearn](https://imbalanced-learn.org/stable/)
* [xgboost](https://xgboost.readthedocs.io/en/stable/)
* [Tensorflow](https://www.tensorflow.org/)

All the packages above can be installed using the `pip install` command-line command.

## Data
* The data were obtained by [Kaggle](https://www.kaggle.com/) and the [Wikipedia Movie Plots](https://www.kaggle.com/datasets/jrobischon/wikipedia-movie-plots) dataset specifically.
* In more detail, this dataset contains the **Plots** and **Genres** of about 35000 movies from around the world, that were scraped from [Wikipedia](https://www.wikipedia.org/).

## Contents
### Notebooks
* <code>data_preparation</code>: includes the preparation of data for the various Machine Learning tasks.
* <code>genre_classification</code>: this task focuses on performing classification of movies into genres based on their plots, with a specific emphasis on the drama and comedy categories.

### Data *(included into the <code>./data</code> folder)*
* <code>wiki_movie_plots_deduped.csv</code>: the initial data as were taken from Kaggle.

#### Data for classification *(included into the <code>./data/classification</code> folder)*
*This folder includes the data prepared for the classification task.*
* <code>genre_encoding.pickle</code>: the encoding of *genre ids (int)* to *genre names (string)*.
* <code>genres_encoded.npy</code>: a numpy array including the encoding of the genres (in the same order as the corresponding plots).
* <code>plots.npy</code>: a numpy array including the encoding of the genres.
* <code>cleaned_plots.npy</code>: the plots of the <code>plots.npy</code> file after cleaning was applied.
