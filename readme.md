## Recommendations Rank & Knowledge Based: 

### Part I: How To Find The Most Popular Movies

For this notebook, we have a single task.  The task is that no matter the user, we need to provide a list of the recommendations based on simply the most popular items.

For this task, we will consider what is "most popular" based on the following criteria:

* A movie with the highest average rating is considered best
* With ties, movies that have more ratings are better
* A movie must have a minimum of 5 ratings to be considered among the best movies
* If movies are tied in their average rating and number of ratings, the ranking is determined by the movie that is the most recent rating

With these criteria, the goal for this notebook is to take a **user_id** and provide back the **n_top** recommendations.  Use the function below as the scaffolding that will be used for all the future recommendations as well.

### Part II: Adding Filters

Now that we have created a function to give back the **n_top** movies, let's make it a bit more robust. We'll Add arguments that will act as filters for the movie **year** and **genre**.  

We'll Use the cells below to adjust our existing function to allow for **year** and **genre** arguments as **lists** of **strings**.  Then the ending results are filtered to only movies within the lists of provided years and genres (as `or` conditions).  If no list is provided, there should be no filter applied.

You can adjust other necessary inputs as necessary to retrieve the final results you are looking for!

```
popular_recs_filtered('1', 20, years=['2015', '2016', '2017', '2018'], genres=['History', 'Comedy'])
```