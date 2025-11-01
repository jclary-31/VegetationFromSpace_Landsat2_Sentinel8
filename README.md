# CODE  (conflict between google collab and github) 
-> see https://colab.research.google.com/github/jclary-31/VegetationFromSpace_Landsat2_Sentinel8/blob/main/Multispectral_Satellite_test.ipynb#scrollTo=xdb1SpPSt4xG

# GOAL
Here I want to test Landsat2 and Sentinel8 multispectral observations from space to analyze vegetation health and droughness in region under water stress. The region taken is approximatively Andalousia (Spain). This is my first project using google earth engine, but figures are for now encouraging. This porject is exploratory by nature

# Main issues
 Mains issues are :
1) same vegetation index give different figure for Landsat and for Sentinel. Reason is unclear.
   
2) I made a .ipynb file on google colab, mainly for vizualisation  but I cannot save the figure in widget (a 2 map upon a google map). Widget existence give erros on github... Only way to play around is to resafe a without widget version by using locally (not on collab) the comment python -m  jupyter nbclassic, then clear widget, save the 0 widget version and uploated it on github. This version is read by github... seems an old problems

3) Time serie analysis show some inconstency betwen index coming from Landsat and from Sentinel.

4) figure for satvi index show nothing. A bug?
    

# Good sides
1) map are nice,  I can save them locally as tif or as jpg and then reloaded them for another analysis
  
2) time serie analysis into seasonal/harmonic + trend + noise  seems to works well for NDVI index. As ndvi is an andex for vegetation, having shown periodicity seems good. Other index remains to be tested. In general, I think one year data is maybe not enough to this  analysis

3) Prediction using ARIMA algorithm but needs before hand study to find a good parametrisation. Prediction needs to be compared with real observations, and I think more data would be better here

4) next idea would be to have a summer map for river and lake in the area by using an existing neural network specialized into image classification. Once this is done, I could make an animation for each summer from 2000 to 2025 (for example) and establish a metric.


 potential are really huge here. One could try to study desertification processes in past years, or 2024 flood near Malaga
