# Surveillance Dashboard
Code for a Python-based Shiny dashboard exploring relationship between LDAS hydrometeorological records and malaria case rates at different lag times and across different geographies.

## Conda recipe

```conda
conda create --name arcccoh_shiny python=3.9.18 -y
activate arcccoh_shiny 
conda install -c esri arcgis=2.2.0.1 -y
jupyter nbextension enable arcgis --py --sys-prefix
conda.exe install -c esri scipy -y
pip install geopandas
conda install -c esri ipyleaflet -y
conda install -c bioconda epiweeks -y
conda install -c esri mapclassify -y
conda install -c esri folium
conda install -c conda-forge shiny -y
pip install shinylive
pip install shinywidgets
pip install rsconnect-python
```

---

## Serving the dashboard

* Open the Python command prompt
* Navigate to the repository folder
* Export the app via ShinyLive to the docs folder:  
  `shinylive export data docs`
* View the app locally:  
  `python -m http.server --directory docs --bind localhost 8008`  
  Then open the browser locally - [link](http://localhost:8008)
* If the app.json file exceeds 100mb, enable Git LFS:
  * Open the repo in the Git bash shell
  * Type the command `git lfs track docs/app.json`
  * Commit the file
  * Push the file
* Enable pages on GitHub

