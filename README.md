# Team0110 - ADA Project


##Milestone P1

Dataset : Movies
Project ideas : 
  1) [MIRCO] Women in movies:
  Use the dataset to measure the condition of women in the society. Two levels are observable: A technical one, and an artistic one. The technical one consists in analyzing the women implication in the movies industry (actresses, producers, directors). The artistic one is to perform a similar analysis, but on the content of each movies (charactresses, genre, main role, second role). This data could be compared to men implication in the industry. The time evolution is the interesting part, where one can assess whether some real world event triggered anything in the movies/art industry. The database must be enlarged by using wikidata dumps. Fortunately, the database already contains links to wikidata for each movie!

Feedback: Good idea, original and good exposition of how you are going to carry out the study. Very good idea to add more data to enrich the current dataset.

  2) [MIRCO] Assessing the policy of authors:
  The question "Who is the author of a movie?" was a large debate in the 1950's. French film critics decided to assume that the film director was the author. However, this decision is questionable. Large production companies play a key role in the industry. Producers often come up with their own movie idea and just ask a director to simply do what the company wants. In this case, directors are more considered as random technicians, "Yes men" more than authors. The french film critics noted that a movie tends to receive more awards when the movie is an original idea of the director, thus litterally making him the author. The goal of the study is to assess the impact and/or validate the policy of authors on a film. A whole range of data can be used; The production company, The budget, the number of awards, the genre, the time period as well as the actors may influence whether a director is really the author and if the relation ship self-author vs. popularity is true. Again the database is enlarged using wikidata

Feedback: Very original idea that can lead to a great data story if interesting results are found. It expresses well the data you are going to use. If you focus on a single country like France, make sure that the dataset is big enough. You also have to define a good way to distinguish which film is auteur and which is "technical", an element that can be subjective and not easy to evaluate on a large scale.
   
  3) [MIRCO] Evolution of the Science-fiction genre:
  Since by definition, science fiction movies try to perform a socio-technical critic of the society, the evolution of the topics is continuous and related to society events. The idea of this project would be to extract main topics or subjects addressed in Sci-fi movies using the movie description, as well as additional wikidata and ratings. The main topics of Sci-fi movies are often related to technology. One could then observe the evolution of society concerns about technology through the whole Sci-fi movies corpus. For example, one approach could talk about the human replacement by "Machines": The first sociological concerns came up with the rise of massive industrialization. Humans feared to be replaced by machines in their jobs. The subject then evolved with the advances in robotics, where technology replaced human bodies. Finally, with advances on artificial intelligence, people feared to have their "mind" replaced. All this fear of losing one's identity has thus been the main subject of Sci-Fi movies. Through the extracted data, one could assess and compare the movies' topics evolution with the technology evolution. The correlation between social implication in these movies and the popularity of Science-Fiction may also be assessed using ratings and box office income.

Feedback: Another concrete and original idea. This study will involve using NLP techniques to extract information from reviews if you want to understand how society was involved in the film and may lead to a more complex project if you do not master this field. In any case, the idea has a lot of potential. Your project mentor throughout the semester will be Saibo Geng : saibo.geng@epfl.ch. For future discussions specific to your P2 and P3 deliverables, you are encouraged to be in touch with your mentor.

JUSTIN :

Men and Women inequality in the cinematographic industry : 

This subject investigates the question of gender inequality in the film industry. It could focus on the disparities in areas like on-screen representation, behind-the-scenes roles, pay or awards. The evolution of these quantities can also be studied through time in order to see (or not) if there is a better equality now. The use of the wikipedia page of the films could help to find the different roles (first role, director, …).


The impact of the 3D technology in the cinematographic industry

This subject explores the transformative effects of 3D technology on the film industry. It could dive into the evolution of 3D cinema with the difference between the number of entry for the same 3D and 2D film and the evolution of the economy (budget and benefit). The global opinion (from the public and from the « professionals » with awards) could also be a good metric, with its evolution (big interest when the technology came out but then quick lack of it).  The use of the wikipedia page of the films (and the web site imdb) may be required to help as another dataset to add informations.

The biography of Leonardo di caprio through the cinematographic industry

This subject offers a compelling exploration of the life and career of Hollywood icon Leonardo DiCaprio. It delves into his early beginnings, filmography, award recognition and evolution as an actor, impact on the industry (success of the films where he played). By weaving his personal and professional story, the research provides an engaging portrait of an actor who has left an indelible mark on both the cinematic world and global causes. Of course this subject could focus on other actors but for the time frame offered by the dataset, Di Caprio seems to be a good choice. Also here, the use of the wikipedia page of the films may be required to help as another dataset to add informations. 

