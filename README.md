# Covid-19-Patient-Health-Analytics

An exploratory machine learning project for predicting recorded outcomes of COVID-19 patients and comparing models.

[Repository](https://github.com/MirzaAlbab/Covid-19-Patient-Health-Analytics)

## Features

- Patient outcome prediction notebook
- Separate model-comparison notebook
- Training and test data plus an output CSV

## Technology

Python and Jupyter / Google Colab; see notebook imports for the required libraries.

## Data and notebooks

| Path | Purpose |
| --- | --- |
| `Covid_19_Patient_Health_Prediction.ipynb` | Patient outcome prediction workflow |
| `COVID_19_Model_Comparison.ipynb` | Model comparison |
| `cvd/data.csv` | Original dataset copy |
| `cvd/train.csv` | Training data with outcome columns |
| `cvd/test.xlsx` | Test data without outcome columns |
| `final.csv` | Previously generated results |

Original dataset source: [Novel Coronavirus 2019 Dataset on Kaggle](https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset). Respect the dataset's own terms and attribution.

## Getting started

```bash
git clone https://github.com/MirzaAlbab/Covid-19-Patient-Health-Analytics.git
cd Covid-19-Patient-Health-Analytics
```

Open the notebooks in Google Colab or Jupyter. The original workflow places `cvd/` in Google Drive, mounts Drive from Colab, and runs `Covid_19_Patient_Health_Prediction.ipynb`. Update notebook paths for your own Drive location or local checkout and install libraries required by the imports.

## Development and checks

Run the notebooks from a fresh kernel. Use held-out evaluation and report class balance, preprocessing, and metrics when comparing models; no performance result is claimed here.

## Project structure

- `cvd/` — Dataset files

## Project notes

The original project describes a boosted Random Forest classifier. Model quality and clinical suitability have not been established by this README.

## Original documentation

<details>
<summary>Preserved original README and credits</summary>

# Covid-19-Patient-Health-Analytics
A Boosted Random Forest Classification model was implemented to predict the outcome of the CoV-2 positive patients in China. Based on multiple features.

The original dataset was taken from: https://www.kaggle.com/sudalairajkumar/novel-corona-virus-2019-dataset

cvd
  + data.csv -> original dataset
  + train.csv -> training dataset (contains data for 'death' and 'recovered' columns)
  + test.xlsx -> test dataset (does not contains data for 'death' and 'recovered' columns)

final.csv -> result obtained by running the model on test.xlsx

Steps to reproduce results:

1) Place the 'cvd' directory in your Google Drive.
2) Connect the Colab Notebook to Google Drive.
3) Run the 'Covid-19 Patient Health Prediction.ipynb' file.

</details>

## License

See [LICENSE](LICENSE). Third-party libraries, datasets, and assets may have separate terms.
