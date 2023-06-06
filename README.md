# QSS One Quarter Project Repository

# **Abstract**

Access to healthcare is a fundamental right, yet the United States lags behind other countries regarding healthcare access, efficiency, equity, and outcomes. Community healthcare centers (CHCs) are critical in providing accessible and affordable healthcare services to underserved populations, including those with low health literacy (HLS). To qualify for federal funding, CHCs must meet specific criteria, but these may not capture the full extent of healthcare disparities. This study aims to explore the relationship between HLS and the placement of CHCs to assess whether incorporating HLS as an additional indicator can enhance CHC designation accuracy. Geospatial analysis was conducted using data from the National Association of Community Health Centers, the National Assessment of Adult Literacy, and the US Census Bureau. The findings reveal a slight inverse relationship between CHC density and HLS, suggesting that areas with low HLS may be a predictor for CHC density, but are still not adequately served by CHCs. These findings indicate a need to revisit current funding criteria to ensure equitable healthcare access. These findings underscore the importance of considering HLS in healthcare policy and planning to achieve equitable access and better health outcomes.

# **Scripts**

[CHC_script.ipynb](https://github.com/jwang3939/HLS_CHC/blob/main/scripts/CHC_script.ipynb)
* Scrape NACHC website for all PDFs
* Convert PDFs to RTFs
* Scrape RTFs for all street addresses
* Batch geocode street addresses and export out to CSV

[HLS_script.ipynb](https://github.com/jwang3939/HLS_CHC/blob/main/scripts/HLS_script.ipynb)
* Load HLS data
* Scrape Census website for shapefiles
* Create GeoDataFrames for shapefiles/HLS and geocodes
* Plot a choropleth with HLS GeoDataFrame
* Run OLS regression