#######################################################

ROMAIN :

Movie success and award : This idea aims to try to make a predictive analysis of the performance of a movie, based on multiple parameters, such as the actors popularity, the producer achievements, and even more precise features such as genre, runtime, release date, languages, and the movie country. The goal would be to use the data to make links between these parameters and find insights about the factors that make a successful movie. We can wonder, for instance, what makes a film win an award ? how to produce a movie that most people will like ? Additional information, such as the review scores of the films, could be extracted from Wikidata to help answering these questions.

Influence of the world on movie production : The goals of this project would be to analyse the evolution of movie production over the years. We can ask ourselves how political, social, or cultural events happening all over the world influence the types of films. The idea would be to inspect the change in genre and the runtime of the movies produced, to find how it would be related to social evolution over time. We can wonder : what kind of movies did people enjoy in the 1950’s ? in the 1970’s ? Can we relate people preferences to a particular event that happened at the same time ? The influence of politics could also be inspected, by analysing the genre of the movies and the languages, in order to find out how movies can be used as soft power. 

Cultural influence on genre : This project would aim to investigate the influence of the language and cultural factors on the success of different movie genre in several regions of the world. The goal would be to conduct a statistical analysis in order to identify correlations between the languages of the movies, the genre and the production country.  It would allow to get insights on the cultural sensitivity to a certain movie genre, and to understand how cultural affiliation impacts the interests of the people. We can ask ourselves if a genre has more success when the language of the original version corresponds to the language of the audience, and if we can detect some exceptions.

#######################################################

LUCAS : 

Analysis of the evolution of an actor's career : This problematic aims at investigating actor's recognition through their career. Exploring the dataset, we will try to understand what are the factors that contribute to their popularity growth or decay. We can ask ourselves if their popularity is linked to roles they play in successful movies or if it is based on the number of apparition in movies. We could also examine whether there are gender-based differences in the timing and longevity of an actor's prime. Are male and female actors affected differently by age and career stage in the industry ?

Adaptation of novels and real-life stories in movies : From the wikidata page of movies, one could extract the original source of a movie. Therefore, the idea would be to explore the success of novel or real-life story based movies and how well they are adapted based on the critics of movie medias and of the audience. To what extent does a movie adaptation arouse the interest of the audience ? Do certain genres such as science fiction, romance, or mystery, have a higher adaptation success rate ? We would need to recover reviews of movies as well as reviews of the corresponding novel. The most valuable reviews would be those from people who have seen the movie adaptation of the novel they previously read. We could therefore create an indicator that quantify the adaptation success and analyse their financial performance.

Releasing Strategies : Investigate the various release strategies to maximize the financial performances of a movie. For example, one could look into how the release date and season of a movie influence its success. Does the timing of release affect box office performance or critical reception? We can ask ourselves whether releasing a movie at "quiet" times of the year could be a good strategy. Can it attract most of the audience and therefore financially perform better ? We could also discuss the role of marketing in a movie's financial performance. Is there a correlation between the marketing strategy of a movie and its financial performance and popularity. To do so, we would have to collect precise data about the budget management of movies, which could be tideous and some of these data may not be accessible.


#######################################################

Nils : 

Idea 1: From Book to Motion Picture: Deciding the Next Book-to-Film Adaptation
Filmmakers have long turned to literature for creative inspiration, with iconic films like James Bond and "The Shining" having their roots in books. As this trend persists, it begs the question: what constitutes a successful transition from book to film? Are there specific genres that lend themselves more easily to cinematic adaptation? Do shorter or longer books result in better movies? Is it more advantageous to adapt a standalone book or an entire series, as was the case with Harry Potter? Do movies based on widely-read books also enjoy strong box office sales? What is the ideal time frame between a book's publication and its film adaptation? Should the book's authors play a role in the movie's production? To take this a step further, we could even develop a predictive model to gauge the potential success of future book-to-film adaptations, thereby identifying books that would make excellent movies.

Idea 2: The Disney Dominance: Shaping the Cinematic Landscape
In recent years, Disney has emerged as the colossal force in the entertainment industry, acquiring renowned studios like Pixar, Marvel, Lucasfilm, and 21st Century Fox. With such acquisitions, Disney's influence on the cinematic landscape is undeniable. But does this influence also extend to the movies the acquired studios produce? Have there been noticeable shifts in the genres and themes of their films? Given Disney's historical focus on family audiences, have the movies from these studios become more family-friendly? Furthermore, has the backing of the Disney brand contributed to greater box office success for these studios? And even more broadly, can we identify any specific patterns or trademarks in films that fall under the Disney umbrella?

