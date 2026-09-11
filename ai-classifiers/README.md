# ai-classifiers



### Project Overview

This repo gets into the nuts and bolts of four classic classification (and clustering) algorithms: k-nearest neighbors, k-means, naïve Bayes, and hierarchical clustering. Each is tried first on simple 2D data, and, if possible, on the ever-popular task of identifying hand-drawn digits. It may sound a bit academic, but these are the same techniques companies use to flag suspicious credit card activity, match you with movies, or decide who gets a loan.

### Contents
- **K-Nearest Neighbors** (KNN): The “ask your neighbors” approach to finding out what something is, this sometimes works better than expected.
- **K-Means**: Finding clusters in a mess of data points, which, depending on the data, can either be surprisingly neat or a total guessing game.
- **Naïve Bayes**: Statistically-minded, a little too trusting about independence, but fast and flexible, especially when you want a quick answer.
- **Hierarchical Clustering**: Like building a family tree for your data, though sometimes the “families” it finds are a little weird.

The pattern is pretty straightforward: First, try the method on two-dimensional points (think scatterplots), then see what happens with drawn numbers. Hierarchical clustering didn’t play nice with digits (long story), so it sticks to 2D.

### Milestones & Notebooks

Here’s the route, with one notebook per leg of the journey:

- K-Nearest Neighbors in 2D — `knn_2d.ipynb`
- K-Nearest Neighbors for Digits — `knn_digits.ipynb`
- K-Means in 2D — `k-means_2d.ipynb`
- K-Means for Digits — `k-means_digits.ipynb`
- Naïve Bayes in 2D — `naive_bayes_2d.ipynb`
- Naïve Bayes for Digits — `naive_bayes.ipynb`
- Hierarchical Clustering in 2D — `hierarchical_clustering_2d.ipynb`

### How You Might Use This

- Clone, open a notebook in Jupyter, and hit “Run.”
- Install requirements (mostly `scikit-learn`, `numpy`, `matplotlib`, and friends); nothing too wild.
- Step through the code blocks—experiment, get things wrong, and see what changes.
- If you mess around with the code and everything breaks, well, you’re in good (and somewhat realistic) company.

### Why Should You Care?

Maybe you just want to see how the basics of AI actually look in code, not in a highlight reel. Or you’re curious if these “classic” methods do anything interesting outside toy datasets. The truth is, these algorithms can be frustrating, surprising, and occasionally kind of elegant. Also, most real-world data isn’t as clean as what gets shown in tutorials.

One last note: Don’t expect perfection (from the models or from me), and don’t be afraid to question how much these classifiers “understand.” Sometimes they’re smarter than you’d think, and sometimes... they’re definitely not.

### Shoutouts

- Project based on the Manning liveProject: _Simple AI Algorithms for Classification_

#### License

This is mainly meant for learning and tinkering, not commercial use.


