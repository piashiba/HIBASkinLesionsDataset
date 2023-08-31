# Hospital Italiano de Buenos Aires Skin Lesions Images (2019-2022) Dataset
This repository hosts the Python script to perform the Exploratory Data Analysis (EDA) of the Hospital Italiano de Buenos Aires skin lesion dataset shared through the ISIC Archive. This project was conducted by the Dermatology Department and the Artificial Intelligence and Data Science program of the Health Informatics Department of the institution.

## Dataset description
The dataset described here was composed of information collected from 628 patients seen by expert dermatologists at the Hospital Italiano de Buenos Aires (Buenos Aires, Argentina). The collection comprises 1,635 images (1,280 contact-polarized dermoscopy images and 355 clinical images) captured from 1,257 lesions corresponding to the most frequent diagnoses observed at the institution. 

![image](https://user-images.githubusercontent.com/74262815/233088432-2bcff90a-e104-4312-81ba-caf84c93fe7d.png)


## Access to the image collection 
The dataset is registered as a collection in the ISIC Archive. In this sense, it can be downloaded in two ways:

1. By visiting the ISIC Archive website or accessing the collection DOI https://doi.org/10.34970/432362.
![image](https://user-images.githubusercontent.com/74262815/233081137-d1403678-59ae-4bb3-8f8c-a25a03f75611.png)

2. By resorting to the official command line tool for interacting with the ISIC Archive (for more information visit https://github.com/ImageMarkup/isic-cli)

```
# Install tool 
pip install isic-cli 

# Find the collection ID
isic collection list # Hospital Italiano de Buenos Aires Skin Lesions (ID 176)

# Download the collection metadata
isic metadata download --collections 176

# Download the collection metadata
isic metadata download --collections 176

# Download the collection images (and save them in the 'images/' folder).
isic image download --collections 176 images/
```
## Exploratory Data Analysis (EDA)
In this [Python notebook](ExploratoryDataAnalysis.ipynb) we performed the download of the collection from the ISIC Archive by resorting to the command line tool, and carried out the exploratory data analysis (EDA). In this regard, we evaluated the distribution of patients, lesions and images, as well as analyzed the characteristics of patients (age, sex, personal and family history of melanoma) and lesions (diagnosis, type of confirmation for diagnosis, location).

## Datasets Comparison
In this [Python notebook](DatasetsComparison.ipynb) we performed a comparison between the dataset presented here and publicly available datasets.
