# Scientific Paper Clustering

## Table of Contents
- [Abstract](#link-part-1)
- [Design](#link-part-2)
- [Data](#link-part-3)
- [Algorithm](#link-part-4)
- [Tools](#link-part-5)
- [Communication](#link-part-6)
- [**How to run**](#link-part-7)
- [Reference](#link-part-8)

## <a name="link-part-1">Abstract</a>

There are a lot of scientific papers online with different topics.
Clustering papers that shares similar topics can provide researchers
paper recommendations to help them recommend papers that they would be
interested in and also to group the papers into categories so they
can be looked up more easily.

## <a name="link-part-2">Design</a>

This project originates from the arXiv dataset. Clustering scientific
papers would enable scientific paper recommendation function to help
researchers find papers that are similar to their research interests,
or papers that are not in their research interests but they might be
interested in. Looking for and reading papers can cost lots of time and
this recommendation system can definately save time for researchers.

## <a name="link-part-3">Data</a>

The data comes from [arXiv Dataset](https://www.kaggle.com/datasets/Cornell-University/arxiv).

It contains data for 2,142,715 scientific papers including authors,
title, doi, categories, abstract, etc. I have filtered the dataset
into a smaller one that only contains 379,985 papers that the last
version was published after 2020, and then sampled 50,000 rows from
the filtered dataset for clustering.

## <a name="link-part-4">Algorithm</a>

**Data Cleaning:**



**Topic Modeling:**


**Models:**

- **K-means model**:

- - Selecting number of clusters:

<img src="/imgs/selecting_clusters.png" style="width: 400px;" />

- - Final number of clusters: 14

- - Final clusters:

<img src="/imgs/KMeans.png" style="width: 400px;" />


**Model Evaluation and Selection:**


**Final scores:**



## <a name="link-part-5">Tools</a>

* **Pandas** for exploratory data analysis.
* **Matplotlib** and **Seaborn** for plotting.
* **Scikit Learn** for modeling and natural language process.
* **Pickle** for saving models in a pickle file.

## <a name="link-part-6">Communication</a>

The project proposal is shown [here](/documents/proposal.md).

The MVP document is shown [here](/documents/MVP.md).

## <a name="link-part-7">How to run</a>

cd into [/recommender](/recommender):
```
cd recommender
```

Run the recommender by:
```
python3 recommender.py $(paper_index)
```

For example:
```
python3 recommender.py 3
```

## <a name="link-part-8">Reference</a>
- [1]: [Cornell University, Joe T., Devrishi, & Brian M. ArXiv Dataset](https://www.kaggle.com/datasets/Cornell-University/arxiv)
