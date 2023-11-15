# Team0110 - ADA Project

# Milestone 2

## Title : 

**From Book to Movie : a analysis of book adaptation to the cinema industry**

## Abstract : 

Ever since the advent of cinema, filmmakers have drawn inspiration from books. From 1968 to 2002, [35% of all English-language films originated from books](https://www.frontier-economics.com/media/vyfd1iz3/publishings-contribution-to-the-wider-creative-industries.pdf). Particularly in high-stakes Hollywood productions, often [exceeding $100 million](https://www.statista.com/statistics/1389936/breakdown-production-budget-hollywood-movies-worldwide/#:~:text=Out%20of%20the%2089%20English,under%20ten%20million%20U.S.%20dollars), executives favor book adaptations, capitalizing on the established fanbases of beloved books. This raises the question: what are the key elements of a successful book-to-film adaptation? Are there specific genres that lend themselves more easily to cinematic adaptation? Is it more effective to adapt recent bestsellers or time-honored classics? And, in light of blockbusters like Harry Potter and Lord of the Rings, should the focus be on serial adaptations rather than standalone novels?
To address these inquiries, we will analyze data from the [CMU Movie Summary Corpus](http://www.cs.cmu.edu/~ark/personas/), [TMDB](https://www.themoviedb.org), [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) and [Goodreads](https://www.kaggle.com/datasets/mdhamani/goodreads-books-100k). Our goal is to use this comprehensive analysis to develop a model that can effectively identify the most promising book for a successful film adaptation.

## Research questions :
**Intro : Why should a movie director adapt a novel into a movie ?**


* Do movies based on books enjoy stronger box office sales?
* How different are the audiences of book adaptation compared to original idea movies ?


**I) Which novels are more likely to be successful in adaptation ?**


* Are there specific genres of novel that lend themselves more easily to cinematic adaptation? 
* What is the ideal time frame between a book's publication and its film adaptation? 
* How does the popularity of the author affects the success of the adaptation ?
* Is it more advantageous to adapt a standalone book or an entire series, as was the case with Harry Potter? 


**II) What is the best way to adapt a novel into a movie ?**


* Do shorter or longer books result in better movies? 
* Should the actors that are playing a role in the movie have a big popularity? (alt : When adapting a book, which actors could be considered ? Which actors are the best at interpreting novel characters ?)



**III) Can we assist production companies in making strategic decisions while adapting novels into movies ?**


* Is it possible to predict if a movie adaptation will gain people’s heart? (alt : What is going to be the next successful book adaptation ?)

## Proposed additional dataset :

The CMU movie summary corpus dataset contains about 80'000 movies with informations like release dates, duration, genre and actors. The dataset is easily readable by the computers of the team. In order to get more informations on the success of the different movies, the IMDb scoring is added to the dataset. Information on the adapted books (if the movies is an adaptation) are also added with Wikidata thank to the wikiID and the Query Service (that uses SPARQL). Here again, the informations like release dates, number of page, genre, author or series belonging are of interest. That way, the characteristics of the book can be compared and linked to the one of the movie and its final success. It is also planed on adding reviews and ratings of books from GoodReads or Kaggle. They could be useful to analyze the popularity of novels and understand why they were chosen to be adapted. Adding all these information don’t give any issue about the size of the dataset as the first stage has been to remove all the movies that were not coming from a book (our dataset contains now around 4000 movies).

## Methods :

First of all, the team familiarized with the dataset and got to know the various features in each dataframes. This first step in our analysis allowed the team to come up with many other ideas and research questions. This lead our team to exploring ideas for which the analysis would require additional data.

In order to extract additional data from the internet, the Wikidata Query Service was used. The wikiID present in the given movie metadata were helpful to retrieve the wikidata page of a movie and determine wether it is based on a book or not. The Query Service was also used to feed the book dataset with various information that could be useful for our analysis. Moreover, the team decided to extract more data on the web, regarding the movies and the books ratings. From the non-commercial dataset available on the Internet Movie Database (IMDb) website was retrieved movie ratings for about 200'000 movies. In order to link this dataset to our current one, the IMDb ID (a.k.a tconst) was extracted from the wikidata pages of the movies. It was therefore easy to merge the two dataframes on this ID, allowing to feed our dataset with additional data from which we could analyse the public appreciation of each movies. Similarly, ratings and reviews of books are added to the dataset from the GoodReads website.

After familiarizing with the dataset and adding it relevant data, the time of data wrangling has come for our team. This step is very important in order to avoid unbiased analysis. The first data wrangling action was done by analyzing the missing data of the various features of our movie metadata. It was observed that information about the box office of many old movies were missing. Carrying out analysis of the performance of movies based on their financial results could therefore be a risk of biased analysis. Hopefully, we retrieved movie ratings which have far less missing data and from which we could base some analysis. 

Two distinct notebooks were created to enhance readability : one for the data collection and data wrangling, called data_wrangling.ipynb, and one for the analysis, called milestone2.ipynb.

Many python libraries will be used in order to perform the data collection and analyses :

* Pandas
* Wikimapper
* …

Different statistical metrics like T-tests, trees, box plot,… will be used  in order to study the data, visualise it and quantify the uncertainty.  

## Proposed timeline : 
* 17.11.23 : project milestone 2
* 24.11.23 : end of that collection and initial organisation
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

## Questions for TAs (optional) :
