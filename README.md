# KUL_MDA
Modern Data Analytics Project (2021 spring)

This repositary contains four folders, one requirement.text, and one Readme file.
To keep consistency, please load requirement.txt in your environment before running our python program.

## 1. Description of Data

Heat Wave spread sheet is scraped from EMDAT(https://public.emdat.be). This website records heat wave that has happened in the past. We download all the variables between 2000 to 2020, which include disaster id, in which country did it happen, temperature, on what time did it happen, the total death number etc. Although this sheet is quite informative, it has a lot of missing values in temperature, the exact happening date period or total death. What's worse, there is only around 200 records. A big data analysis needs more samples to carry out. After discussion, we decided to search for the data of temperature and relative humidity, which are the key variables to determine heat wave. Despite of digging more information about the characteristics in heat wave, we wish to find more about the impact on GDP resulting from heatwaves. Therefore, GDP information by country is also collected. 

Relative humidity data is retrieved from European Climate Data Store (https://cds.climate.copernicus.eu/cdsapp\#!/dataset/ecv-for-climate-change?tab=form). A monthly averaged world-wide relative humidity data set between 2000 to 2020 is scraped from the website. However, the original format of the file is GRIB, a special file format to store geographical information. Therefore, a python package PyGrib is loaded to transform the data sets from GRIB to CSV for further exploration. The transformed CSV files have two groups. One is the monthly data of world's geographical latitude and longitude data. The other one is the monthly average data of relative humidity. Each cell in the geographical file maps to the same location in the relative humidity file. Thus, a relative humidity value on that particular position can be spotted. Based on the characteristic of these files, we write a program to extract the relative humidity value of a particular city based on its latitude and longitude that we gathered from the internet. 

The variables in our cleaned files are disaster numbers, each month from 2000 to 2020, the country where that disaster happened, and the monthly relative humidity value for that particular month and year.

## 2. Description of Scripts

Scripts folder contains our main deliverables - python program. We strongly recommend you just run our main modelling and visualization notebook, which exclude stage 0. We use stage 0 notebook to transform massive unstructured data into the one we can use. It is quite time consuming. Their results are stored, and can be directly read in later stage.

The ordering of the jupyter notebooks:
stage 0 two notebooks;
1-Predict Heat Waves
2-MDA_visualization
3-Impact of Heat Waves
