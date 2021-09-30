# NLP-project-Sentiment-Analysis-with-Sarcasm-Detection
NLP summer project, using Sarcasm Detection to improve Sentiment score prediction.
Including 4 parts:
1) training a bert model for sarcasm detection
- dataset: SemEval2018-Task3 (https://github.com/Cyvhee/SemEval2018-Task3)
- model: bert (transformers)
2) training a bert model for sentiment score prediction
- dataset: google-play-store-apps reviews data (https://www.kaggle.com/lava18/google-play-store-apps)
- model: bert (transformers)
3) Constructing a benchmark to measure how prediction model improve when using both sentiment polarity and sarcasm score as features
- dataset: web scraping data from apple app store, top 20 apps in September 1st, 2021 (17 apps collected in fact)
- model: random forest (sklearn)
4) Result
- contains the final sentiment score prediction for all reviews, the cos similarity between prediction in 5 grades and the real reviews star-grades from users. The initiative Baseline is by simple sampling from 1 to 5,  the comparitive baseline is constructed by sentiment features, the performance of project is constructed by sentiment features and sarcasm features. There is slight improvement overall but this approach gets different performances in different app types. In only 2 types of apps, performance is worse than only use sentiment features, others get improvement in difference.
