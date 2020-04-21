# finalproject.github.io
#final project for practical machine learning
#LOADING LIBRARIES AND IMPORT DATA
Loading the required libraries andrRead training and testing data. Identifying “”, “NA” and “#DIV/0!” as “NA” (missing value) everywhere.
library(caret)
library(randomForest)
library(rpart)
url.train <- "https://d396qusza40orc.cloudfront.net/predmachlearn/pml-training.csv"
url.test <- "https://d396qusza40orc.cloudfront.net/predmachlearn/pml-testing.csv"
training <- read.csv(url(url.train), na.strings = c("NA", "", "#DIV0!"))
testing <- read.csv(url(url.test), na.strings = c("NA", "", "#DIV0!"))
