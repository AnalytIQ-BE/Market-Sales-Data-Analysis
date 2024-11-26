## Market Sales Dataset

### Overview
The "Market Sales Dataset" is a comprehensive collection of sales data that includes various features such as product categories, sales figures, timestamps, and more. This dataset is ideal for performing data analysis to uncover trends and insights in market sales.

### Dataset Details
- **Source**: Kaggle
- **File Format**: ZIP
- **Contents**: The ZIP file contains multiple CSV files, each representing different aspects of market sales data.

### Folder Structure
The dataset is stored in the `data` folder of this project. Upon extraction, the folder structure is as follows:

data/ └── market-sales-data/ ├── supermarket_sales new.csv 

└── README.md

### Usage
To use the dataset, follow these steps:
1. **Download the ZIP file**: The dataset can be downloaded from Kaggle using the provided script.
2. **Extract the ZIP file**: Unzip the downloaded file into the `data` folder.
3. **Load the data**: Use pandas or any other data manipulation library to load the CSV files for analysis.

### Example Code
Here is an example of how to download and extract the dataset using the Kaggle API:

```python
import os
from kaggle.api.kaggle_api_extended import KaggleApi
```
# Initialize the Kaggle API
```
api = KaggleApi()
api.authenticate()
```
# Specify the dataset and the download path
```
dataset = "willianoliveiragibin/market-sales-data"
download_path = "data/market-sales-data"
```
# Create the download path if it doesn't exist
```
os.makedirs(download_path, exist_ok=True)
```
# Download and unzip the dataset
```
api.dataset_download_files(dataset, path=download_path, unzip=True)

print(f"Path to dataset files: {download_path}")
```
## Notes
Ensure you have the necessary permissions and API tokens configured to access the dataset from Kaggle.
The dataset is intended for educational and research purposes.
By following the steps above, you can easily integrate the “Market Sales Dataset” into your data analysis workflow. Happy analyzing!


