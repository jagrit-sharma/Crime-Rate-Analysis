# U.S. Crime Data Analysis Project

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Techniques Used](#techniques-used)
- [Key Findings](#key-findings)
- [Installation Steps](#installation-steps)
- [Files in the Repository](#files-in-the-repository)
- [Results](#results)
- [Limitations](#limitations)
- [Future Work](#future-work)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Overview

This project analyzes crime data across U.S. cities to identify trends, high-risk areas, and factors related to victims and criminals. The analysis uses various machine learning techniques to process and interpret a comprehensive dataset of U.S. crimes.

## Dataset

The analysis uses the "U.S. Crime Dataset" from Kaggle, which includes information about various crimes across different states in the United States. The dataset provides details such as:

- Type of crime
  - Part 1-2 (Crime Classification)
  - Crm Cd (Crime Code)
  - Crm Cd Desc (Crime Code Description)
  - Crm Cd 1, Crm Cd 2, Crm Cd 3, Crm Cd 4 (Additional Crime Codes)

- Location
  - AREA NAME
  - Rpt Dist No (Reporting District Number)
  - LOCATION
  - Cross Street
  - LAT (Latitude)
  - LON (Longitude)

- Date
    - DATE RPTD (Date Reported)
    - DATE OCC (Date of Occurrence)
    - TIME OCC (Time of Occurrence)

- Other relevant factors
  - Mocodes (Modus Operandi Codes)
  - Vict Age (Victim Age)
  - Vict Sex (Victim Sex)
  - Vict Descent (Victim Descent)
  - Premis Cd (Premise Code)
  - Premis Desc (Premise Description)
  - Weapon Used Cd (Weapon Used Code)
  - Weapon Desc (Weapon Description)
  - Status
  - Status Desc (Status Description)

Dataset source: [U.S. Crime Dataset on Kaggle](https://www.kaggle.com/datasets/arpitsinghaiml/u-s-crime-dataset)

## Techniques Used

1. K-means Clustering
2. Linear Regression
3. Decision Trees
4. Principal Component Analysis (PCA)
5. Map-Reduce

## Key Findings

- Spatial patterns in crime distribution across different areas
- Importance of various features in predicting crime locations
- Classification of crimes into Part 1 and Part 2 categories
- Dimensionality reduction for visualizing complex crime data
- Area-specific crime patterns and distributions

## Installation Steps

1. **Clone the Repository**  
   First, clone the repository to your local machine:

   ```bash
   git clone https://github.com/jagrit-sharma/Crime-Rate-Analysis.git
   cd Crime-Rate-Analysis
   ```
2.	**Create a Virtual Environment (Optional but recommended)**
    
    It’s recommended to create a virtual environment to manage dependencies for your project:

	•	For Windows:

    ```bash
    python -m venv venv
    venv\Scripts\activate
    ```

	•	For macOS/Linux:

    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```

3.	**Install Dependencies**
    
    Install the required dependencies by running the following command:

    ```bash
    pip install -r requirements.txt
    ```
	
4.	**Run the Code**

    Once the environment is set up, and dependencies are installed, you can run the Jupyter Notebook.

    ```bash
    python CrimeRate_Analysis.ipynb
    ```

5.	**Output Plots**

    The code generates several plots and stores them in folders under Plots. These include:
    - EDA Plots
    - KMeans Plots
    - LR Plots
    - DT Plots
    - PCA Plots

    You can view these plots after running the code.

## Files in the Repository

The repository contains the following main files and directories:

```
Crime-Rate-Analysis/
├── CrimeRate_Analysis.ipynb  # Jupyter Notebook with the analysis code
├── Plots/
│   ├── EDA_plots/                   # Folder containing exploratory data analysis plots
│   ├── KMeans_plots/               # Folder containing K-means clustering plots
│   ├── LR_plots/            # Folder containing linear regression plots
│   ├── DT_plots/                      # Folder containing decision tree plots
│   └── PCA_plots/                      # Folder containing PCA plots
├── requirements.txt              # List of dependencies required for the project
└── README.md                     # Project overview and instructions
```

## Results

The project provides insights into:

- Crime hotspots and high-risk areas
- Factors influencing crime occurrences
- Patterns in crime types across different locations
- Potential strategies for law enforcement resource allocation

## Limitations

- The analysis is based on available data and may not capture all factors influencing crime
- Some techniques assume linear relationships which may not always hold true for complex crime data
- The project focuses on specific aspects of crime and may not provide a comprehensive view of all crime-related issues

## Future Work

- Incorporate temporal analysis to understand crime trends over time
- Include additional contextual factors such as population density and socioeconomic indicators
- Explore more advanced machine learning techniques for improved predictions

## License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/jagrit-sharma/Crime-Rate-Analysis/blob/main/LICENSE) file for details.

## Acknowledgments

- Kaggle for providing the U.S. Crime Dataset