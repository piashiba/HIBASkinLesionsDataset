# Hospital Italiano de Buenos Aires Skin Lesions Dataset
This repository hosts the Python script to perform the Exploratory Data Analysis (EDA) of the Hospital Italiano de Buenos Aires skin lesion dataset shared through the ISIC Archive. 

## Dataset description


## Access to the image collection 
The dataset is registered as a collection in the ISIC Archive. In this sense, it can be downloaded in two ways:

(1) By visiting the ISIC Archive website or accessing the collection DOI https://doi.org/10.34970/432362.
![image](https://user-images.githubusercontent.com/74262815/233081137-d1403678-59ae-4bb3-8f8c-a25a03f75611.png)

(2) By resorting to the official command line tool for interacting with the ISIC Archive (for more information visit https://github.com/ImageMarkup/isic-cli)

```
# Install tool 
pip install isic-cli 

# Find the collection ID
isic collection list # Hospital Italiano de Buenos Aires Skin Lesions (ID 176)

# Download the collection metadata
isic metadata download --collections 176

# Download the collection metadata
isic metadata download --collections 176

# Download the collection images (and save them on 'images/' folder)
isic image download --collections 176 images/
```
