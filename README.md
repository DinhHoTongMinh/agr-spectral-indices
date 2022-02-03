# Vegetation Indices
**Contributors:** *Michele Croci*, *Giorgio Impollonia*, *Andrea Marcone* and *Stefano Amaducci*

This repository is inspired by `"davemlz/awesome-ee-spectral-indices"`, but with the aim of collecting specific vegetation indices for crop monitoring 🌱🌾 and precision agriculture 🚜.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5957470.svg)](https://doi.org/10.5281/zenodo.5957470)

The ready-to-use curated list of spectral indices ([check the list here](https://github.com/MCroci/agr-spectral-indices/blob/master/Output/)) for remote sensing applications is presented here. The list is available in the csv formats ([CSV](https://github.com/MCroci/agr-spectral-indices/blob/master/Output/Spectral%20Vegetation%20Indices.csv)).

## Attributes
Each item of the list has the following attributes:
- `short_name`: Short name of the index (e.g. `"NDVI"`).
- `long_name`: Long name of the index (e.g. `"Normalized Difference Vegetation Index"`).
- `formula`: Expression/formula of the index (e.g. `"(N - R)/(N + R)"`).
- `bands`: List of required bands/parameters for the index computation (e.g. `["N","R"]`).
- `reference`: Link to the index reference/paper/doi (e.g. `"https://doi.org/10.1080/01431169608948714"`).
- `type`: Type/application of the index (e.g. `"Biomass"`).
- `date_of_addition`: Date of addition to the list (e.g. `"2022-01-01"`).
- `contributor`: GitHub user link of the contributor (e.g. `"https://github.com/mcroci"`).

## Expressions

The formula of the index is presented as a string/expression (e.g. `"(N - R)/(N + R)"`) that can be easily evaluated. The parameters used in the expression for each index follow this standard:

<table>

<tr>

<th> Description </th>
<th> Standard </th>
<th> Sentinel-1 </th>
<th> Sentinel-2 </th>
<th> Landsat-8 </th>
<th> Landsat-457 </th>
<th> MODIS </th>
</tr>

<tr>

<td>Aerosols</td>
<td>A</td>
<td></td>
<td>B1</td>
<td>B1</td>
<td></td>
<td></td>

</tr>

<tr>

<td>Blue</td>
<td>B</td>
<td></td>
<td>B2</td>
<td>B2</td>
<td>B1</td>
<td>B3</td>

</tr>

<tr>

<td>Green</td>
<td>G</td>
<td></td>
<td>B3</td>
<td>B3</td>
<td>B2</td>
<td>B4</td>

</tr>

<tr>

<td>Red</td>
<td>R</td>
<td></td>
<td>B4</td>
<td>B4</td>
<td>B3</td>
<td>B1</td>

</tr>

<tr>

<td>Red Edge 1</td>
<td>RE1</td>
<td></td>
<td>B5</td>
<td></td>
<td></td>
<td></td>

</tr>

<tr>

<td>Red Edge 2</td>
<td>RE2</td>
<td></td>
<td>B6</td>
<td></td>
<td></td>
<td></td>

</tr>

<tr>

<td>Red Edge 3</td>
<td>RE3</td>
<td></td>
<td>B7</td>
<td></td>
<td></td>
<td></td>

</tr>

<tr>

<td>Red Edge 4</td>
<td>RE4</td>
<td></td>
<td>B8A</td>
<td></td>
<td></td>
<td></td>

</tr>

<tr>

<td>NIR</td>
<td>N</td>
<td></td>
<td>B8</td>
<td>B5</td>
<td>B4</td>
<td>B2</td>

</tr>

<tr>

<td>SWIR 1</td>
<td>S1</td>
<td></td>
<td>B11</td>
<td>B6</td>
<td>B5</td>
<td>B6</td>

</tr>

<tr>

<td>SWIR 2</td>
<td>S2</td>
<td></td>
<td>B12</td>
<td>B7</td>
<td>B7</td>
<td>B7</td>

</tr>

<tr>

<td>Thermal 1</td>
<td>T1</td>
<td></td>
<td></td>
<td>B10</td>
<td>B6</td>
<td></td>

</tr>

<tr>

<td>Thermal 2</td>
<td>T2</td>
<td></td>
<td></td>
<td>B11</td>
<td></td>
<td></td>

</tr>

</table>

Additional index parameters also follow a standard:

- `g`: Gain factor (e.g. Used for EVI).
- `L`: Canopy background adjustment (e.g. Used for SAVI and EVI).
- `C1`: Coefficient 1 for the aerosol resistance term (e.g. Used for EVI).
- `C2`: Coefficient 2 for the aerosol resistance term (e.g. Used for EVI).
- `cexp`: Exponent used for OCVI.
- `nexp`: Exponent used for GDVI.
- `alpha`: Weighting coefficient used for WDRVI, BWDRVI and NDPI.
- `gamma`: Weighting coefficient used for ARVI.
- `omega`: Weighting coefficient used for MBWI.
- `sla`: Soil line slope.
- `slb`: Soil line intercept.



# Spectral Indices by Type

## Vegetation 🌱

### A

- [AFRI1600](https://doi.org/10.1016/S0034-4257(01)00190-0): Aerosol Free Vegetation Index (1600 nm).
- [AFRI2100](https://doi.org/10.1016/S0034-4257(01)00190-0): Aerosol Free Vegetation Index (2100 nm).
- [ARI](https://doi.org/10.1562/0031-8655(2001)074%3C0038:OPANEO%3E2.0.CO;2): Anthocyanin Reflectance Index.
- [ARVI](https://doi.org/10.1109/36.134076): Atmospherically Resistant Vegetation Index.
- [ATSAVI](https://doi.org/10.1016/0034-4257(91)90009-U): Adjusted Transformed Soil-Adjusted Vegetation Index.

### B

- [BCC](https://doi.org/10.1016/0034-4257(87)90088-5): Blue Chromatic Coordinate.
- [BGI](https://doi.org/10.1016/j.rse.2005.09.002): Blue Green pigment Index.
- [BNDVI](https://www.indexdatabase.de/db/i-single.php?id=135): Blue Normalized Difference Vegetation Index.
- [BWDRVI](https://doi.org/10.2135/cropsci2007.01.0031): Blue Wide Dynamic Range Vegetation Index.

### C

- [CCCI](https://doi.org/10.1016/j.fcr.2013.12.018): Canopy Chlorophyll Content Index
- [CIgreen](https://doi.org/10.1078/0176-1617-00887): Chlorophyll Index Green.
  - CIgreen740.560
  - CIgreen783.560
  - CIgreen865.560

- [CIred-edge](https://doi.org/10.1078/0176-1617-00887): Chlorophyll Index Red Edge.
  - CIred-edge740.705
  - CIred-edge783.705
  - CIred-edge865.705
 
- [CVI](https://www.cabdirect.org/cabdirect/abstract/20073176046): Chlorophyll Vegetation Index. 
  - CVI705
  - CVI783
  - CVI865
  
### D
- [Datt1](http://dx.doi.org/10.1071/BT98042): Datt1
- [Datt2](http://www.sciencedirect.com/science/article/pii/S092427161100089X): Simple Ratio 850/710 Datt2
- [Datt3](): Datt1
- [Datt4](): Datt1
- [DVI](https://doi.org/10.2307/1936256): Difference Vegetation Index.
- [DVIplus](https://doi.org/10.1016/j.rse.2019.03.028): Difference Vegetation Index Plus.

### E

- [EVI](https://doi.org/10.1016/S0034-4257(96)00112-5): Enhanced Vegetation Index.
   - EVI740
   - EVI783
   - EVI865
 
- [EVI2](https://doi.org/10.1016/j.rse.2008.06.006): Two-Band Enhanced Vegetation Index. 
- [ExG](https://doi.org/10.13031/2013.27838): Excess Green Index. 

### F

- [FCVI](https://doi.org/10.1016/j.rse.2020.111676): Fluorescence Correction Vegetation Index. 

### G

- [GARI](https://www.indexdatabase.de/db/i-single.php?id=363): Green Atmospherically Resistant Vegetation Index.
- [GBNDVI](https://www.indexdatabase.de/db/i-single.php?id=186): Green-Blue Normalized Difference Vegetation Index.
- [GCC](https://doi.org/10.1016/0034-4257(87)90088-5): Green Chromatic Coordinate.
- [GDVI](https://doi.org/10.3390/rs6021211): Generalized Difference Vegetation Index. 
- [GEMI](http://dx.doi.org/10.1007/bf00031911): Global Environment Monitoring Index.
- [GI](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.610.5657&rep=rep1&type=pdf): Greenness Index
- [GLI](http://dx.doi.org/10.1080/10106040108542184): Green Leaf Index. 
- [GNDVI](https://doi.org/10.1016/S0034-4257(96)00072-7): Green Normalized Difference Vegetation Index. 
   - GNDVI740.560
   - GNDVI865.560
- [GOSAVI](http://www.lib.ncsu.edu/resolver/1840.16/4200): Green Optimized Soil-Adjusted Vegetation Index
- [greenWDRVI]()
- [GRNDVI](https://www.indexdatabase.de/db/i-single.php?id=185): Green-Red Normalized Difference Vegetation Index.
- [GRVI]()
- [GVMI](https://doi.org/10.1016/S0034-4257(02)00037-8): Global Vegetation Moisture Index. 

### I

- [IRECI](https://doi.org/10.1016/j.isprsjprs.2013.04.007): Inverted Red-Edge Chlorophyll Index. 

### M

- [MCARI](http://dx.doi.org/10.1016/S0034-4257(00)00113-9): Modified Chlorophyll Absorption in Reflectance Index.
- [MCARI1](https://doi.org/10.1016/j.rse.2003.12.013): Modified Chlorophyll Absorption in Reflectance Index 1.
- [MCARI2](https://doi.org/10.1016/j.rse.2003.12.013): Modified Chlorophyll Absorption in Reflectance Index 2.
- [MCARI705](https://doi.org/10.1016/j.agrformet.2008.03.005): Modified Chlorophyll Absorption in Reflectance Index (705 and 750 nm).
- [MCARIOSAVI](https://doi.org/10.1016/S0034-4257(00)00113-9): MCARI/OSAVI Ratio.
- [MCARIOSAVI705](https://doi.org/10.1016/j.agrformet.2008.03.005): MCARI/OSAVI Ratio (705 and 750 nm). 
- [MGRVI](https://doi.org/10.1016/j.jag.2015.02.012): Modified Green Red Vegetation Index.  
- [MNDVI](https://doi.org/10.1080/014311697216810): Modified Normalized Difference Vegetation Index.
- [MNLI](https://doi.org/10.1109/TGRS.2003.812910): Modified Non-Linear Vegetation Index.
- [MSAVI](https://doi.org/10.1016/0034-4257(94)90134-1): Modified Soil-Adjusted Vegetation Index.
- [MSR](https://doi.org/10.1080/07038992.1996.10855178): Modified Simple Ratio.
- [MSR705](https://doi.org/10.1016/j.agrformet.2008.03.005): Modified Simple Ratio (705 and 750 nm).
- [MTCI](https://doi.org/10.1080/0143116042000274015): MERIS Terrestrial Chlorophyll Index.
- [MTVI1](https://doi.org/10.1016/j.rse.2003.12.013): Modified Triangular Vegetation Index 1.
- [MTVI2](https://doi.org/10.1016/j.rse.2003.12.013): Modified Triangular Vegetation Index 2.

### N

- [NDGI](https://doi.org/10.1016/j.rse.2019.03.028): Normalized Difference Greenness Index.
- [NDII](https://www.asprs.org/wp-content/uploads/pers/1983journal/jan/1983_jan_77-83.pdf): Normalized Difference Infrared Index.
- [NDMI](https://doi.org/10.1016/S0034-4257(01)00318-2): Normalized Difference Moisture Index.
- [NDPI](https://doi.org/10.1016/j.rse.2017.04.031): Normalized Difference Phenology Index.
- [NDREI](https://doi.org/10.1016/1011-1344(93)06963-4): Normalized Difference Red Edge Index.
- [NDVI](https://doi.org/10.1016/0034-4257(79)90013-0): Normalized Difference Vegetation Index.
- [NDVI705](https://doi.org/10.1016/S0176-1617(11)81633-0): Normalized Difference Vegetation Index (705 and 750 nm).
- [NDYI](https://doi.org/10.1016/j.rse.2016.06.016): Normalized Difference Yellowness Index.
- [NGRDI](https://doi.org/10.1016/0034-4257(79)90013-0): Normalized Green Red Difference Index.
- [NIRv](https://doi.org/10.1126/sciadv.1602244): Near-Infrared Reflectance of Vegetation.
- [NIRvH2](https://doi.org/10.1016/j.rse.2021.112723): Hyperspectral Near-Infrared Reflectance of Vegetation.
- [NIRvP](https://doi.org/10.1016/j.rse.2021.112763): Near-Infrared Reflectance of Vegetation and Incoming PAR.
- [NLI](https://doi.org/10.1080/02757259409532252): Non-Linear Vegetation Index.
- [NRFIg](https://doi.org/10.3390/rs13010105): Normalized Rapeseed Flowering Index Green.
- [NRFIr](https://doi.org/10.3390/rs13010105): Normalized Rapeseed Flowering Index Red.

### O

- [OCVI](http://dx.doi.org/10.1007/s11119-008-9075-z): Optimized Chlorophyll Vegetation Index.
- [OSAVI](https://doi.org/10.1016/0034-4257(95)00186-7): Optimized Soil-Adjusted Vegetation Index.

### R

- [RCC](https://doi.org/10.1016/0034-4257(87)90088-5): Red Chromatic Coordinate.
- [RDVI](https://doi.org/10.1016/0034-4257(94)00114-3): Renormalized Difference Vegetation Index.
- [REDSI](https://doi.org/10.3390/s18030868): Red-Edge Disease Stress Index.
- [RVI](https://doi.org/10.2134/agronj1968.00021962006000060016x): Ratio Vegetation Index.

### S

- [S2REP](https://doi.org/10.1016/j.isprsjprs.2013.04.007): Sentinel-2 Red-Edge Position.
- [SARVI](https://doi.org/10.1109/36.134076): Soil Adjusted and Atmospherically Resistant Vegetation Index.
- [SAVI](https://doi.org/10.1016/0034-4257(88)90106-X): Soil-Adjusted Vegetation Index.
- [SAVI2](https://doi.org/10.1080/01431169008955053): Soil-Adjusted Vegetation Index 2.
- [SeLI](https://doi.org/10.3390/s19040904): Sentinel-2 LAI Green Index.
- [SIPI](https://eurekamag.com/research/009/395/009395053.php): Structure Insensitive Pigment Index.
- [SR555](https://doi.org/10.1016/S0176-1617(11)81633-0): Simple Ratio (555 and 750 nm).
- [SR705](https://doi.org/10.1016/S0176-1617(11)81633-0): Simple Ratio (705 and 750 nm).

### T

- [TCARI](https://doi.org/10.1016/S0034-4257(02)00018-4): Transformed Chlorophyll Absorption in Reflectance Index.
- [TCARIOSAVI](https://doi.org/10.1016/S0034-4257(02)00018-4): TCARI/OSAVI Ratio.
- [TCARIOSAVI705](https://doi.org/10.1016/j.agrformet.2008.03.005): TCARI/OSAVI Ratio (705 and 750 nm).
- [TCI](http://dx.doi.org/10.1109/TGRS.2007.904836): Triangular Chlorophyll Index.
- [TGI](http://dx.doi.org/10.1016/j.jag.2012.07.020): Triangular Greenness Index.
- [TRRVI](https://doi.org/10.3390/rs12152359): Transformed Red Range Vegetation Index.
- [TSAVI](https://doi.org/10.1109/IGARSS.1989.576128): Transformed Soil-Adjusted Vegetation Index.
- [TTVI](https://doi.org/10.3390/rs12010016): Transformed Triangular Vegetation Index.
- [TVI](http://dx.doi.org/10.1016/S0034-4257(00)00197-8): Triangular Vegetation Index.

### V

- [VARI](https://doi.org/10.1016/S0034-4257(01)00289-9): Visible Atmospherically Resistant Index.
- [VARI700](https://doi.org/10.1016/S0034-4257(01)00289-9): Visible Atmospherically Resistant Index (700 nm).
- [VI700](https://doi.org/10.1016/S0034-4257(01)00289-9): Vegetation Index (700 nm).
- [VIG](https://doi.org/10.1016/S0034-4257(01)00289-9): Vegetation Index Green.

### W

- [WDRVI](https://doi.org/10.1078/0176-1617-01176): Wide Dynamic Range Vegetation Index.
- [WDVI](https://doi.org/10.1016/0034-4257(89)90076-X): Weighted Difference Vegetation Index.

## Burn 🔥

- [BAI](https://digital.csic.es/bitstream/10261/6426/1/Martin_Isabel_Serie_Geografica.pdf): Burned Area Index.
- [BAIS2](https://doi.org/10.3390/ecrs-2-05177): Burned Area Index for Sentinel 2.
- [CSIT](https://doi.org/10.1080/01431160600954704): Char Soil Index Thermal.
- [NBR](https://www.usgs.gov/core-science-systems/nli/landsat/landsat-normalized-burn-ratio): Normalized Burn Ratio.
- [NBR2](https://www.usgs.gov/core-science-systems/nli/landsat/landsat-normalized-burn-ratio-2): Normalized Burn Ratio 2.
- [NBRT](https://doi.org/10.1080/01431160600954704): Normalized Burn Ratio Thermal.
- [NDVIT](https://doi.org/10.1080/01431160600954704): Normalized Difference Vegetation Index Thermal.
- [SAVIT](https://doi.org/10.1080/01431160600954704): Soil-Adjusted Vegetation Index Thermal.

## Water 🌊

- [AWEInsh](https://doi.org/10.1016/j.rse.2013.08.029): Automated Water Extraction Index.
- [AWEIsh](https://doi.org/10.1016/j.rse.2013.08.029): Automated Water Extraction Index with Shadows Elimination.
- [MBWI](https://doi.org/10.1016/j.jag.2018.01.018): Multi-Band Water Index.
- [MNDWI](https://doi.org/10.1080/01431160600589179): Modified Normalized Difference Water Index.
- [NDVIMNDWI](https://doi.org/10.1007/978-3-662-45737-5_51): NDVI - MNDWI Model.
- [NDWI](https://doi.org/10.1080/01431169608948714): Normalized Difference Water Index.
- [NWI](https://doi.org/10.11873/j.issn.1004-0323.2009.2.167): New Water Index.
- [WI1](https://doi.org/10.3390/rs11182186): Water Index 1.
- [WI2](https://doi.org/10.3390/rs11182186): Water Index 2.
- [WRI](https://doi.org/10.1109/GEOINFORMATICS.2010.5567762): Water Ratio Index.

## Drought 🏜️

- [NDDI](https://doi.org/10.1029/2006GL029127): Normalized Difference Drought Index.
- [NMDI](https://doi.org/10.1029/2007GL031021): Normalized Multi‐band Drought Index.


# List

Check the full list of spectral indices with their formulas [here](https://github.com/MCroci/agr-spectral-indices/blob/master/Output/).

# Download Raw Files

You can download or clone the repository:

```
git clone https://github.com/MCroci/spectral-indices.git
```

Or you can download the single files here (right-click > Save link as...):
- CSV: [Raw list](https://github.com/MCroci/agr-spectral-indices/blob/master/Output/Spectral%20Vegetation%20Indices.csv)
