# NCS-1MLProject Scraping and Machine Learning

`scrape_vars.ipynb` is the Jupyter notebook for scraping the variables from the DS1 code book.  In addition to creating a Mongo DB, 
the notebook creates 3 temporary files: `variables.csv`, `titles.csv`, `variables.json`.  The last file contains the same variable
maps that are stored in the Mongo DB.  `scrape4.ipynb` is the scraping from the DS2 code book.

`sort_variables.ipynb` is the Jupyter notebook that attempts to classify each variable based on the results of the scraping by looking
at the values of each label found.  It then attempts to convert the entire dataset.

There are various `.json` files that include temporary workfiles for sorting and scraping variables.  Saving the intermediate work allows
one to start over at a point other than the beginning.

`r-joined.csv` is the joined .csv file of the DS1 and DS2 data sets.

`coding-variables.ipynb` is the Jupyter notebook for converting variable's integer-coded values to their
descriptive values.

`reduced-data2.csv` is the subset of the data used for fitting our models.

`morefitting.ipynb` is the Jupyter notebook with the Lasso Logistic Regression.  Adjusting the threshold to 
acheive the desired recall is done at the end of the notebook.