Idea 3: The Evolution of Villains
Movies are a reflection of their times, often mirroring the prevailing sentiments, fears, and biases of the society in which they are produced. Historically, major geopolitical events, particularly those involving the United States, have had a profound impact on how villains are portrayed in Hollywood. For example, consider "Rocky 4," made during the height of the Cold War, where the American hero faces off against a seemingly unbeatable Russian foe, Drago, epitomizing the U.S.-Soviet tensions of the time. Similarly, the landscape of villainy in cinema underwent a transformation following the events of 9/11, reflecting the altered political and social climate. This leads us to question: what common stereotypes characterize movie villains? What drives them, and what are their objectives? Does the influence of real-world geopolitical events find its way into these fictional narratives? And are there other discernible trends in the portrayal of villains over time?




Dataset : Youniverse
Project ideas :
  1) Youtuber colaborations : through the descriptions we might infer other liked youtubers indicating some sort of collaboration. We can research if collaboration helps gain subscribers.
  2) Title analysis : How does a title effect the popularity of a video ? Are there words that have a significant effect ? Did the titles evolve over time ?
  3) Gaming analysis : Focusing only on videos from gaming branch. From the video titles, infer the game title. Then see if popularity on youtube affects users and resell data.
  4) Tag analysis : what kind of tags, how many tags to get more view ? Are they linked to the video content ? What are the evolution of popular tags over time.
  5) How to become the best Youtuber : the youtuber's guide (typically takes all the other ideas to get the best channel).
  6) Audience target : what are the age/sexe of the targeted audience.
  7) Advertisement : evolution of the importance of partnership in videos (from title and description), in what kind of videos ? How many subscribers to get a partership.
  8) Animals on Youtube : what animal would be the best youtuber ?
  9) Politics : impact of presidential elections in the US (Trump/Clinton in 2017) on the videos, assessing popularity of candidates thanks to the videos.
  10) Could Youtube remplace school ? : analyze the education/vulgaristation videos, what subject is the most present ? Can I become enginer on Youtube ? What job can I get from Youtube (backer, cooker)? 

# Milestone 2

**From Book to Motion Picture**

## Title : 
**What makes a book adaptation a good movie ?**

## Abstract : 
Deciding the Next Book-to-Film Adaptation Filmmakers have long turned to literature for creative inspiration, with iconic films like James Bond and "The Shining" having their roots in books. The idea would be to study the common points between the adaptations through history. 

## Research questions : 
* Are there specific genres that lend themselves more easily to cinematic adaptation? 
* Do shorter or longer books result in better movies? 
* Is it more advantageous to adapt a standalone book or an entire series, as was the case with Harry Potter? 
* Do movies based on a books enjoy stronger box office sales? 
* Do movies based on widely-read books also enjoy strong box office sales? 
* What is the ideal time frame between a book's publication and its film adaptation? 
* Should the actors that are playing a role in the movie have a big popularity?
* Is it possible to predict if a movie adaptation will gain people’s heart?

## Proposed additional dataset :
The CMU movie summary corpus dataset contains 42306 movies with informations like release dates, duration, genre and actors. The dataset is easily readable by the computers of the team. In order to get more informations on the success of the different movies, the IMDb scoring is added to the dataset by using an existing python function. Informations on the adapted books (if the movies is an adaptation) are also added with Wikidata thank to the wikiID and the Query Service (that uses SPARQL). Here again, the informations like release dates, number of page, genre, author or series belonging are of interest. That way, the characteristics of the book can be compared and linked to the one of the movie and its final success. Adding all these informations don’t give any issue about the size of the dataset as the first stage has been to remove all the movies that were not coming from a book ( our dataset contains now around 4000 movies).

## Methods :

As informations (on box office mainly) on many old movies are missing, the dataset may need to be narrowed down to films before a certain release date. 
Two distinct notebooks will be created to enhance readability : one for the data collection and one for the analysis.

Many python libraries will be used in order to perform the data collection and analyses :

* Pandas
* Wikimapper
* …

Different statistical metrics like T-tests, trees, box plot,… will be used  in order to study the data, visualise it and quantify the uncertainty.  


## Proposed timeline : 
17.11.23 : project milestone 2
24.11.23 : end of that collection and initial organisation
01.12.23 : visualisation of results
08.11.23 : quantification of error and uncertainty of the results
15.11.23 : end of the code
22.11.23 : end of website (project milestone 3)

## Organisation within the team :
Mainly organized in group of two for each task
Nils : data collection, data organisation
Mirco : data collection, Statistical analysis
Romain : Statistical analysis, website
Lucas : website, Data visualisation 
Justin : Data visualisation, Data organisation

## -Questions for TAs (optional) :