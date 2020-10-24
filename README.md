# Microsoft Movie Studio Case Study

<img src= 
"images/movies.jpg" 
         alt="Movie Logo Image" 
         align="right"> 

Flatiron Data Science Project - Phase 1  
Prepared and Presented by:  **_Asher Khan_** and **_Melody Peterson_**  
Presentation PDF: here  

### Business Problem    
Microsoft has decided to create a new movie studio, but the problem is they don't know anything about creating movies.  They have hired us to help them better understand the movie industry.  We will explore what type of films are currently doing best at the box office and translate those findings into actionable insights to help decide what type of films to create. 

### Data    
We have been provided data from Box Office Mojo, IMDB, Rotten Tomatoes, TheMovieDB.org, and The-Numbers.com.  We have also chosen to use a database downloaded from OpusData that includes information on movies meeting the following criteria:  production year between 2006 and 2018, production budget greater than or equal to $10 million, figures for domestic or international box office. 

### Questions Explored  
#### How have box office returns been changing over time?  
Here we have taken a high level look at box office sales for movies over time, both domestic and international, to establish an expectation for Microsoft's projected sales revenue.  Data is used from the Opus Movie Data dataframe and includes movies with the following attributes: production year between 2006 and 2018, figures for domestic or international box office, production budget greater or equal to $10 million.  We can see from the graph below that there is a definite increase in box office sales over time. To truly be able to know if the industry is growing however, we would want to account for inflation over the years. Also measuring profit instead of gross sales would ensure us that movies are not costing so much more to make now that it is overshadowing the increase in revenue.  
[View the data calculation notebook](https://github.com/melodygr/microsoft_movie_analysis/blob/main/Notebooks/Box_Office_Trends.ipynb "Box Office Trends Notebook").  
![alt text](https://github.com/melodygr/microsoft_movie_analysis/blob/main/images/avg_gross.png "Avg Box Office Trends Graph")  

#### Which studios are the biggest competitors? 
We established a rank order of world-wide gross revenue (in millions) for all studios and then examined the top 20 studios. As a comparison, we also calculated the top 100 grossing movies and measured which studios produced them.  Data from Box Office Mojo was provided.  Buena Vista, Fox, and Warner Brothers top our list of highest grossing studios according to this dataset. And Buena Vista received the majority of its world-wide box office revenue from the top 100 blockbuster hits. This would certainly indicate that Buena Vista is the competitor to watch. Interestingly, however, the name Buena Vista was discontinued as a trade name in 2009 by its' parent owner Walt Disney Studios, bringing into question the timeliness of our dataset. Further research into each studio is recommended as well as an analysis of the studios' performance over time.  

[View the data calculation notebook](https://github.com/melodygr/microsoft_movie_analysis/blob/main/Notebooks/Studio_Competition.ipynb "Studio Competition Notebook")  
![alt text](https://github.com/melodygr/microsoft_movie_analysis/blob/main/images/studios.png "Studio Graph")

#### Which movie genres are the most popular?  
Popularity can be determined in many ways. In this analysis, we looked at how popular a movie genre is to produce, as evidenced by how many movies of each genre are made. Then we also looked at how popular a movie genre is to consumers, based on the TheMovieDataBase popularity score, from the tmdb_movies_df dataset.  We established a rank order of how many movies are in each genre as well as calculated the percentage of movies with the given genre attribute, since many movies have multiple genres. We then calculated each genres' average popularity according to the TMDB popularity score given to each movie in the category.  The top three movie genres produced during the time period of this dataset are Drama, Comedy, and Documentary. But, if the popularity attribute is to be believed, people prefer the movie genres of Adventure, Action, and Fantasy.  We would like to compare actual box office gross to these figures to see if popularity actually results in higher gross. But if we assume it does, then Microsoft should consider producing Adventure, Action, and Fantasy films. We should also consider analyzing if movie genre popularity has been changing over time.

[View the data calculation notebook](https://github.com/melodygr/microsoft_movie_analysis/blob/main/Notebooks/Genre_Popularity.ipynb "Genre Popularity Notebook").  
![alt text](https://github.com/melodygr/microsoft_movie_analysis/blob/main/images/popularity.png "Genre Popularity Graph")

#### Has the average cost for production increased, decreased or remained the same throught the years?  
For this analysis we combined two dataframes: the Opus Movie Data cross-referenced with The Numbers Movie Budgets data. The average production cost of movies has been increasing throughout the years.  If microsoft is considering long term production projects, it is important to keep in mind the production cost of future projects will be more.  

[View the data calculation notebook](https://github.com/melodygr/microsoft_movie_analysis/blob/main/Notebooks/Box_Office_Trends.ipynb "Visualizations Notebook").  
<p align="center">
<img src="https://github.com/melodygr/microsoft_movie_analysis/blob/main/images/budget.png" alt="Budget Graph" width="600" height="350">
</p>

#### What is the corrolation between average production budget and total revenue? 
The average total revenue throughout the years has also increased with production cost. This direct corrolation could be possibly just be because of inflation in general costs.

[View the data calculation notebook](https://github.com/melodygr/microsoft_movie_analysis/blob/main/Notebooks/Box_Office_Trends.ipynb "Visualizations Notebook").  
<p align="center">
<img src="https://github.com/melodygr/microsoft_movie_analysis/blob/main/images/budget_and_revenue.png" alt="Budget and Revenue Graph" width="600" height="350">
</p>

### Conclusions  
Descriptive conclusions and recommendations

### Next Steps / Future Work  
Others things that could be done to improve analysis

