Data and code for Torrente, F., Yoris, A., Low, D., Lopez, P., Bekinschtein, P., Vázquez, G. H., ... & Cetkovich, M. (2022). Psychological symptoms, mental fatigue and behavioural adherence after 72 continuous days of strict lockdown during the COVID-19 pandemic in Argentina. BJPsych open, 8(1).


## 1. Data

Available at `./data/input/`

* `Emotional symptoms COVID19_Arg_May20_v2_text.csv` Main Dataset
* `covid-stringency-index.csv` For Figure 1 (obtained from https://ourworldindata.org/grapher/covid-stringency-index)

* `population-by-country_worldbank.csv` used to select certain countries to plot in Figure 1

Available at https://www.google.com/covid19/mobility/

* `Global_Mobility_Report.csv` For supplementary Figure S1 


## 2. Reproduce

**Google Colab**

The `.ipynb` can run on Google Colab (for which data should be on Google Drive; code to load data from Google Drive is available in scripts)
You can install packages with `!pip install <package-name>`


**Jupyter Notebook**

To run the `.ipynb` on Jupyter Notebook, open terminal, create a virtual environment and install the `requirements.txt`:

```
conda create --name covid_argentina --file requirements.txt
conda activate covid_argentina
```

Go to directory where you want to put this repo:

```
cd ./path/to/
git clone https://github.com/danielmlow/extract_opensmile.git
cd ./path/to/covid19_argentina/
```


**Scripts**

Contextual analysis: Figure 1, Table S1, Figure S1:
```
jupyter notebook stringency_mobility.ipynb
```


Regression analysis: Table 5:
```
jupyter notebook regression.ipynb
```












