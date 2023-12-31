# NCALM_raster_analysis

Repo for all the NCALM raster analysis scripts
* processing lidar, create clean netcdfs of data, visualizing the data, performing random forest analysis 

created by Cassie Lumbrazo\
July 2023 





---
### **\lidar_analysis** directory 
---

*Clean the lidar data and create tidy netcdfs from raster (tifs)*
**\CER_model_create_netcdf.ipynb**
- creates final cleaned netcdf file: *cer_model_cleandata_create_netcdf.nc* 

**\SR_model_create_netcdf.ipynb**
- creates final cleaned netcdf file: *sr_model_cleandata_create_netcdf.nc* 

**\FL_model_create_netcdf.ipynb**
- creates final cleaned netcdf file: *fl_model_cleandata_create_netcdf.nc* 


*Visualizing the lidar data* 
**\CER_model_plots.ipynb**
- creates a final figure in WADNR report 

**\SR_model_plots.ipynb**
- creates a final figure in WADNR report 

**\FL_model_plots.ipynb**
- creates a final figure in WADNR report 

**\AllSites_plots.ipynb**
- creates a final figure in WADNR report 

*xDEM analysis* 
**\CER_xdem.ipynb**
**\FL_xdem.ipynb**
- creates a final figure in WADNR report 


---
### **\random_forest** directory 
---

**\AllSites_RandomForest_1.ipynb**
- runs random forest with all data to produce PDP plot of elevation

**\AllSites_RandomForest_2.ipynb**
- runs random forest with full elevation bins (not final bins)

**\AllSites_RandomForest_3.ipynb**
- runs random forest with reduced (and final) elevation bins

**\AllSites_RandomForest_4.ipynb**
- produces snow depth direction plots from the Random Forest #3 notebook

**\AllSites_RandomForest_5.ipynb**
- changes the coloring convention of the plots from the Random Forest #4 notebook 

**\AllSites_RandomForest_6.ipynb**
- changes the decision tree order convention of the plots from the Random Forest #5 notebook
- creates final random forest figures, snow depth and feature PDFs

---
### **\data** directory 
---
These datasets are large and not stored on github. I will update this with a link to the data.

The datasets required to run the scrips in this repo include,

*a few final datasets with all the rasters combined into a single netcdf*
- cer_model_cleandata_create_netcdf.nc
-  fl_model_cleandata_create_netcdf.nc
-  sr_model_cleandata_create_netcdf.nc

*and a few pickle python instances saved to make moving between notebooks easier...*
-  all_sites_snowdepth_dem_dah_tpi_dce.pkl
-  randomforest_bin1_1000.pkl
-  randomforest_bin2_1000.pkl
-  randomforest_bin3_1000.pkl

