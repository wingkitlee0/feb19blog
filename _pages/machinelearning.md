---
layout: single
title: "Machine Learning"
permalink: /machinelearning/
author_profile: true
toc: true
---

## [Abstract Analyzer](https://azj31tvvek.execute-api.us-east-1.amazonaws.com/dev/)

![A demo GIF was here..](../assets/images/demo.gif)

When a paper is being submitted to the [arxiv](www.arxiv.org) preprint server, the author needs to manually select which category the paper belong to. This [webapp](https://azj31tvvek.execute-api.us-east-1.amazonaws.com/dev/) allow user to enter their abstract (i.e., a few lines of the summary of their important paper), then the code will analyze it and suggest a category it belongs (in astronomy). The classification task is done by a small neural network (trained by submitted abstracts).

Check the title for the webapp. 

The code can be found [here](https://github.com/wingkitlee0/arxiv_explore) <i class="fab fa-fw fa-github"></i>.

For the deployment detail (e.g., ow to deploy the webapp (with numpy and tensorflow) onto [AWS Lambda](https://aws.amazon.com/lambda/) <i class="fab fa-aws"></i>), I have written a [blog post](../_posts/2019-02-02-deploying-tensorflow-on-amazon-lambda.md) about it.

## Demo of webapp (20 news group  dataset)

[webapp](https://sm2op9jgr0.execute-api.us-east-1.amazonaws.com/dev/)

(It may take a few seconds to load.)

Before fully implementing the above project, I tried to make a working demo. This demo takes two numbers (features) from users, and predict which type of Iris it should belong. While it is a textbook machine learning, I have made an web app.

Features:
- Data (model parameters) are hosted on *Amazon S3*
- Webapp is running on AWS Lambda <i class="fab fa-aws"></i> using *flask* and scikit-learn.

The codes and reference are hosted on [GitHub](https://github.com/wingkitlee0/flask-webapps/tree/master/newsgroup) <i class="fab fa-fw fa-github"></i>.
