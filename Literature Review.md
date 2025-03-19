####
Literature Review
1.	Facebook vs Twitter – what makes they different
2.	Data integration techniques
3.	Review of personality prediction from Facebook data
4.	Review of personality prediction from Twitter data
5.	Conclusion


Serrano-Guerrero et al. (2024) developed a novel approach to predicting personality traits using a stacked ensemble model that integrates multiple machine learning and deep learning algorithms that leveraged text data from 250 Facebook users. However, there was a notable difference in the performance of the model particularly with the Openness trait compared to other personality traits. This is likely due to the fact the model has the highest number of instances in the dataset for the Openness trait while other traits such as Agreeableness and Conscientiousness have fewer instances. (data imbalance)

Utami, Oyong, Raharjo, Dwi Hartanto, & Adi (2021) explored the use of machine learning and natural language processing (NLP) techniques to classify personality traits based on Twitter posts in Bahasa Indonesia using the DISC personality model. The initial data distribution revealed by SVC (support vector classifier) performed poorly due to data imbalance. However, significant improvement was seen in the model performance when the SMOTETomek resampling technique was used to address the data imbalance.


Sirasapalli & Malla (2023) proposed a novel methodology for improving personality prediction models on social media text data by combining two benchmark datasets: the MBTI dataset (from Twitter) and the Big Five dataset (from essays) using the dataset mapping algorithm. The proposed model outperforms existing models, with the highest accuracy for Openness and Extraversion. However, we do not know how the model will perform on other social media platforms such as Facebook regarding its generalizability. 

Ryan, Katarina, & Suhartono, (2023) explored the use of machine learning and natural language processing (NLP) techniques to predict Myers-Briggs Type Indicator (MBTI) personality types based on textual data using Word2Vec for word embedding and various machine learning models. Six models were tested: Logistic Regression (LR), Linear Support Vector Classification (LSVC), Stochastic Gradient Descent (SGD), Random Forest (RF), Extreme Gradient Boosting (XGBoost), and CatBoost. However, due to class imbalance, the SMOTE technique was used to increase the number of data points by generating new samples from existing ones, thus, an improvement was recorded in each model’s performance.

A study by Maharani & Effendy (2022) employed machine learning techniques such as Naive Bayes (NB), K-Nearest Neighbors (KNN), and Support Vector Machine (SVM) to predict personality traits with a focus on the Big Five Model from a dataset of 160,000 tweets collected from 800 Indonesian Twitter users. The study revealed that SVM excels better than NB and KNN in predicting personality traits even though it achieved a below-average performance with an accuracy of 59.45% compared to other prediction models developed for the same purpose. However, I believe that the model's performance would have improved significantly if techniques such as SMOTE or data integration were used to increase the size of the dataset.

Focusing on Twitter, Karanatsiou et al. (2022) presented a novel approach using a holistic profiling model to predict personality traits and relational traits of social media users by leveraging machine learning techniques.  The data employed for this study was collected from 243 Twitter users via Amazon Mechanical Turk, gathering 350,000 tweets and self-reported psychological profiles. The developed model exploiting correlations between personality traits and attachment orientations outperformed state-of-the-art approaches by improving prediction accuracy of 29 percent,








1.	Serrano-Guerrero, J., Alshouha, B., Bani-Doumi, M., Chiclana, F., Romero, F. P., & Olivas, J. A. (2024). Combining machine learning algorithms for personality trait prediction. Egyptian Informatics Journal, 25, 100439. doi:10.1016/j.eij.2024.100439 
2.	Utami, E., Oyong, I., Raharjo, S., Dwi Hartanto, A., & Adi, S. (2021). Supervised learning and resampling techniques on disc personality classification using Twitter information in Bahasa Indonesia. Applied Computing and Informatics, 21(1/2), 141–151. doi:10.1108/aci-03-2021-0054 
3.	Machine learning approach to improve data connectivity in text-based personality prediction using multiple data sources mapping. (2023). Journal of Scientific &amp; Industrial Research, 82(01). doi:10.56042/jsir.v82i1.70218 
4.	Ryan, G., Katarina, P., & Suhartono, D. (2023). MBTI personality prediction using machine learning and smote for balancing data based on statement sentences. Information, 14(4), 217. doi:10.3390/info14040217 
5.	Maharani, W., & Effendy, V. (2022). Big five personality prediction based in Indonesian tweets using machine learning methods. International Journal of Electrical and Computer Engineering (IJECE), 12(2), 1973. doi:10.11591/ijece.v12i2.pp1973-1981 
6.	Karanatsiou, D., Sermpezis, P., Gruda, D., Kafetsios, K., Dimitriadis, I., & Vakali, A. (2022). My tweets bring all the traits to the yard: Predicting personality and relational traits in online social networks. ACM Transactions on the Web, 16(2), 1–26. doi:10.1145/3523749 






The social media can be considered a goldmine of information, as it holds a vast amount of data whose potential remains untapped and whose power have not been fully utilized. However, there are quite a number of challenges associated with dataset limitation, some of which this paper intends to address. Firstly, despite the massive amount of content generated daily on these platforms, only a small amount is accessible to researchers via API due to data privacy concerns(Manovich, 2011). In addition, data collected from different platforms is likely to have demographics focus and platform-specific behavior. For example, a study by Jaidka et al. (2018) on the differences between Facebook and Twitter in self-disclosure and psychological traits discovered some useful insights that will inform this study. Firstly, they found a higher predictive accuracy on facebook and attributed it to greater self-closure and longer text length  allowing more detailed and personal expression on facebook. They also found out that a model trained on one platform performed poorly when applied to another and both platforms had similar predictive power when equal sample size are used  