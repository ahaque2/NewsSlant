# NewSlant: Identifying Political Slant in News and Understanding Influence on Readers

Abstract—It is widely believed that political news is often slanted to suit news publishers’ ideology. Politically slanted news can influence its readers to focus on different aspects of contentious social and political issues and hinder effective discussions. To identify political slants in news and its influence on readers, we analyze Election-related news and analyze user response to the news on Twitter. We collect Election-related news from six mainstream US news publishers covering the 2020 US Presidential Elections. We compute news publishers’ political slants based on the favorability of news toward the two major parties’ Presidential candidates. We use a Target- dependent Sentiment Classification (TSC) approach to determine the favorability of news toward the two candidates. We find that the Election-related news coverage shows signs of political slant in both, news headlines and on Twitter. The difference in news coverage of the two Presidential candidates between the left-leaning news publishers (LEFT) and right-leaning news publishers (RIGHT) is statistically significant. The effect size is larger for the news on Twitter than for headlines. Further, news on Twitter is more sentimental than news headlines. We further identify moral foundations in user responses to news on Twitter based on Moral Foundation Theory (MFT). We fine-tune a transformer- based deep learning model to identify moral foundations in user responses. Moral foundations in user responses to LEFT and RIGHT differ significantly. Further, the shift in moral foundation in user responses to LEFT and RIGHT differ across social and political issues. User engagement is highest in user responses to the RIGHT, and lowest in user responses to BALANCED news.


### Reproducing the results

Download the data from the link in the Readme under the dataset/ and place under the dataset/ folder.
The dataset files already contain the sentiment towards the two Presidential candidate in news headlines and Tweets, as well as moral foundation scores for user response. The results can be directly produced from these. If you wish to produce these scores, the repository includes code for that as well

Sentiment Analysis
- 1a_target_sentiment_analysis.ipynb contains code to compute the target based sentiment for news headlines and Tweets.
- 6a_statistical_analysis.ipynb contains code to compares sentiment distributions between left and right.

Topic Modeling
- 4a_topic_modeling_news.ipynb contains code for topic modeling of the news headlines. 
- 4a_topic_modeling_news_tweets.ipynb contains code for topic modeling of the news Tweets.
- 5a_topic_analysis.ipynb contains code to analyze the topics identified and comapore between left and right

User Response Analysis
- 2a_Training_MFT_model.ipynb conatins code to train the moral foundation model using the MFTC dataset.
- 2b_MFT_UR_prediction.ipynb conatins code to use the trained model to predict moral foundation scores os user responses.
- 2c_MFT_user_resp_analysis.ipynb contains code to analyse the moral foundation scores in user responses.
- 3a_statistical_tests_MFT.ipynb contains code to conduct statistical tests for moral foundation scores (comparing moral foundations across user responses to Left and Right).
- 3*_user_response_emotion_analysis.ipynb contains additional analysis based on the emotions in user response.
