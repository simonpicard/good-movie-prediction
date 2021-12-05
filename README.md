# good-movie-prediction

A data science assignment I did in 2021.

## Quickstart

```
git clone git@github.com:simonpicard/good-movie-prediction.git
cd good-movie-prediction
conda env create -f environment.yml
conda activate good_movie
```
- Downlad the [IMDb dataset](https://www.kaggle.com/stefanoleone992/imdb-extensive-dataset) and move its content to `/data`.
- Downlad the [GloVe Common Crawl (840B.300d)](https://nlp.stanford.edu/data/glove.840B.300d.zip) and move its content to `/data`.
  - If the above link does not work, you may also download it from [kaggle](https://www.kaggle.com/takuok/glove840b300dtxt)

You are now ready to run the notebook.

```
jupyter lab
```

Explore key takeaways in `key_takeaways.pdf`.
 
## Goal 

Create a predictive model that predicts whether a movie will achieve an average IMDb rating of > 7.5. Shows the variables that have the greatest impact on model decisions. Also shows the predicted performance of the model with a random sample of 10% of the data.

## Dataset

The dataset can be fetched from [Kaggle](https://www.kaggle.com/stefanoleone992/imdb-extensive-dataset).

Thanks to [Stefano Leone](https://www.kaggle.com/stefanoleone992) for sharing it.

### Context

IMDb is the most popular movie website and it combines movie plot description, Metastore ratings, critic and user ratings and reviews, release dates, and many more aspects.

The website is well known for storing almost every movie that has ever been released (the oldest is from 1874 - "Passage de Venus") or just planned to be released (newest movie is from 2027 - "Avatar 5").

IMDb stores information related to more than 6 million titles (of which almost 500,000 are featured films) and it is owned by Amazon since 1998.

### Content

- The movies dataset includes 85,855 movies with attributes such as movie description, average rating, number of votes, genre, etc.
- The ratings dataset includes 85,855 rating details from demographic perspective.
- The names dataset includes 297,705 cast members with personal attributes such as birth details, death details, height, spouses, children, etc.
- The title principals dataset includes 835,513 cast members roles in movies with attributes such as IMDb title id, IMDb name id, order of importance in the movie, role, and characters played.

### Acknowledgements

Data has been scraped from the publicly available website https://www.imdb.com.

All the movies with more than 100 votes have been scraped as of 01/01/2020.
