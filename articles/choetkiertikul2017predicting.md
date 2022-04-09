# JIRA-Estimation-Prediction - agile sprints 
Source: https://github.com/jai2shukla/JIRA-Estimation-Prediction/tree/master/agile%20sprints


## Analysis
* They found several works on effort estimation model to predict the effort required for the entire project (citation 5, 6 and 7).
* Other work found looked only at how prediction is done at a project level (8, 9, 10, 11, 12)
* They therefore suggest to look at the iteration level, something we aim at as well.
* Going one level down is of course looking at risk at a user story level.
* 3834 sprints from 5 large open source projects with a total of 56687 user stories.
* When using some of these data sets, of course we can expand on those numbers by getting the most recent data of those projects
* 15 attributes used for features of the iteration
* 12 attributes used for features of the user stories
* additionally, a graph was created describing the dependency between these user stories, which is used as a feature for the iteration.
* attributes from a set of user stories inside an interation are aggregated statistically to create another group of features for the iterations.
* they then created models to predict the delivery capacity of an iteration.
* it is based on 3 randomized ensemble methods: random forests, stochastic gradient boosting machines and deep neural networks with dropouts.
* the model outperforms the common baselines and well across all case studies.
* "In our previous work [14] we developed models for characterizing and predicting delays at the level of issues. [...] This work, in contracts, aims to predict the quantum of achieved works at the level of iterations [...]. Here, we leverage feature/representation learning techniques which were not used in those previous works."


## Research gap
* This research suggests looking at user stories individually, as 
* future works suggests incorporating more features such as team structure, developrs skill and workload.

<!-- ## Data structure
```
Features of ...
│
└───Iteration
│     * duration in days
│     * no. issues at start of iteration
│     * story points at start of iteration
│     * no. issues added during
│     * story points added during
│     * no. of issues removed during
│     * story points removed during
│     * no. of todo issues
│     * story points todo issues
│     * no. in-progress issues
│     * story points in-progress issues
│     * no. of done issues
│     * story points done
│     * no. of scrum masters
│     * no. of team members
│   
└───Issue
│     * type
│        │  task
│        │  bug
│        │  new feature
│        │  improvement
│        │  story
│     * priority
│        │  high
│        │  medium
│        │  low
│     * no. of comments
│     * no. of affect versions
│     * no. of fix versions
│     * issue links
│     * no. of blocking issues for this
│     * no. of blocked by this
│     * no. of changes fix version
│     * no. of changes priority
│     * no. of changes description
│     * description read ability index
│   
└───Feature aggregation 
    (of story points from features inside iteration)
      * min
      * max
      * mean 
      * median
      * std
      * var
      * range
      * frequency
``` -->
