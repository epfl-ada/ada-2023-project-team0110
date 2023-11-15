# Team0110 - ADA Project

# Milestone 2

## Title : 

**From Book to Movie : a analysis of book adaptation to the cinema industry**

## Abstract : 
The goal of this project is to understand the success of novel adaptation in cinema. Can we predict which recent novels are going to be adapted in cinema ? 

The motivation behind this project was to understand why movie directors were tending to adapt novels. Are they attracted by the potentially larger audience ? Or are they interested by the artistic challenge of adapting literature into a visual medium ?
Some of our group members are regular novel readers and wondered why some novels were not adapted. This project aims at analyzing what type of novel makes a successful adaptation.
And finally, the motivation of this project is to create a predictive model. Could this assist production companies in making strategic decisions while adapting novels into movies ?  

We would like to tell a story about the history of novel adaptation in cinema and its evolution with time. The idea would be to analyze the data to investigate the public reception to these adaptation and answer the problematic : What makes a book adaptation a good movie ?

NILS : 

Ever since the advent of cinema, filmmakers have drawn inspiration from books. From 1968 to 2002, [35% of all English-language films originated from books](https://www.frontier-economics.com/media/vyfd1iz3/publishings-contribution-to-the-wider-creative-industries.pdf). Particularly in high-stakes Hollywood productions, often [exceeding $100 million](https://www.statista.com/statistics/1389936/breakdown-production-budget-hollywood-movies-worldwide/#:~:text=Out%20of%20the%2089%20English,under%20ten%20million%20U.S.%20dollars), executives favor book adaptations, capitalizing on the established fanbases of beloved books. This raises the question: what are the key elements of a successful book-to-film adaptation? Are there specific genres that lend themselves more easily to cinematic adaptation? Is it more effective to adapt recent bestsellers or time-honored classics? And, in light of blockbusters like Harry Potter and Lord of the Rings, should the focus be on serial adaptations rather than standalone novels?
To address these inquiries, we will analyze data from the [CMU Movie Summary Corpus](http://www.cs.cmu.edu/~ark/personas/), [TMDB](https://www.themoviedb.org), [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) and [Goodreads](https://www.kaggle.com/datasets/mdhamani/goodreads-books-100k). Our goal is to use this comprehensive analysis to develop a model that can effectively identify the most promising book for a successful film adaptation.

## Research questions :
* Why should a movie director adapt a novel into a movie ?
    * Do movies based on books enjoy stronger box office sales?
    * How different are the audiences of book adaptation compared to original idea movies ?

* Which novels are more likely to be successful in adaptation ?
    * Are there specific genres of novel that lend themselves more easily to cinematic adaptation? 
    * What is the ideal time frame between a book's publication and its film adaptation? 
    * How does the popularity of the author affects the success of the adaptation ?
    * Is it more advantageous to adapt a standalone book or an entire series, as was the case with Harry Potter? 

* What is the best way to adapt a novel into a movie ?
    * Do shorter or longer books result in better movies? 
    * Should the actors that are playing a role in the movie have a big popularity? (alt : When adapting a book, which actors could be considered ? Which actors are the best at interpreting novel characters ?)

* Can we assist production companies in making strategic decisions while adapting novels into movies ?
    * Is it possible to predict if a movie adaptation will gain people’s heart? (alt : What is going to be the next successful book adaptation ?)

## Proposed additional dataset :

The CMU movie summary corpus dataset contains about 80'000 movies with informations like release dates, duration, genre and actors. The dataset is easily readable by the computers of the team. In order to get more informations on the success of the different movies, the IMDb scoring is added to the dataset. Information on the adapted books (if the movies is an adaptation) are also added with Wikidata thank to the wikiID and the Query Service (that uses SPARQL). Here again, the informations like release dates, number of page, genre, author or series belonging are of interest. That way, the characteristics of the book can be compared and linked to the one of the movie and its final success. It is also planed on adding reviews and ratings of books from GoodReads or Kaggle. They could be useful to analyze the popularity of novels and understand why they were chosen to be adapted. Adding all these informations don’t give any issue about the size of the dataset as the first stage has been to remove all the movies that were not coming from a book (our dataset contains now around 4000 movies).

## Methods :

Data wrangling is conducted in order to carry out unbiased analysis. As information (on box office mainly) on many old movies are missing, the dataset may need to be narrowed down to films released after a certain date. This would allow to avoid any biased analysis generated by missing data.
Two distinct notebooks will be created to enhance readability : one for the data collection and one for the analysis.

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
