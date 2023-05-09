# MovieExploration
Exploring the making of magnificent movies!

## Aim

“You gotta watch it! It’s an instant classic! I don’t care what Rotten Tomatoes says.”
 
 Coworker, every two months about the movie ‘Infinite’
 
“Did you see the new Top Gun movie? That Tom Cruise is so handsome.”
 
 Grandma, three times in the same conversation
 
“What should we watch tonight?”

Girlfriend, every night - usually followed by “What should we eat.”
 
Selecting the perfect movie to watch has become somewhat of a tradition in American culture.
Sifting through various streaming services, trying to find that one title that is right is an agonizing
and tedious process that most would rather avoid. During this process, it is common to search
reviews to determine what others recommend. One of the most popular online sources that
ranks titles is the Rotten Tomatoes Tomatometer. The Tomatometer was created to separate
the good movies from the bad movies in an effort to help viewers determine what to watch. A
film’s Tomatometer score is determined by numerous movie critic reviews. The categories
within the score are Rotten for movies with poor reviews, Fresh for movies with good reviews,
and Certified Fresh for movies with consistently excellent reviews. It appears the Tomatometer
usually gets it right, with movies like Top Gun receiving a Certified Fresh, while movies like the
dreadful Fool’s Gold receiving a Rotten. However, there are some movies, such as epic cult
classic Space Jam, that have clearly been unfairly categorized as Rotten (though it is important
to note the correct categorization of Space Jam 2 -- Rotten). Furthermore, It is painful to think of
the millions of people tricked into spending two and a half hours watching Certified Fresh-- Star
Wars: The Last Jedi only to be majorly disappointed. Some of these head scratchers could
make one wonder how the critics come up with this stuff, and what other factors could influence
a movie’s Tomatometer score. Thus, the aim of this exploration is to determine different movie
characteristics associated with the Tomatometer, and to use Bayesian statistics to create
models that can predict Tomatometer score. Hopefully, we can then use our insight to better
determine what movies are good and what movies are bad, making the movie selection process
a lot less painful.

## Executive Summary
We tackle the problem of defining a probability distribution for our outcome variable: the critics’
rating of a particular film. More specifically, we will categorize each movie using the critics_score
variable, which uses three ratings, each summarized above: Rotten, Fresh, and Certified Fresh.
Our goal is to predict which movies received higher ratings by extracting their biggest sources of
variance via data exploration. Using these as the categories of our response, we will explore
relationships and trends within our remaining dataset to find the best combination of covariates
to include in our final models. We take a Bayesian logistic regression modeling approach at first
to see how one of the most tried and true methods of machine learning classification performs
on our relatively small dataset. Further, we binarize our outcome variable and rerun a Bayesian
logistic regression model with only our most important covariates to improve our results.
Enhancing results from that of a logistic regression, we finally extend our analysis into Bayesian
Additive Regression Trees as a bootstrapping method to combine many simple regression trees
together to estimate a robust posterior probability distribution. We conclude that audience
scores of movies have the largest magnitude of impact on critics rating. More specifically, a
higher audience score on average calls for a higher critics rating on a given movie.
