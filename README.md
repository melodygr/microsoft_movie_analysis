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
#### Which studios are the biggest competitors? 
We established a rank order of world-wide gross revenue (in millions) for all studios and then examined the top 20 studios. As a comparison, we also calculated the top 100 grossing movies and measured which studios produced them.  Data from Box Office Mojo was provided.  Buena Vista, Fox, and Warner Brothers top our list of highest grossing studios according to this dataset. And Buena Vista received the majority of its world-wide box office revenue from the top 100 blockbuster hits. This would certainly indicate that Buena Vista is the competitor to watch. Interestingly, however, the name Buena Vista was discontinued as a trade name in 2009 by its' parent owner Walt Disney Studios, bringing into question the timeliness of our dataset. Further research into each studio is recommended as well as an analysis of the studios' performance over time.  

[View the data calculation notebook](https://github.com/melodygr/microsoft_movie_analysis/blob/main/Notebooks/Studio_Competition.ipynb "Studio Competition Notebook")  
![alt text](https://github.com/melodygr/microsoft_movie_analysis/blob/main/images/studios.png "Studio Graph")

#### Which movie genres are the most popular?  
Popularity can be determined in many ways. In this analysis, we looked at how popular a movie genre is to produce, as evidenced by how many movies of each genre are made. Then we also looked at how popular a movie genre is to consumers, based on the TheMovieDataBase popularity score, from the tmdb_movies_df dataset.  The top three movie genres produced during the time period of this dataset are Drama, Comedy, and Documentary. But, if the popularity attribute is to be believed, people prefer the movie genres of Adventure, Action, and Fantasy.  We would like to compare actual box office gross to these figures to see if popularity actually results in higher gross. But if we assume it does, then Microsoft should consider producing Adventure, Action, and Fantasy films. 

[View the data calculation notebook](https://github.com/melodygr/microsoft_movie_analysis/blob/main/Notebooks/Genre_Popularity.ipynb "Genre Popularity Notebook").  
![alt text](https://github.com/melodygr/microsoft_movie_analysis/blob/main/images/popularity.png "Genre Popularity Graph")

#### Which movie ratings provide the highest box office returns?  
Here we have taken a high level look at box office sales for movies over time, both domestic and international, to establish an expectation for Microsoft's projected sales revenue.  Data is used from the Opus Movie Data database.  Looking at average movie revenue by year we can see a definite increase in box office sales over time. Most of the movies in our dataset are rated either PG-13 or R.  Making the assumption that the same ratio is true for all movies produced, when we look at the average movie revenue by rating, we see that the top grossing movie ratings are PG, followed by G, and then PG-13.  These would be the ratings that Microsoft should focus on as they generate the most revenue.  For better results, we would need to know that our dataset is representative of the entire population of movies produced in this time period.  Instead, what we know is that this data is only for movies with a production budget over $10 million.  

[View the data calculation notebook](https://github.com/melodygr/microsoft_movie_analysis/blob/main/Notebooks/Box_Office_Trends.ipynb "Box Office Trends Notebook").  

![alt text](https://github.com/melodygr/microsoft_movie_analysis/blob/main/images/count_and_avg_by_rating.png "Count and Avg Box Office by Ratings Graph")  

#### Has the average cost for production increased, decreased or remained the same throught the years?  
For this analysis we combined two dataframes: the Opus Movie Data cross-referenced with The Numbers Movie Budgets data. The average production cost of movies has been increasing throughout the years. The production cost had a steady growth up until the 1990's when the production cost started to grow rapidly.  If Microsoft is considering long term production projects, it is important to keep in mind the production cost of future projects will be more.

[View the data calculation notebook](https://github.com/melodygr/microsoft_movie_analysis/blob/main/Notebooks/Visualizations.ipynb "Visualizations Notebook").  
<p align="center">
<img src="https://github.com/melodygr/microsoft_movie_analysis/blob/main/images/budget.png" alt="Budget Graph" width="600" height="350">
</p>

#### What is the correlation between average production budget and total revenue? 
The average total revenue throughout the years has also increased with production cost. In the mid 1900's there were two particular movies that grossed more than expected: "Snow White" This direct correlation could possibly just be because of inflation in general costs. However, Microsoft should consider producing multiple movies simultaneously in order to avoid high production costs in the future; meanwhile spreading out the movie release dates in order to maximize revenue.

[View the data calculation notebook](https://github.com/melodygr/microsoft_movie_analysis/blob/main/Notebooks/Visualizations.ipynb "Visualizations Notebook").  
<p align="center">
<img src="https://github.com/melodygr/microsoft_movie_analysis/blob/main/images/budget_and_revenue.png" alt="Budget and Revenue Graph" width="600" height="350">
</p>

### Conclusions  
The movie industry appears to still be growing every year, both in budgets and revenue.  While there are many players in the industry, a top few, including Walt Disney Studios, appear to be the ones to watch.  Movie-goers prefer movies in the Action, Adventure, and Fantasy genres, although these are not the most produced movies.  In that vein, the highest grossing moving ratings are PG, G and PG-13, yet these also are not the most produced movies.  Microsoft should consider producing movies based on what market research indicates that movie-goers actually want to watch.

### Next Steps / Future Work  
To truly be able to know if the industry is growing, we would want to account for inflation over the years.  Also, measuring profit instead of gross box office sales would ensure us that movies are not costing so much more to make now that it is overshadowing the increase in revenue. Further research into each studio is recommended as well as an analysis of the studios' performance over time.  Gross revenue and profitablity of popular genres and movie ratings should be examined with current data.  We should also consider analyzing if movie genre or rating popularity has been changing over time.

