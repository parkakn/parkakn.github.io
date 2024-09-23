---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

<span style="font-size: 1.4em; font-weight: bold;">Citation Network of Finance Journal Articles</span> <em>(2024)</em> 
<a href="https://github.com/parkakn/Citation-Network-Finance-Journals">[Github]</a>
<br>
We built a paper-to-paper citation network of journal articles published in the Journal of Financial Economics (JFE) and their citing papers on Google Scholars through a web scrapping program. Our dataset covers 2,373 JFE papers published from January 2005 to February 2004 and 184,568 citing papers from Google Scholars. It contains 410,772 directed edges and node attributes, such as paper authors, publication dates, and sources of publication for citing papers. We further provide information on authors by identifying the university/institute of association and its location. 
<div style="display: flex; justify-content: center;">
  <img width="70%" src="/images/citation network zoom 1.png" alt="obj">
</div>
------

<span style="font-size: 1.4em; font-weight: bold;">Analysis of Miners in the Bitcoin Blockchain Network</span> <em>(2023)</em> 
<a href="https://mitsloan.mit.edu/shared/ods/documents?PublicationDocumentID=7981">[Referenced Paper]</a>
<br>
As the probability of mining a block and obtaining a reward in the Bitcoin blockchain is proportional to the hashing power spent on mining, miners are incentivized to pool their computing power. Consequently, mining in the Bitcoin blockchain is dominated by mining pools. 

High concentration of mining pool capacity poses a risk to Bitcoin, such as the danger of a 51% attack. However, information individual miners are not commonly available, unlike that of minings pools. Thus, we track the distribution of mining rewards from some of the largest mining pools to the miners to identify individual miners and understand the concentration of the Bitcoin mining capactiy. 
<div style="display: flex; justify-content: center;">
  <img width="100%" src="/images/Antpool_dist_graph-1.png" alt="obj">
</div>
------

<span style="font-size: 1.4em; font-weight: bold;">Robo-Advisor for Individual Retirement Pension (IRP) Funds</span> <em>(2024)</em> 
<a href="https://github.com/kangokseo/cqralgo?tab=readme-ov-file">[Github]</a>
<br>
In 2023, the Financial Services Commission of South Korea annoucned the implementation of providing robo-advisory services for retirement pension funds. Robo-advisors that are approved from the [Robo Advisor Test Bed Center](https://www.ratestbed.kr:7443/portal/main/main.do) earn the rights to provide services for Individual Retirement Pension (IRP) accounts beginning in the summer of 2024.<sup>[1](https://www.digitaltoday.co.kr/news/articleView.html?idxno=513226)</sup> 

We built a prototype of our robo-advisor and are currently in the development stages. Our algorithm is based on market cycles and seasonality and invests in stock market indices of the United States and South Korea. The goal of our robo-advisor is to provide the optimal portfolio suitable based on investor risk preferences while beating the returns of the S&P500 index as our benchmark.
<div style="display: flex; justify-content: center;">
  <img width="70%" src="/images/backtest.png" alt="obj">
</div>
------

<span style="font-size: 1.4em; font-weight: bold;">Principal Component Analysis and Hidden Markov Model for Forecasting Stock Returns</span> <em>(2023)</em> 
<a href="https://arxiv.org/abs/2307.00459">[Paper]</a>
<br>
This paper presents a method for predicting stock returns using principal component analysis (PCA) and the hidden Markov model (HMM) and tests the results of trading stocks based on this approach. Principal component analysis is applied to the covariance matrix of stock returns for companies listed in the S&P 500 index, and interpreting principal components as factor returns, we apply the HMM model on them. Then we use the transition probability matrix and state conditional means to forecast the factors returns. Reverting the factor returns forecasts to stock returns using eigenvectors, we obtain forecasts for the stock returns. We find that, with the right hyperparameters, our model yields a strategy that outperforms the buy-and-hold strategy in terms of the annualized Sharpe ratio.
<div style="display: flex; justify-content: center;">
  <img width="70%" src="/images/hmm.png" alt="obj">
</div>
------

<span style="font-size: 1.4em; font-weight: bold;">Analyzing Entity Portrayals in Narrative Text: PCA vs UMAP for Affect Subspace Projection </span> <em>(2022)</em> 
<br>
To analyze the portrayals of people in narrative text, pre-trained contextualized word embeddings have been used to extract affect information about target entities. Words have three key affective dimensions: valence representing sentiment, arousal representing agency, and dominance representing power. We use the Affect Subspace Projection (ASP) model to find a one-dimensional representation for each affect dimension and to predict affect scores of each entity by mapping its embedding onto each of dimensions. Specifically, we test ASP with two different dimension reduction techniques - Principal Component Analysis (PCA) and Uniform Manifold Approximation and Projection (UMAP).

[Pipeline](/images/dimensionality_reduction.pdf)

<div style="display: flex; justify-content: center;">
  <img width="35%" src="/images/word affect scores.jpeg" alt="obj">
  <img width="33%" src="/images/results_ASP.png" alt="obj">
</div>
------



