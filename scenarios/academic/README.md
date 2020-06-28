# Recommender Systems for Academics 

Recommender systems have become a key growth and revenue driver for modern retail.  For example, recommendation was estimated to [account for 35% of customer purchases on Amazon](https://www.mckinsey.com/industries/retail/our-insights/how-retailers-can-keep-up-with-consumers#). In addition, recommenders have been applied by retailers to delight and retain customers and improve staff productivity. 

Recommendation system has been widely applied in the commmericial fields like retail, entertainment, etc. It's been recognizied that recommendation technology can also help researchers find relevant articles to help conduct research activities. There are tremendous efforts in this field. For example, [Microsoft Academic Graph has developed a hybrid scalable recommendation system that provides recommendations for approximately 160 million English research papers and patents](https://arxiv.org/abs/1905.08880).

## Scenarios

Academic recommendaiton may work for a variety of different problems, e.g., 

* searching the literature in any topic a researcher is interested in 
* finding recent or traditional papers related to a research problem
* improving the reference list of a manuscript being written
* finding a set of researchers in a field of interest to follow their work
* finding a list of potential reviwers

### Literature recommendation

This is usually seen in the academic recommendation problems. There are usually two types of recommendation techniques used for this problem, which are *citation-based recommendation* and *content-based recommendation*. 

#### Citation-based recommendation

Citation-based recommendation refers to the recommendation problem where the recommended literature generated for users is based on its citation network. 

### Citation-based recommendation

### Content-based recommendation

### Personalized recommendation

A major task in applying recommenations in retail is to predict which products or set of products a user is most likely to engage with or purchase, based on the shopping or viewing history of that user. This scenario is commonly shown on the personalized home page, feed or newsletter.  Most models in this repo such as [ALS](../../examples/00_quick_start/als_movielens.ipynb), [BPR](../../examples/02_model_collaborative_filtering/cornac_bpr_deep_dive.ipynb), [LightGBM](../../examples/00_quick_start/lightgbm_tinycriteo.ipynb) and [NCF](../../examples/00_quick_start/ncf_movielens.ipynb) can be used for personalization. [Azure Personalizer](https://docs.microsoft.com/en-us/azure/cognitive-services/personalizer/concept-active-learning) also provides a cloud-based personalization service using reinforcement learning based on [Vowpal Wabbit](../../examples/02_model_content_based_filtering/vowpal_wabbit_deep_dive.ipynb).

### You might also like

In this scenario, the user is already viewing a product page, and the task is to make recommendations that are relevant to it.  Personalized recommendation techniques are still applicable here, but relevance to the product being viewed is of special importance.  As such, item similarity can be useful here, especially for cold items and cold users that do not have much interaction data.

### Frequently bought together

In this task, the retailer tries to predict product(s) complementary to or bought together with a  product that a user already put in to shopping cart. This feature is great for cross-selling and is normally displayed just before checkout.  In many cases, a machine learning solution is not required for this task.

### Similar alternatives

This scenario covers down-selling or out of stock alternatives to avoid losing a sale. Similar alternatives predict other products with similar features, like price, type, brand or visual appearance.

## Data and evaluation

Datasets used in retail recommendations usually include  [user information](../../GLOSSARY.md), [item information](../../GLOSSARY.md) and [interaction data](../../GLOSSARY.md), among others.

To measure the performance of the recommender, it is common to use [ranking metrics](../../GLOSSARY.md). In production, the business metrics used are [CTR](../../GLOSSARY.md) and [revenue per order](../../GLOSSARY.md). To evaluate a model's performance in production in an online manner, [A/B testing](../../GLOSSARY.md) is often applied.

## Other considerations

Retailers use recommendation to achieve a broad range of business objectives, such as attracting new customers through promotions, or clearing products that are at the end of their season. These objectives are often achieved by re-ranking the outputs from recommenders in scenarios above. 




