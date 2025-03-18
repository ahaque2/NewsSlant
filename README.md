# NewSlant: Identifying Political Slant in News and Understanding Influence on Readers

Abstract—Political news is often slanted toward its publisher's ideology and seeks to influence readers by focusing on selected aspects of contentious social and political issues. We investigate political slants in news and their influence on readers by analyzing election-related news and reader reactions to the news on Twitter. To this end, we collected election-related news from six major US news publishers who covered the 2020 US presidential elections. We computed each publisher's political slant based on the favorability of its news toward the two major parties' presidential candidates. We found that the election-related news coverage shows signs of political slant both in news headlines and on Twitter. The difference in news coverage of the two candidates between the left-leaning (LEFT) and right-leaning (RIGHT) news publishers is statistically significant. The effect size is larger for the news on Twitter than for headlines. And, news on Twitter expresses stronger sentiments than the headlines. We identified moral foundations in reader reactions to the news on Twitter based on Moral Foundation Theory. Moral foundations in readers' reactions to LEFT and RIGHT differ statistically significantly, though the effects are small. Further, these shifts in moral foundations differ across social and political issues. User engagement on Twitter is higher for RIGHT than for LEFT. We posit that an improved understanding of slant and influence can enable better ways to combat online political polarization.

## Reproducing the results

Download the dataset and unzip under the '_dataset/_' folder.
You can download the dataset from [IEEE-DataPort](https://ieee-dataport.org/documents/newsslant). 
For more details about the dataset read the README file under the '_dataset/_' folder.
The dataset files already contain the sentiment towards the two Presidential candidate in news headlines and Tweets, as well as moral foundation scores for user response. The results can be directly produced from these. If you wish to produce these scores, the repository includes code to reproduce these scores as well.

#### Sentiment Analysis
- 1a_target_sentiment_analysis.ipynb contains code to compute the target based sentiment for news headlines and Tweets.
- 6a_statistical_analysis.ipynb contains code to compares sentiment distributions between left and right.

#### Topic Modeling
- 4a_topic_modeling_news.ipynb contains code for topic modeling of the news headlines. 
- 4a_topic_modeling_news_tweets.ipynb contains code for topic modeling of the news Tweets.
- 5a_topic_analysis.ipynb contains code to analyze the topics identified and comapore between left and right

#### User Response Analysis
- 2a_Training_MFT_model.ipynb conatins code to train the moral foundation model using the MFTC dataset.
- 2b_MFT_UR_prediction.ipynb conatins code to use the trained model to predict moral foundation scores os user responses.
- 2c_MFT_user_resp_analysis.ipynb contains code to analyse the moral foundation scores in user responses.
- 3a_statistical_tests_MFT.ipynb contains code to conduct statistical tests for moral foundation scores (comparing moral foundations across user responses to Left and Right).
- 3*_user_response_emotion_analysis.ipynb contains additional analysis based on the emotions in user response.

If you use any of the code or data from this repo, kindly cite our paper. 

- **A. Haque and M. P. Singh**, *"NewsSlant: Analyzing Political News and Its Influence Through a Moral Lens,"* in IEEE Transactions on Computational Social Systems, vol. 11, no. 3, pp. 3329-3337, June 2024, [![DOI:10.1109/TCSS.2023.3341910](https://doi.org/10.1007/978-3-031-21438-7_60)]
