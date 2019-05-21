# Pharmaceutical-ML

In biopharmaceuticals, producing a pure and potent therapy is important for patient safety and efficacy. This project utilizes three different data sets to explore relationships between the quality attributes and process parameters of fictional biopharmaceutical products.  We use different machine learning techniques to create predictive models allowing us to work proactively rather than reactively.
 
Where do expiration dates come from?  Is a result expected or unexpected based on historical data? 
- We demonstrate the relationship between drug product quality, shelf-life, and temperature.  This includes linear regression analysis to describe the relationship mathematically and visually. We analyze samples of multiple lots of lumab, primarily at the 5C condition, over a period of three years.
What contributes to our product variability?
- In biopharmaceuticals, consistency and control are king and queen.  While inherent process variability is to be expected based on numerous inputs (chemicals, reagents, cell lines, materials, analysts, instruments, sites, etc.) our goal is to understand our sources of variability just a little bit better.  Thus, we perform cluster analysis and an analysis of variance (ANOVA) on a data set consisting of a reference material analyzed hundreds of times over a period of years.
Can we detect an unexpected trend or a single outlier from several different measures?
- Detecting an outlier or sharp trend on an x/y axis isn’t particularly difficult.  However, we have multiple measures for our process. Rather than generate control charts for each of them, we use an autoencoder neural network to encode a single “health score” for the process.  This allows us to monitor a single trace and detect values or trends as they exceed a specified threshold.  Given a model trained on the results from historical lots we detect if a new batch is trending up or down.

## Methods and Tools
 
Pulling the data:
- Oracle queries
- Exporting to CSV
Shaping the data:
- Pandas and numpy
Analyzing the data:
- Scikit-learn
- researchPy
- stats.models
- Tensorflow
- Visualizing the data:
- Matplotlib
- seaborn
