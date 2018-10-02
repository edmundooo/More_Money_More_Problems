# More_Money_More_Problems (DRAFT)
---

I authored the Python script and IPython Notebooks in this repo to collect all the Tweets by the [current members of the United States Congress](https://gwu-libraries.github.io/sfm-ui/posts/2017-05-23-congress-seed-list), clean the data, preprocess the text of all Tweets using Natural Languge Toolkit, and model their topics using [gensim's Latent Dirichlet allocation](https://radimrehurek.com/gensim/models/ldamodel.html). I then introduced [Campaign Finance information](https://www.opensecrets.org/api/admin/?function=user_api_use) for each member of Congress and analyzed how the amount PAC money they receive to finance their campaigns affects what they Tweet about.

---

<img width="1007" alt="screen shot 2018-10-01 at 3 43 05 pm" src="https://user-images.githubusercontent.com/25728710/46312190-59f62200-c592-11e8-9aaf-c65d65c72646.png">

---
### This repository includes:



* __01_Get_Congress_Tweets.py:__ gets the Tweets of all the current members of the US Congress, and reads the Tweets and select Tweet metadata into CSV files

* __02_Partial_Data_EDA.ipynb:__ reads in Senator Amy Klobuchar's Tweets performs EDA on on the them

* __03_Tweets_to_Pickle.ipynb:__ reads all Tweets from CSV files and then Pickles the data

* __04_Full_Data_Clean_Preprocess.ipynb:__ reads all Tweets from Pickle, performs EDA, cleans them, and preprocceses them in preparation for topic modeling

* __05_Topic_Modeling.ipynb:__ reads preprocessed Tweets from Pickle, converts preprocessed Tweets to a matrix of token counts, and performs Latent Dirichlet Allocation to derive topics from and assign topics to the Tweets

* __06_Congress_Metadata.ipynb:__ - downloads metadata for each Congress member, and resolves discrepancies between the Twitter usernames listed in the Congress metadata and Tweet data

* __06_Campaign_Finance_Data.ipynb:__ downloads campaign finance information for each relevant member of Congress
