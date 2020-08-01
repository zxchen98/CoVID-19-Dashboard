Description：

This online dashboard presents spatial distribution and dynamics of COVID-19 in San Diego county as related to public health, social-economic, and demographic variables. It is implemented in ArcGIS Online and is updated using several Python scripts written with ArcGIS API for Python.
Key features of the dashboard are:
-	It allows users to simultaneously visualize spatial patterns and trends of the infection and identify associated risk factors. Different sections of the dashboard are dynamically linked. For example, selecting a Zip code from a list updates both the maps and the diagrams reflecting selected risk factors.
-	It integrates data from several sources, including current and historical COVID-19 infection data (by Zip codes), hospitalization, ICU use, and death time series (for the entire county), and selected indicators from the American Community Survey. 
-	The dashboard is automatically updated. Python scripts retrieve current infection counts from the county sources, process and reformat the data, and update feature layers underlying the dashboard, to keep the maps, charts, and models up-to-date. The scripts are in my GitHub repository at …
-	A separate map and a gage control show predicted case counts by Zip codes. The predictions are generated using ARIMA time series model, which integrates several risk factors in the forecast. Initial model runs (in late May) forecasted an upward infection trend in about two-thirds of the Zip code areas. Now all but two Zip codes show an upward trend.
-	Maps include a heat map reflecting confirmed COVID cases (to show the infection as a continuous surface and de-emphasize Zip code boundaries); a map of confirmed cases; and predictions
-	Hospitals and COVID testing facilities, with their profiles and hours of operation, are also shown, to help people navigate to these locations as needed.

Credits:
Author: Xiangchen Zhao, UCSD undergraduate program in data science. This dashboard project is developed as part of UCSD DSC 198 “Directed Group Study” (Spring 2020) and DSC 199 “Independent Research” (Summer 2020) classes.
Data sources: San Diego County Health and Human Services; US Census Bureau 

