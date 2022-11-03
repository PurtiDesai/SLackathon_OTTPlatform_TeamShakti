# Content Diversification through EDA on OTT Platforms  


## Summary

### What's the problem?
The way we consume videos nowadays has undergone massive changes. Now we have multiple OTT platforms such as Netflix, Amazon Prime Video, Disney+ Hotsar, etc. to stream TV shows and movies online. With an overabundance of information and multiple criteria to compare various OTT platforms, it has become increasingly difficult for users to find the best fit for their taste. This is referred to as "choice paralysis" which is causing loss to ott streaming services and is also disappointing to users in search of quality entertainment programs. 
	
### The Idea
The idea is to extract data from various ott platforms to derive meaningful insights based on various fields like genre, ratings, revenues, release year etc. In future, these insights can serve as an input to a prediction model. This model will suggest content creators with most trending creative ideas to achieve best imdb rating and most suitable platform for their content. Furthermore, it can be made available to all through a public platform.


## Section 1: Gathering the data 
Most of the data was available on kaggle. Following are the links from where data has been extracted to create meaningful insights.

https://www.kaggle.com/datasets/shivamb/disney-movies-and-tv-shows  
https://www.kaggle.com/shivamb/netflix-shows  
https://www.kaggle.com/shivamb/amazon-prime-movies-and-tv-shows  
https://www.kaggle.com/datasets/stephanerappeneau/350-000-movies-from-themoviedborg  

## Section 2 : Data Wrangling 
Data wrangling is an essential step, as it contains variety of processes to transform raw data into meaningful information. Its importance is enhanced because it creates a concrete fundamental to base our insights upon. If the data is left as raw, incomplete or faulty , then the accuracy of all derivations becomes questionable.
- Exploring the dataset : Making yourself familiar with the data is a great start to any project. More deeper understanding of trends and patterns in the data results in better yield of output.
- Cleaning : Cleaning can come in different forms including standardizing datatypes, handling missing or null values, and dropping duplicates etc.
- Enriching data : After above steps, it becomes important to evaluate that you have all the necessary data in the final dataset. If not, then one can consider enriching their data from secondary data sources and later merging it all into one logical data structure.
For this project, we went beyond these 3 basic data wrangling steps to handle categorical columns and standardize the "Maturity-rating" column. In order to handle categorical columns, all string datatypes were converted to lowercase to ease the process of avoiding duplicates. While, mapping rating values to corresponding age groups allowed to maintain consistency across data coming from all 3 platforms.

## Section 3: EDA

Given below are visualizations that led to the following insights :

![Diagram1](Images/1-imdb-rating-wise.png)

Above diagram shows the IMDB Rating Distribution for movies on different OTT platforms. It can be briefly concluded that most content on all 3 platforms is rated between 5 to 7 IMDB rate value.

![Diagram1](Images/2-imdb-rating-wise.png)  
A more accurate representation of content division across all platforms based on IMDB ratings. It can be seen that very few (less than 200) movies are marked with the highest IMDB rating possible. 


![Diagram1](Images/3-maturity-rating-wise.png)
Maturity rating defines the class or age group of society that proves to be the best audience for a given content. It is derived that Netflix has more content for 18+ age group whereas Disney Hotstar has most of its content fit for "all" age groups.


![Diagram1](Images/4-maturity-rating-all-platforms.png)
A line graph showing overall distribution of content combining all 3 platforms. Clearly "18+" type of content is most popular amongst all the boards


![Diagram1](Images/5-languages-all.png)
![Diagram1](Images/6-languages-netflix.png)
![Diagram1](Images/7-languages-prime.png)
![Diagram1](Images/8-languages-disney.png)

Colourful pie charts providing a visual treat to analyze most popular language across all media! English being the most common international language continues to top the list. Hindi ranks second being specific to Netflix.


![Diagram1](Images/9-budget-imdb.png)
![Diagram1](Images/10-revenue-imdb.png)

Scatter plot has no definite shape indicating no direct relation between imdb and budget / revenue respectively


![Diagram1](Images/11-directors-all.png)
![Diagram1](Images/12-directors-netflix.png)
![Diagram1](Images/13-directors-prime.png)
![Diagram1](Images/14-directors-hotstar.png)

Director is the one who visualizes the story and makes it come alive on the white screen! Above graph shows top directors to have most of their content published on these platforms.
Jay Chapman leading across all boards with more than 30 movies currently running on OTT. Steven Spielberg and John English are ranked as most popular on Netflix and Prime respectively. However, Charles Nichols and Paul Hoen share the title for Disney+ Hotstar


![Diagram1](Images/18-actor-wise.png)

The honorable title for best actor goes to Shah Rukh Khan! Significantly being the most popular actor across all boards, genres and languages. Re-iterating that this data has been biased and collected from Indian audience, it wasn't a surprise that SRK topped the list.

![Diagram1](Images/19-genre-wise.png)

Genre wise comparison is an extremely critical information for content creators to see what type of genre is being consumed at large. Since this data is majorly extracted from Indian audience, Drama category undoubtedly tops the list for both - Netflix and Prime. Hotstar is for people who prefer 'Family' type content for their entertainment. History, War and Music are some of the least favorites for audiences of all age groups.

## Section 4: Conclusion:
1. English is the most commonly communicated language throughout different audiences and countries.
2. Shah Rukh Khan was and is the King Khan of bollywood. He is the most viewed actor across all platforms.
3. It can be isolated that audience is more attracted towards Netflix and Prime as compared to Hotstar in current times. 
4. Although 18+ content is most easily available on Netflix, people from all age groups are religiously watching OTT content.

## Section 5: Future Roadmaps
These insights have been analyzed to draw conclusions to help content creators. It is designed so to help them identify trends and what type of content is most liked with respect to genre, language or maturity-rating. 
Furthermore, it can serve as input for a recommendation model that predicts whether a certain piece of content can become a blockbuster hit or not! Various ensemble learning techniques can help built an interactive and easy to use model. It can also be made publicly available to producers, directors or individual content creators.