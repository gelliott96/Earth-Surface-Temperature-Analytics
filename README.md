# Earth-Surface-Temperature-Analytics

The impact of climate change on Earth has increased significantly over the last century, with human activity being the main contributor. The effects are seen today with the melting of ice caps causing the rise of sea levels and extreme weather conditions. Therefore, the purpose of this paper is to investigate and make predictions based on the changes in average land temperature on Earth from the year 1850 to date. This is a Big Data Analytics project implemented on Apache Spark with the models used to make predictions built through Apache Spark's machine learning library MLlib.

The topic of global warning has become a very important
point of discussion because of human activity over many
years. Several consequences from global warming include the
increase in global temperature, sea levels rising and extreme
events such as the forest fires in Australia in 2020. Global
warming is therefore very real with such changes and hence
possible forthcoming disasters on Earth.

Due to the serious repercussions to the planet and its
inhabitants currently facing us because of climate change,
the United Nations (UN) adopted the Paris Agreement on
12 December 2015 which was subsequently enforced on 4
November 2016. The purpose of the Paris Agreement is to
provide guidelines and support member countries on how to
limit global warming and hence combat the dangerous effects
of climate change.

Therefore, taking the above into account, the purpose of
this project is to investigate global warming in the context
of global land temperature in First World countries between
the years 1850 and 2013 which follows the complexity of the
dimensions Volume, Variety and Velocity associated to a Big
Data problem. This specific timeframe that is selected is due
to the increased industrialisation throughout the world since
the mid-20th century.

The main goals of this project is to:
1) Investigate which First World Countries (top five) have
had the biggest change in average land temperature
between 1850 and 2013.
2) Investigate which Cities (top five) of the five First World
Countries from Goal 1 have seen the biggest change in
average land temperature between 1850 and 2013.
3) Predict the average land temperature of the City found
to have the greatest change in average land temperature
from Goal 2 for the years 2014-2020.
To achieve the goals stated above, a data analytic pipeline
is used.

The pipeline for this project comprises of
the following stages:
1) Data Collection
2) Data Transformation
3) Feature Engineering (Goal 3 only)
4) Algorithm Selection (Goal 3 only, for Predicitve Analysis)
5) Training (Goal 3 only, for Predicitve Analysis)
6) Testing (Goal 3 only, for Predicitve Analysis)
7) Descriptive or Predictive Analysis
8) Data Visualisation

Due to the nature of the goals, i.e. Goal 2 depends on the
results of Goal 1 and Goal 3 depends on the results of Goal
2, we shall implement the data analytic pipeline three times,
once for each goal.

Due to the large scale of the data used in this project, i.e.
Multicore Big Data processing, we will use SparkSQL and
the DataFrame API (PySpark) from Apache Spark to create,
transform and perform analytics on Spark DataFrames, which
is executed via a Hadoop cluster on Databricks. The datasets
used in this project are imported and stored to the Databricks
File System, DBFS.

The techniques or algorithms that will be used in this
project are dependent on the aims of the project outlined
in the subsection Goals. For Goals 1 and 2, the technique
used to achieve these goals involves taking the maximum
and minimum yearly average land temperature for each First
World country between 1850 and 2013, taking the difference
and calculating the absolute value. For Goal 3, we intend to
make prediction, hence we will use Machine Learning (ML)
algorithms, or more specifically Supervised Machine Learning
algorithms: Linear Regression, Decision Tree Regression and
Random Forest Regression. These regression algorithms are
used because we intend to make predictions based on the
continuous quantities yearly average land temperature.

NOTE: Due to the large file size of the dataset GlobalLandTemperaturesByCity.csv, this dataset is unavailable in this repository. For access to this dataset, please see the following link https://www.kaggle.com/berkeleyearth/climate-change-earth-surface-temperature-data.
