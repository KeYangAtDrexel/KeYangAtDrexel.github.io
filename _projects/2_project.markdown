---
layout: page
title: FairDBMS
description: Make DBMS fair
img: /assets/img/fairness.png
---


The term fairness refers to impartial and just treatment, lacking favoritism toward one side or another.
Arguments about fairness have a long tradition in the legal arena and in philosophical discourse. We interpret fairness in an algorithmic
decision-making process as impartial treatment of the individuals who are influenced by the algorithmic decisions. Partial treatment can
come from biased input data that is used to generate decisions, or from the algorithms that are driving the decision-making process.
It is usually difficult to ascertain the origin of partial treatment purely by observing algorithmic outcomes.
A typical example of partial treatment is Google Ads for Women. While Google showed ads for “$200K+” executive jobs to men 1,852 times, the same ads were only displayed 318 times to women.

<div class="img_row">
  <img class="col three" src="/assets/img/women_ads.png"/>
</div>

Two examples to illustrate possible causes of bias in the input data: under-representation and over-representation:

A crime dataset that only includes data from the New York boroughs of Manhattan and Brooklyn is insufficiently representative
to draw conclusions about the over-all crime rate in New York City. This is an example of geographic under-representation.

An example of over-representing a demographic group in input data is the cause of famous unintentional mistake of Google's photo app.
Google's photo app classified images of black people as gorillas when it applies automatic labels to pictures in digital photo albums.
If the training dataset in the photo recognition apps is over-representing white people (i.e., under-representing black people), it shows
bad performance when recognizing non-white people [whiteGuyProblem](http://www.nytimes.com/2016/06/26/opinion/sunday/artificial-intelligences-white-guy-problem.html), such as labeling black people as gorillas.

<div class="img_row">
    <img class="col two" src="/assets/img/google_photos.png" title="Google Photos"/>
    <img class="col one" src="/assets/img/label_black.png" title="Labeled people as Gorillas"/>
</div>

Through the steps of a DBMS, lack of fairness can be mitigated through modifying the data itself, modifying the algorithms or modifying
the outcomes of the decision-making process.

We currently focus on encoding fairness in the ranked outcomes of decision-making processes. Comparing to literature on fairness in the output of a data
mining or a machine learning task, we interpret fairness in the context of rankings besides inside a selection and classification problem.

A short paper "Measuring Fairness in Ranked outputs" [(PDF)](https://arxiv.org/pdf/1610.08559) captures our initial steps on interpreting fairness in rankings.

