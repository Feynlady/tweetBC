# tweetBC
Python script for binary classification of social media related text (tweets, comments...etc).

## Motivation

Filtering posts, comments and tweets has become a day to day issue concerning the public usage of social networks. Balancing the need for freedom of speech and avoiding the spreading of hate, racism and homophobia has always been a challenging task, so challenging that discerning the two still quite often requires human actors. Unfortunately, due to the extremely high rate of growth of the amount of data produced by social media users, human intervention is not feasible in all cases, and therefore a text classifier could easily come in handy. The classifiers and models presented in this project could easily be re-applied to a different dataset to discern regular from discriminatory comments. For now, the classification is limited to the polarity of the tweets in terms of positive and negative emotions.

## Framework
Built with <a href="https://jupyter.org" target="_blank">Jupyter Notebook</a>.</h4>


## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install:
* numpy
* pandas
* seaborn
* matplotlib.pyplot
* re
* sklearn
* nltk

```bash
pip install numpy
pip install pandas
pip install seaborn
pip install matplotlib.pyplot
pip install re
pip install sklearn
pip install nltk
```

## Files

Two files are needed for the script to run:
*NLP_Project: this file constitutes the main script, where the parts that need to be necessarily executed are marked as such. Different classifiers can be run separately, according to one's goal.
*AllData.csv: whole dataset. Different parts of the dataset are used as training and test sets.

It is also required to download the [DATASET](https://www.kaggle.com/kazanova/sentiment140) and include it in the same folder as the main script NLP_Project.

## Usage

When run, the NLP_Project script cleans, splits and reorganizes the data in the main dataset. The AllData.csv contains 1.600.000 lines of classified tweets, of which only 1.25% (20.000 lines) is used to train the models.
Following the data processing, the script is organised base on the language model, vectorization method and classifier used per cell. A total of three classifiers is used on two models.

## Bag of Words
* Näive-Bayes - Tested accuracy: 74.71%
* SVM - Tested accuracy: 76.2%
* Logistic Regression - Tested accuracy: 74.57%
## TF-IDF
* Näive-Bayes - Tested accuracy: 74.81%
* SVM - Tested accuracy: 76.57%
* Logistic Regression - Tested accuracy: 76.46%

## Tests
* Bag of Words
  * Näive-Bayes
  ![Näive-Bayes](https://github.com/Feynlady/tweetBC/blob/master/Test_pictures/Näive_Bayes.png)
  * SVM
  ![SVM](https://github.com/Feynlady/tweetBC/blob/master/Test_pictures/SVM.png)
  * Logistic Regression
  ![LogReg](https://github.com/Feynlady/tweetBC/blob/master/Test_pictures/LogReg.png)
* TF-IDF
   * Näive-Bayes
   ![TF-IDF Näive-Bayes](https://github.com/Feynlady/tweetBC/blob/master/Test_pictures/TFIDF_Näive_Bayes.png)
   * SVM
   ![SVM](https://github.com/Feynlady/tweetBC/blob/master/Test_pictures/TFIDF_SVM.png)
   * Logistic Regression
   ![LogReg](https://github.com/Feynlady/tweetBC/blob/master/Test_pictures/TFIDF_LogReg.png)

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Credits
Amanda C. Kane
Silvia Fallone
