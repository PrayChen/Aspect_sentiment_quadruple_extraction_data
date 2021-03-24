# Aspect sentiment quadruple extraction dataset
## Task Description
Aspect sentiment quadruple extration (ASQE) is the task of extracting the quadruples of aspect, opinion, category, polarity. 

For example:  

Given a sentiment:  

**Waiters are very friendly and the pasta is simply average.**  

The objective of ASQE task is to predict the quadruples: 

**[(Waiters, friendly, service, Positive), (pasta,  average, food, Neutral)]**  

where a triplet consists of (aspect, opinion, category, polarity)  

## Data Description

The data is Zhijiang Sentiment Analysis Task Preliminary Chinese DataSet

There two csv files. **reviews.csv**  contains **id** and **reviews**, and its label corresponds to the row data with same **id** in **labels.csv**

The data of **labels.csv** have the following format:  

> id, AspectTerms, Aspect_start_index, Aspect_end_index, OpinionTerms, Opinon_start_index, Opinion_end_index, Category, Polarities.

For example:

> 1, _, , , 很好，0, 2, 整体，正面

**'_'** denotes the aspect term or opinion term is None, it do not appear in the reviews. Then the position of Aspect_start_index and Aspect_end_index are empty.

There are three types of **Polarity**,  {Positive, Negtive, Neutral}

There are 13 types of **Category**,  {整体，使用体验， 功效，价格， 物流， 气味， 包装， 真伪， 服务， 其他， 成分， 尺寸， 新鲜度}




