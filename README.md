# KUL_MDA
Modern Data Analytics Project (2021 spring)

This repositary contains four folders (scripts, data, outputs), one requirement.text, and one Readme file.
To keep consistency, please load requirement.txt in your environment before running our python programs.

## 1. Description of Data

1. Heat Wave spread sheet is scraped from EMDAT (https://public.emdat.be). 
2. Relative humidity data is retrieved from European Climate Data Store (https://cds.climate.copernicus.eu/cdsapp\#!/dataset/ecv-for-climate-change?tab=form). 
3. Temperature data is retrieved from the Meteostat website.
4. Relative GDP data is retrieved from The Organisation for Economic Co-operation and Development.

## 2. Description of Scripts

Scripts folder contains our main deliverables - python programs. We strongly recommend you just run our main modelling and visualization notebooks, which exclude collecting weather data. We use "collect-" notebooks to transform massive unstructured data into the one we can use. It is quite time consuming. Their results are stored, and can be directly read in later stage.

The ordering of the jupyter notebooks:
Collect Data - Weather
Collect Data - Relative Humidity
1-Predict Heat Waves
2-MDA_visualization
3-Impact of Heat Waves
