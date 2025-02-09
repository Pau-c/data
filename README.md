# Data analysis and ML projects



---

## 1970's survey about school unrest

 <div align="center">
  
<!-- PROJECT SHIELDS -->
[![deepnoteBadge][deepnote-shield]][deepnote-url]
[![pythonBadge][python-shield]][python-url]
[![pandasBadge][pandas-shield]][pandas-url]
[![plotlyBadge][plotly-shield]][plotly-url]
[![seabornBadge][seaborn-shield]][seaborn-url]
[![matplotlibBadge][matplotlib-shield]][matplotlib-url]
<!-- PROJECT SHIELDS -->
  
 </div>
 
The goal of this project is to update the survey commissioned by the US government during the Vietnam war to look into university students' attitudes toward campus protests that took place during that time. The commission's objective was to analyze the causes of unrest, identify patterns, and make recommendations for preventing or addressing similar situations in the future.  

### Data Source
You can find the files [here](https://catalog.archives.gov/id/610064) . The most important ones are the raw file RG220.PCC.CAMPUS with the survey results and the one containing the technical documentation that specifies which position corresponds to each column and how to interpret the answers, which are originally presented as numerical values.

Based on those instructions, it's possible to determine how to parse the file so that it can be analyzed using python. The survey originally  used an **IBM 360** machine, which had punched cards for input. These cards were made of stiff paper with holes punched in specific locations, each hole representing a bit of data. It was coded into an ASCII text at a later date:

The ASCII file looked like this:
<img src="https://github.com/Pau-c/data/blob/7c4c24c2f6b304b590bccacdc8b566f99c24d2d7/format.jpg" alt="original format"  />

After the ETL process:
<img src="https://github.com/Pau-c/data/blob/bd1c0096c1288bd4d85902c5a6f42b74890c75f2/formatted.jpg" alt="new format"  />

### Project details

- __Data Cleaning__: After the construction of the dataframe, the next steps involve cleaning up the dataset to prepare it for analysis. This includes handling missing values, removing nans, and improving performance.
- __Data Analysis__: The exploratory analysis delves into several key areas: identifying how many completed the survey, examining the characteristics of the surveyed institutions, and understanding the causes of the protests as perceived by both the administration and the student body.
- __Visualization__: The insights are presented using various chart types, including bar and pie charts, violin plots, heat maps and word clouds, among others.

### Live demo

 [Part I](https://deepnote.com/workspace/projects-975f-efed272e-9ae6-4c78-9f2e-e4a5eb60a3ea/project/Projects-9f46395a-c0d8-45cb-b6d3-50191b329853/notebook/Survey-US-1970-campus-unrest-I-intro-f6737292381a4acbbdb13fb6ef8a6164?utm_source=share-modal&utm_medium=product-shared-content&utm_campaign=notebook&utm_content=9f46395a-c0d8-45cb-b6d3-50191b329853) |  [Part II](https://deepnote.com/app/projects-975f/Projects-9f46395a-c0d8-45cb-b6d3-50191b329853?utm_source=share-modal&utm_medium=product-shared-content&utm_campaign=data-app&utm_content=9f46395a-c0d8-45cb-b6d3-50191b329853)
 
---  

## Prediction model for fatalities in school shootings based on US state


 <div align="center">
  
<!-- PROJECT SHIELDS -->
[![colabBadge][colab-shield]][colab-url]
[![pythonBadge][python-shield]][python-url]
[![pandasBadge][pandas-shield]][pandas-url]
[![sklearnBadge][sklearn-shield]][sklearn-url]
[![matplotlibBadge][matplotlib-shield]][matplotlib-url]
<!-- PROJECT SHIELDS -->
  
 </div>
 
Exploratory paper for the class 'Data analysis II'. The objective of this work is to apply a random model to a dataset and evaluate its performance. In this case, the Random Forest algorithm, a supervised learning method based on decision trees, was randomly chosen to predict the presence of fatalities based on the state where the incident occurred.

### Data Source

This [dataset](https://drive.google.com/file/d/1VA8g3qU2EX8QzH74a_l_abqRqGklraWz/view?usp=sharing) contains information on mass shootings in the USA collected by the [Gun Violence Archive](https://www.gunviolencearchive.org/reports) from 2014 to 2023. 

### Project details

- __Preparation__: use of one hot encoding to convert categorical data into a numerical format.
- __Data splitting__: Split the data into training and testing dataset.
- __Model selection and training__: Apply the random forest model.
- __Model evaluation__ Evaluate the model using metrics such as accuracy, precision, recall, F1 score, confusion matrix, and AUC-ROC.
- __Hyperparameter tuning__:  Optimize the model's performance through hyperparameter tuning.
- __Model re-evaluation__: Re-evaluate the model after tuning.


### Live demo

 [Colab Notebook](https://colab.research.google.com/drive/19Xrg2eJlaqHi7XWPtUh_wpdTHBU-itj_?usp=sharing) 
 
---  


<!-- PROJECT SHIELDS VARIABLES-->
[colab-shield]:https://img.shields.io/badge/Live-Collab-black?style=flat&labelColor=%23808080k&color=de6d40&logo=googlecolab&logoColor=white
[colab-url]: https://colab.google/
[deepnote-shield]:https://img.shields.io/badge/Live-Deepnote-black?style=flat&labelColor=%23808080k&color=de6d40&logo=deepnote&logoColor=white
[deepnote-url]: https://deepnote.com/
[matplotlib-shield]:https://img.shields.io/badge/Data_Viz-matplotlib-black?style=flat&labelColor=%23808080k&color=fec260
[matplotlib-url]:https://matplotlib.org/
[pandas-shield]:https://img.shields.io/badge/Data_analysis-Pandas-black?style=flat&labelColor=%23808080k&color=453076&logo=pandas
[pandas-url]:https://pandas.pydata.org/
[python-shield]:https://img.shields.io/badge/Language-Python-black?style=flat&labelColor=%23808080k&color=2a0944&logo=python&logoColor=white
[python-url]: https://www.python.org/
[plotly-shield]:https://img.shields.io/badge/Data_Viz-Plotly-black?style=flat&labelColor=%23808080k&color=9ABF80&logo=plotly&logoColor=white
[plotly-url]: https://plotly.com/python/
[seaborn-shield]:https://img.shields.io/badge/Data_Viz-Seaborn-black?style=flat&labelColor=%23808080k&color=a12568
[seaborn-url]: https://seaborn.pydata.org/
[sklearn-shield]:https://img.shields.io/badge/ML-sklearn-black?style=flat&labelColor=%23808080k&color=teal&logo=scikitlearn&logoColor=white
[sklearn-url]: https://scikit-learn.org/
