# Top Movies

This is a simple repository that allows you to define your top movies in a simple CSV format.  Your movie likes are then aggregated together using the github API (we walk the forks) to determine aggregate scores.

## How to Score Your Movies

Simply, fork this repository, and start entering data into the `movies.csv` in the following format:

```
movie title (as recorded on imdb),points
```

At this stage, the algorithm we are playing with allows you to distributed a total of 50 points across all the movies in your list, and the most that can be allocated to a single movie is 5 points.  This is not a rating score, but just how much you liked it compared to the other movies in your list.

Additionally, in the interests of being terse you don't need to ascribe a particular points figure to a movie if you don't want to.  In these cases, the points attributed to that movie will be the total number of unallocated points, divided by the number of movies in your list (up to a maximum of 5, with no more than 50 points being allocated).

