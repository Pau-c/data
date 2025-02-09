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
 
The goal of this project is to update the survey commissioned by the US government during the Vietnam war to investigate university students' attitudes toward campus protests that took place during that time. The commission's objective was to analyze the causes of unrest, identify patterns, and make recommendations for preventing or addressing similar situations in the future.  

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

 [Notebook](https://deepnote.com/app/projects-975f/Projects-9f46395a-c0d8-45cb-b6d3-50191b329853?utm_source=share-modal&utm_medium=product-shared-content&utm_campaign=data-app&utm_content=9f46395a-c0d8-45cb-b6d3-50191b329853)

---  

<!-- PROJECT SHIELDS VARIABLES-->
[deepnote-shield]:https://img.shields.io/badge/Live-Deepnote-black?style=flat&labelColor=%23808080k&color=red&logo=deepnote&logoColor=white
[deepnote-url]: https://deepnote.com/
[matplotlib-shield]:https://img.shields.io/badge/Data_Viz-matplotlib-black?style=flat&labelColor=%23808080k&color=teal
[matplotlib-url]:https://matplotlib.org/
[pandas-shield]:https://img.shields.io/badge/Data_analysis-Pandas-black?style=flat&labelColor=%23808080k&color=violet&logo=pandas
[pandas-url]:https://pandas.pydata.org/
[python-shield]:https://img.shields.io/badge/Language-Python-black?style=flat&labelColor=%23808080k&color=black&logo=python&logoColor=white
[python-url]: https://www.python.org/
[plotly-shield]:https://img.shields.io/badge/Data_Viz-Plotly-black?style=flat&labelColor=%23808080k&color=teal&logo=plotly
[plotly-url]: https://plotly.com/python/
[seaborn-shield]:https://img.shields.io/badge/Data_Viz-Seaborn-black?style=flat&labelColor=%23808080k&color=teal
[seaborn-url]: https://seaborn.pydata.org/
