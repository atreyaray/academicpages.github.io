---
layout: archive
title: "Projects"
permalink: /projects/
toc: true
---
{% include toc %}

This page is under construction... I will keep updating the projects page, in the meantime, do check out the github links.


## Finnish Housing Market Prediction

**Key Concepts** - *Exploratory Data Analysis, Data Visualisation, Clustering, Time Series Analysis, Facebook Prophet, SARIMAX*   
**Tools and Frameworks**- *Python, Numpy, Pandas, Sklearn, FB Prophet, Heroku, Git, Latex*

This project was a part of the course CS-C3250 Data Science Project 2021 under the supervision of  Prof. Jorma Laaksonen and Juha Vesanto, OP Financial Group's principal data scientist. The project's main objective was to gather related data from public sources and make a forecasting model of the development of house prices for the next four quarters.

We used data from the [Statistics Finland (Tilastokeskus)](https://tilastokeskus.fi/index_en.html) website. The dataset contained the prices of different house types for various postal codes throughout Finland. We performed exploratory data analysis by visualising missing data and conducting time series analysis on the data to discover trends and patterns in housing prices during the past 46 quarters. Next we preprocessed the data by adding features such as latitude and longitude, followed by trying out different imputation methods for missing data.

<img src="../images/projects/missing_geo.jpg" alt="graph" width="300"/>
<img src="../images/projects/prices_states.png" alt="graph" width="550"/>

For the prediction task we applied a couple of different time series methods. We used Prophet, an additive model utilising components such as trends, seasonality, holiday effect, and noise. Additionally we also made use of the Seasonal Autoregressive Integrated Moving Average eXogenous (SARIMAX) model using the `statsmodel` library. The final model which was deployed was an ensemble model pooling the results of both the SARIMAX and Prophet models. Based on the amount of missing data, we either used a model trained on individual postal code data, a grouped model from data of postal code clusters, or data from a postal code which was closest geographically.

<div>
<!-- <img class="center" src ="https://cdn.sstatic.net/Sites/stackoverflow/company/img/logos/so/so-icon.png?v=c78bd457575a"> -->
<img style="display:block; margin: 0 auto;" src="../images/projects/results.png" alt="results" width="700"/>
</div>

**Collaborators**: [Ken Riipa](https://www.linkedin.com/in/kenriippa/), [Bruce Nguyen](https://www.linkedin.com/in/quan-possible/), [Taeyoung Kee](https://www.linkedin.com/in/taeyoung-kee-960550113/), [Duong Tran](https://www.linkedin.com/in/duong-tran-552522176/), Son Nguyen

{% include buttons_dsp.html %}

<br/>


## IQ Growth Trends: Bayesian Analysis

**Key Concepts** - *Bayesian Analysis, Linear Regression, Monte Carlo Markov Chains, Convergence Diagnostics ( $\hat{R}$, $n_{\text{eff}}$ ), Performance Assessment (PSIS-LOO, $p_{\text{eff}}$ ), Prior Sensitivity Analysis, Data Preprocessing*   
**Tools and Frameworks**- *R, RMarkdown, Stan, Git*

This project was completed as a part of the course CS-E5710 Bayesian Data Analysis 2022. The main objectives of the report were to understand and apply the various steps in a Bayesian workflow. The project utilised the [Stan](https://mc-stan.org/) statistical programming language to perform Bayesian analysis on the IQ growth data. We used the [RMarkdown](https://rstudio.github.io/rmarkdown/) package to generate the report.

In this report we attempted to validate the [Flynn effect](https://en.wikipedia.org/wiki/Flynn_effect) with the help of [Full Scale IQ Change](https://github.com/owid/owid-datasets/tree/master/datasets/IQ%20Data%20-%20Pietschnig%20and%20Voracek%20(2015)) and [Schooling Index](https://frdelpino.es/investigacion/wp-content/uploads/2020/02/AHDI_1.1-1.xlsx) data. We explored the dependency between IQ change, time and change in average years of schooling in the population through Linear Regression. We investigated these dependencies both globally and per continent.

The trends in IQ were validated with a model that explored temporal dependency alone and a further model that factored in schooling level. We modeled the data with a pooled, separate and hierarchical model. These models explored the relationship between the passage of time and the development of IQ scores from the start of testing and the relationship between schooling level and the development of IQ scores from the start of testing.

<img src="../images/projects/linreg.png" alt="graph" width="450"/>
<img src="../images/projects/ppc.png" alt="graph" width="450"/>

**Collaborators**: [Aayush Kuckeria](https://www.linkedin.com/in/aayushkucheria/), and one other student from the course.


{% include buttons_bda.html %}
<br/>

## Predicting Helsinki's Humidity levels

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet. Duis sagittis ipsum. Praesent mauris. Fusce nec tellus sed augue semper porta. Mauris massa. Vestibulum lacinia arcu eget nulla. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. 

Curabitur sodales ligula in libero. Sed dignissim lacinia nunc. Curabitur tortor. Pellentesque nibh. Aenean quam. In scelerisque sem at dolor. Maecenas mattis. Sed convallis tristique sem. Proin ut ligula vel nunc egestas porttitor. Morbi lectus risus, iaculis vel, suscipit quis, luctus non, massa. Fusce ac turpis quis ligula lacinia aliquet. Mauris ipsum. Nulla metus metus, ullamcorper vel, tincidunt sed, euismod in, nibh. 

{% include buttons_ds.html %}
<br/>

## Cassino Game

Cassino, a fishing card game, played by drawing cards and matching them with those on the deck with similar value or symbols. Made with Scala, using graphics from ScalaFX and tested with ScalaTest.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet. Duis sagittis ipsum. Praesent mauris. Fusce nec tellus sed augue semper porta. Mauris massa. Vestibulum lacinia arcu eget nulla. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. 

Curabitur sodales ligula in libero. Sed dignissim lacinia nunc. Curabitur tortor. Pellentesque nibh. Aenean quam. In scelerisque sem at dolor. Maecenas mattis. Sed convallis tristique sem. Proin ut ligula vel nunc egestas porttitor. Morbi lectus risus, iaculis vel, suscipit quis, luctus non, massa. Fusce ac turpis quis ligula lacinia aliquet. Mauris ipsum. Nulla metus metus, ullamcorper vel, tincidunt sed, euismod in, nibh. 

<a class="github-button" href="https://github.com/atreyaray/CassinoGame" data-size="large" aria-label="Github Repo">Github Repo</a>

<script async defer src="https://buttons.github.io/buttons.js"></script>
