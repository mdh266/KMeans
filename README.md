# Writing A Scikit Learn Compatible Clustering Algorithm
-----------------------

## About
---------
In this post, I will go over how to write a K-means clustering algorithm from scratch using [NumPy](https://numpy.org/). The algorithm will be explained in the next section and while seamingly simple, it can be tricky to implement efficiently! As an added bonus, I will go over how to implement a [Scikit-Learn](https://scikit-learn.org/stable/) compatible clustering algorithm so that we can using Scikit-Learn's framework including [Pipelines](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html) and [GridSearchCV](https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.GridSearchCV.html).


## Using The Notebook
----------
You can install the dependencies and access the notebook using <a href="https://www.docker.com/">Docker</a> by building the Docker image with the following:

	docker build -t kmeans .

Followed by running the command container:

	docker run -ip 8888:8888 -v `pwd`:/home/jovyan -t kmeans

See <a href="https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html">here</a> for more info. 

Otherwise without Docker, make sure to use Python 3.9 and install the libraries listed in <code>requirements.txt</code>.  These can be installed with the command,

	pip install -r requirements.txt
