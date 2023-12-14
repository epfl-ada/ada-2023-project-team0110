# Team0110 - ADA Project

# Milestone 3

## Title : 

**From Book to Movie : an analysis of book adaptation to the cinema industry**

## Abstract : 

Ever since the advent of cinema, filmmakers have drawn inspiration from books. From 1968 to 2002, [35% of all English-language films originated from books](https://www.frontier-economics.com/media/vyfd1iz3/publishings-contribution-to-the-wider-creative-industries.pdf). Particularly in high-stakes Hollywood productions, often [exceeding $100 million](https://www.statista.com/statistics/1389936/breakdown-production-budget-hollywood-movies-worldwide/#:~:text=Out%20of%20the%2089%20English,under%20ten%20million%20U.S.%20dollars), executives favor book adaptations, capitalizing on the established fanbases of beloved books. This raises the question: what are the key elements of a successful book-to-film adaptation? Are there specific genres that lend themselves more easily to cinematic adaptation? Is it more effective to adapt recent bestsellers or time-honored classics? And, in light of blockbusters like Harry Potter and Lord of the Rings, should the focus be on serial adaptations rather than standalone novels?
To address these inquiries, we will analyze data from the [CMU Movie Summary Corpus](http://www.cs.cmu.edu/~ark/personas/), [TMDB](https://www.themoviedb.org), [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) and [Goodreads](https://www.kaggle.com/datasets/mdhamani/goodreads-books-100k). Our goal is to use this comprehensive analysis to develop a model that can effectively identify the most promising book for a successful film adaptation.

## Research questions :
**Intro : How do book adaptations compare to original movies?**
* Do movies based on books perform better at the box office?
* Are movies based on books better movies according to IMDB ratings?

**I) What kind of books are turned into movies?**
* When where the adapted books published?
* Do books that are adapted into movies typically have higher ratings on Goodreads?
* Do filmmakers tend to favor shorter or longer books for movie adaptations?
* Are books that are adapted into movies typically more popular and critically acclaimed?
* Are there certain book genres that are more suitable for movie adaptations?
* Is it possible to predict which books will be selected for movie adaptations? If so, can we predict which books will be adapted next? 

**II) What makes a commercially successful book adaptation?**
* Is there a book genre that leads to successful adaptations?
* Do book adaptations on book series perform better at the box office?
* What is the ideal time frame between a book's publication and its adaptation?
* How does the popularity of the book affect the box office revenue?
* Can we predict the expected revenue of a future book adaptation? If so, which adaptation would perform best at the box office?


## Proposed additional dataset :

The CMU movie summary corpus dataset contains about 80'000 movies with informations like release dates, duration, genre and actors. For the purpose of our study we enriched it using data from multiple sources:
- `IMDb Ratings`: To quantify the audience reception of movies, we extend our dataset by IMDb scores
- `TMDB`: For most entries in the CMU movie dataset, information about the revenue is missing. We used data obtained from `The Movie Database (TMDB)` to fill missing values for revenue. 
- `Wikidata`: To get the information on which movies are book adaptations we queried the Wikidata Graph Database using SPARQL. In addition we also queried additional information about the books such as release dates, number of page, genre, or author. That way, the characteristics of the book can be compared and linked to the one of the movie and its final success.
- `Goodreads`: We supplement our book data with a dataset scraped from Goodreads, which includes additional information such as a user ratings or number of pages for each book.
- `Consumer Price Index`: As we deal with revenue data from multiple decades, we need to normalize them to make them compareable. Therfore we use the US-Consumer Price Index (CPI). 


## Methods :

First of all, the team familiarized with the dataset and got to know the various features in each dataframes. This first step in our analysis allowed the team to come up with many other ideas and research questions. This lead our team to explore ideas for which the analysis would require additional data.

In order to extract additional data from the internet, the Wikidata Query Service was used. The wikiID present in the given movie metadata were helpful to retrieve the wikidata page of a movie and determine wether it is based on a book or not. The Query Service was also used to feed the book dataset with various information that could be useful for our analysis. Moreover, the team decided to extract more data on the web, regarding the movies and the books ratings. From the non-commercial dataset available on the Internet Movie Database (IMDb) was retrieved movie ratings. In order to link this dataset to our current one, the IMDb ID (a.k.a tconst) was extracted from the wikidata pages of the movies. This allowed to feed our dataset with additional data from which we could analyse the public appreciation of each movies. Similarly, ratings and reviews of books are added to the dataset from the GoodReads website.

After familiarizing with the dataset and adding it relevant data, the time of data wrangling has come for our team. This step is very important to avoid biased analysis. The first data wrangling action was done by analyzing the missing data of the various features of our movie metadata. It was observed that information about the box office of many old movies were missing. Carrying out analysis of the performance of movies based on their financial results could therefore not be sufficient to draw conclusions. Hopefully, we retrieved movie ratings which have far less missing data and from which we could base some analysis. 

Three distinct notebooks were created to enhance readability : two for the data collection and data wrangling, called `create_movie_dataset.ipynb` and `create_adaptation_dataset.ipynb` and one for the analysis, called `milestone2.ipynb`.

Different statistical metrics like T-tests, confidence intervals, box plots,… will be used in order to study the data, visualise it and quantify the uncertainty. Later on in the analysis, the team plans on using correlation coefficients to measure the relationship between the studied data.

## Proposed timeline : 
* 17.11.23 : project milestone 2
* 24.11.23 : end of data collection and initial organisation
* 01.12.23 : visualisation of results
* 08.12.23 : quantification of error and uncertainty of the results
* 15.12.23 : end of the code
* 22.12.23 : end of website (project milestone 3)

## Organisation within the team :
Mainly organized in group of two for each task
* **Nils** : data collection, data organisation
* **Mirco** : data collection, Statistical analysis
* **Romain** : Statistical analysis, website
* **Lucas** : Data collection, Data visualisation 
* **Justin** : Data visualisation, Data organisation
