<p style="text-align: right">
September 19, 2022</p>

**GDP-Based Recession Indicator Index**

In this dataset, there are a set of probabilities associated with different periods of the United States’ economy’s history that demonstrate how likely the United States experienced an economic recession during each particular quarter. The data will be accessed from the economic database of the Federal Reserve Bank of St. Louis by extracting the GDP-Based Recession Indicator Index dataset. The collected data is presented in a combination of two columns, including DATE (ranging from October of 1967 to January of 2022, and represented by quarter) and James Hamilton GDP-Based Recession Indicator Index (abbreviated as JHGDPBRINDX) data objects (ranging from values of 0.0 to 100.0; values growing above 67.0 indicate an entrance into a recession and values following that threshold and dropping below 33.0 indicate an exit from a recession). 

Based on the local maximum and local minimum values in the dataset, it appears as though this data may be useful for anticipating when another economic recession may occur next. 

    The problem for this project to attempt to solve is the following: 
    
How can we model this data in order to predict future periods of economic recession in the United States?

    The methods that are planned to test solutions to this problem are as follows:
 
**Time Series Analysis:** *by Date and Marginal Differences* - Visualizing change over time to find trends in data, such as identifying oscillation and outliers.

**Deep Learning:** *of GDP-Based Recession Indicator Index values* - Training an algorithm to develop a neural network for understanding incremental change of data values.

    These methods will be tested using techniques following this procedure: 
    
* Using the partial autocorrelation function (PACF) to determine ideal values to build Autoregressive Integrated Moving Average (ARIMA) models for describing temporal evolution of the data.
* Analyzing the Residuals and Akaike information criterion (AIC) scores of tested ARIMA models to infer linear modeling consistency and predictive significance.
* Testing a wide range of batch sizes and learning rates in a variety of Artificial Neural Networks (ANN) models with stochastic gradient descent in order to forecast further change of index values.

The biggest challenge to anticipate facing in this exploration is the aspect of fluctuation in the GDP-Based Recession Indicator Index’s set of values. Specifically, it may prove to require keen attention to detail due to the seemingly oscillating nature of variation in the dataset. To address this, it may be valuable to utilize more meticulous code when preparing the data to be processed by the programming focused on developing models for forecasting new data (particularly, the ARIMA and ANN models). In this case, building effective predictive models may also become more successful if the target variable is binarized by splitting the data into two groups based on whether the economy entered or exited a recession (yielded an index value greater than 67% or less than 33%, respectively) during each indicated quarter. Following this, a comparison between this approach and an approach that does not sort the data may lead to clearer results.

Stakeholders who will find this research and solution valuable include professionals involved in the United States’ economy (as government officials, industrial executive leaders, or even simply agents of its commercial sectors), as well as individuals with investment accounts or active engagement with the stock market. Considering the widespread impact that economic recessions have historically had on all socioeconomic levels in the United States, it would be difficult to find a person with no reason to be interested in the predictability of economic recession. 

    The audience will benefit from these findings by gaining the following:
    
* An understanding of historical periodicity of peaks of economic recession in the United States.
* Familiarity with using a federal index for indicating economic recession based on GDP.
* A perspective on the factors and obstacles involved in predicting economic recession.

As a result of these parameters and expectations, perhaps this research may serve as a reference for providing insight and advice on analyzing economic recession in relation to GDP.

---

**Source Citation & Link to Dataset:**

Hamilton, James, GDP-Based Recession Indicator Index [JHGDPBRINDX], retrieved from FRED, Federal Reserve Bank of St. Louis; https://fred.stlouisfed.org/series/JHGDPBRINDX, September 15, 2022.

[Description of dataset, including its defining properties and important limiting factors](https://fred.stlouisfed.org/series/JHGDPBRINDX)

[Further background on the gathering and understanding of the data](http://econbrowser.com/recession-index)

[Downloadable CSV file copy of dataset, as used in this study](https://fred.stlouisfed.org/graph/fredgraph.csv?bgcolor=%23e1e9f0&chart_type=line&drp=0&fo=open%20sans&graph_bgcolor=%23ffffff&height=450&mode=fred&recession_bars=off&txtcolor=%23444444&ts=12&tts=12&width=1168&nt=0&thu=0&trc=0&show_legend=yes&show_axis_titles=yes&show_tooltip=yes&id=JHGDPBRINDX&scale=left&cosd=1967-10-01&coed=2022-01-01&line_color=%234572a7&link_values=false&line_style=solid&mark_type=none&mw=3&lw=2&ost=-99999&oet=99999&mma=0&fml=a&fq=Quarterly&fam=avg&fgst=lin&fgsnd=2020-02-01&line_index=1&transformation=lin&vintage_date=2022-09-17&revision_date=2022-09-17&nd=1967-10-01)
