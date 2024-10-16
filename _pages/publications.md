---
layout: archive
title: 
permalink: /projects/
author_profile: true
---
<span style="font-size: 1.5em; font-weight: bold;">Predicting Job Transitions with Graph Machine Learning</span> <em>(2024)</em> 
<br>

U.S. manufacturers face significant challenges in filling job openings, particularly those requiring skilled technical workers. The situation becomes even more difficult for roles involving advanced technologies. Given that traditional education and training programs lag behind technological advancements, we aim to address this gap by identifying potential candidates from the existing workforce.

Using resume data from 132 million U.S. workers, we mine job transitions and model them as a one-step Markov chain. This model is represented as a random walk on a directed, weighted graph, where jobs are nodes and transitions are edges. The resulting job transition network includes 1,013 nodes and 571,172 edges. Based on this network, we identify potential sources of workers for target manufacturing roles and for a set of emerging manufacturing jobs not present in the original network.

Furthermore, we predict job transitions using graph machine learning models. By incorporating node and edge features—such as wages, employment, and skills for each job—along with network-based features like centrality measures, we enrich our network. We then apply encoding models, such as node2vec and graph neural network models, to test the predictive power of our model and these features.

------
<span style="font-size: 1.5em; font-weight: bold;">PyTutor with Personal Robots Group of MIT Media Lab</span> <em>(2024)</em> <a href="https://www.media.mit.edu/projects/pytutor-empowering-equitable-education-pathways-in-computing-with-generative-ai/overview/">[PyTutor]</a>

<span style="font-size: 1.1em;font-weight: bold;">Improving Contextual Knowledge for AI Tutor: Advanced RAG with Multi-modal LLM</span>  
With the Personal Robots Group at the Media Lab, we are developing an educational AI tutor driven by an LLM. To give the AI tutor access to domain-specific knowledge, which in our case are course materials for an introductory programming course at MIT and GSU, we implement RAG. Given the nature of LLMs in generating response from prompts with context, a significant part of our RAG framework is the data ingestion pipeline. The course materials are complex PDF documents with various embedded objects, such as tables, flowcharts, and figures, and naively parsing these documents will lead to thrash-in, thrash-out. To avoid this situation, we use a multi-modal LLM to parse our documents to markdown format, which LLMs are able to understand more easily than the text formats humans are used to, and chunk these documents into texts and objects based on the structure of the markdown file. These chunks are then stored in our database for the AI tutor to access and retrieve domain-specific knowledge from. 

<div style="display: flex; justify-content: center;">
  <img width="80%" src="/images/pytutor_2.png" alt="obj">
</div>

<span style="font-size: 1.1em;font-weight: bold; ">Personalized Learning with Prompt Engineering</span> 
<br>
Another feature we aim to implement in our AI tutor is personalization. Students in a course are most likely to have different learning needs. For example, one student may have a strong understanding of multiplication and lack undestanding of division, while another may be the opposite. Hence, we achieve efficient learning by assessing each student's progress through the entire course and in each course event (defined as a particular event in a course, such as reviewing a lecture or completing an assignemnt) and  providing tailored learning pathways. Our current method is to prompt an LLM with abundunt context, including summaries of the course and the target course event, past chat history between the student and AI tutor, and the history of assessments of the student progress. Although context windows are increasing for LLMs, we aim to improve this personalization feature by constructing a knowledge graph of the course materials and embedding deepr understanding of the course, such as relationships between the course events. 

------

<span style="font-size: 1.5em; font-weight: bold;">Citation Network of Finance Journal Articles</span> <em>(2024)</em> 
<a href="https://github.com/parkakn/Citation-Network-Finance-Journals">[Github]</a>
<br>

We construct a citation graph of finance journal articles and their citing papers. Through web crawling and web scraping, we collect publication data, including titles, authors, and dates, for all papers published in the *Journal of Financial Economics* (JFE) from January 2005 to February 2024, along with their corresponding citing papers listed on Google Scholar. In this graph, a directed edge exists from paper i to paper j if i cites j. The resulting citation network consists of 186,941 papers (2,373 JFE papers and 184,568 citing papers) and 410,772 directed edges.

We also collect profile data for each author, including their affiliated university and location, sourced from the websites of various finance associations. This enriches our dataset, allowing for the construction of a heterogeneous graph where nodes represent both papers and authors, and edges capture the associations between authors and their papers, as well as paper-to-paper citations. 

------

