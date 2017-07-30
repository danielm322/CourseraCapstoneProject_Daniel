### Coursera Data Science Capstone Project


This application is the capstone project for the Coursera Data Science specialization.

******

#### Objective

The main goal of this project is to build a shiny application that is able to predict the next word after an arbitrary number of words. To this end, many tasks were necessary, such as getting and cleaning the data, exploratory analysis, modeling, testing, and app development and deployment.

The data that is used to build the model comes from a corpus called [HC Corpora](http://www.corpora.heliohost.org/). 

All processes were done in the R programming language, and some R packages

******

#### Methods & Models

After creating a data sample from the HC Corpora data, this sample was cleaned by performing profanity filtering, marking beginning and end of sentences, conversion to lowercase, expansion of contracted forms, conversion of numbers to token "num", removing punctuation except apostrophes, links, additional white spaces, and special characters.
This data sample was then [tokenized](http://en.wikipedia.org/wiki/Tokenization_%28lexical_analysis%29) into [*n*-grams](http://en.wikipedia.org/wiki/N-gram). Fourgrams, threegrams, bigrams, and unigrams were extracted from the data.

To estimate sentence probabilities, and next word predictions,  Modified [Kneser-Ney smoothing](https://en.wikipedia.org/wiki/Kneser%E2%80%93Ney_smoothing) was used, as proposed in Chen and Goodman's [paper](https://dash.harvard.edu/bitstream/handle/1/25104739/tr-10-98.pdf?sequence=1), section 3. 

******

#### How to use the Application

Enter text freely in upper-case or lower-case, and three predictions will appear below as you finish typing every word. The predictions appear always in lower-case. The word "num" stands for any number of any length. Please note that periods are treated always as end-of-sentence markers, so abbreviations like Mr. or Mrs. should be typed without the period, i.e.: Mr or Mrs

******

#### Additional Information

* The whole code of this application, as well as all the milestone report, related scripts, this presentation  etc. can be found in this GitHub repo: [https://github.com/danielm322/CourseraCapstoneProject_Daniel](https://github.com/danielm322/CourseraCapstoneProject_Daniel)

* This pitch deck is located here: [http://rpubs.com/](http://rpubs.com/)

* Learn more about the Coursera Data Science Specialization: [https://www.coursera.org/specializations/jhu-data-science](https://www.coursera.org/specializations/jhu-data-science)