<span style="font-size: 1.5em; font-weight: bold;">Analysis of Miners in the Bitcoin Blockchain Network</span> <em>(2023)</em> 
<a href="https://mitsloan.mit.edu/shared/ods/documents?PublicationDocumentID=7981">[Referenced Paper]</a>
<br>

As the probability of mining a block and obtaining a reward in the Bitcoin blockchain is proportional to the hashing power spent on mining, miners are incentivized to pool their computing power. Consequently, mining in the Bitcoin blockchain is dominated by mining pools. 

High concentration of mining pool capacity poses a risk to Bitcoin, such as the danger of a 51% attack. However, information individual miners are not commonly available, unlike that of minings pools. Thus, we track the distribution of mining rewards from some of the largest mining pools to the miners to identify individual miners and understand the concentration of the Bitcoin mining capactiy. 
<div style="display: flex; justify-content: center;">
  <img width="100%" src="/images/Antpool_dist_graph-1.png" alt="obj">
</div>
------

<span style="font-size: 1.5em; font-weight: bold;">Robo-Advisor for Individual Retirement Pension (IRP) Funds</span> <em>(2024)</em> 
<a href="https://github.com/kangokseo/cqralgo?tab=readme-ov-file">[Github]</a>
<br>

In 2023, the Financial Services Commission of South Korea annoucned the implementation of providing robo-advisory services for retirement pension funds. Robo-advisors that are approved from the [Robo Advisor Test Bed Center](https://www.ratestbed.kr:7443/portal/main/main.do) earn the rights to provide services for Individual Retirement Pension (IRP) accounts beginning in the summer of 2024.<sup>[1](https://www.digitaltoday.co.kr/news/articleView.html?idxno=513226)</sup> 

We built a prototype of our robo-advisor and are currently in the development stages. Our algorithm is based on market cycles and seasonality and invests in stock market indices of the United States and South Korea. The goal of our robo-advisor is to provide the optimal portfolio suitable based on investor risk preferences while beating the returns of the S&P500 index as our benchmark.
<div style="display: flex; justify-content: center;">
  <img width="70%" src="/images/backtest.png" alt="obj">
</div>
------

<span style="font-size: 1.5em; font-weight: bold;">Principal Component Analysis and Hidden Markov Model for Forecasting Stock Returns</span> <em>(2023)</em> 
<a href="https://arxiv.org/abs/2307.00459">[Paper]</a>
<br>

This paper presents a method for predicting stock returns using principal component analysis (PCA) and the hidden Markov model (HMM) and tests the results of trading stocks based on this approach. Principal component analysis is applied to the covariance matrix of stock returns for companies listed in the S&P 500 index, and interpreting principal components as factor returns, we apply the HMM model on them. Then we use the transition probability matrix and state conditional means to forecast the factors returns. Reverting the factor returns forecasts to stock returns using eigenvectors, we obtain forecasts for the stock returns. We find that, with the right hyperparameters, our model yields a strategy that outperforms the buy-and-hold strategy in terms of the annualized Sharpe ratio.
<div style="display: flex; justify-content: center;">
  <img width="70%" src="/images/hmm.png" alt="obj">
</div>
------

<span style="font-size: 1.5em; font-weight: bold;">Analyzing Entity Portrayals in Narrative Text</span> <em>(2022)</em> 
[[Pipeline]](/images/dimensionality_reduction.pdf) 
<br>

Bidirectional Encoder Representations from Transformers (BERT) has shown the ability to understand the context of a word in a sentence, making it one of the most popular models in NLP. Our aim is to use this pre-trained language model in combination with dimension reduction techniques to understand how entities are portrayed in narrative text based on three primary affect dimensions: potency, valence, and activity. For example, given a target entity, such as Batman, mentioned in a movie plot, our goal is to capture its scores for each affect dimension. 

To extract an affect dimension, we select pairs of semantically similar, but polar opposite words (corresponding to each affect) from the VAD Lexicon and construct a matrix of word embeddings. Then, we apply a dimension reduction technique to extract the subspace corresponding to the affect dimension. From movie plot summaries, we extract contextual word embeddings for a target entity and project it to the affect dimensions. We compare PCA and UMAP for extracting the affect subspace and find that PCA leads to more significant accuracy for all affect dimensions.

<div style="display: flex; justify-content: center;">
  <img width="35%" src="/images/word affect scores.jpeg" alt="obj">
  <img width="33%" src="/images/results_ASP.png" alt="obj">
</div>
------



