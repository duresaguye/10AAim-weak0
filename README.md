Solar Farm Data Analysis
Overview

The aim of this analysis is to uncover key insights from the solar radiation data for the regions of Benin, Sierra Leone, and Togo. By identifying trends and patterns in solar irradiance, wind conditions, temperature variations, and sensor data quality, the analysis will guide MoonLight Energy Solutions in determining high-potential regions for solar installations that align with the company's sustainability goals.. The results are presented through an interactive Streamlit dashboard https://mainpy-dp4otqcupvpauesq3grhie.streamlit.app/ , making it easy to explore the data and findings.
Project Structure

The repository is organized as follows:

   

    app/main.py: The main script for the Streamlit application. This script loads the data, performs analysis, and renders the interactive dashboard.

    requirements.txt: Lists the Python dependencies required to run the project, including libraries such as pandas, numpy, matplotlib, seaborn, scipy, and streamlit.

    README.md: Provides an overview of the project, setup instructions, and details about the Streamlit dashboard.

Streamlit Dashboard

Streamlit is an open-source app framework for creating data-driven web applications in Python. In this project, we use Streamlit to create an interactive dashboard that allows users to explore the solar farm data. The dashboard includes several features:

   Data Previews: Display the first few rows of the datasets for Benin, Sierra Leone, and Togo.
    Summary Statistics: Show descriptive statistics for the datasets, including measures of central tendency and variability.
    Missing Values: Identify and display the number of missing values in each dataset.
    Outlier Detection: Detect and display outliers in the Global Horizontal Irradiance (GHI) values using the Z-score method.
    Visualizations:
        Time Series Plots: Visualize the temporal patterns of GHI.
        Correlation Heatmaps: Explore the relationships between solar parameters like GHI, DNI, and DHI.
        Wind Polar Plots: Display the distribution of wind speed and direction.
        Histograms: Analyze the distribution of GHI values.

The Streamlit dashboard is designed to be user-friendly, allowing users to interact with the data and gain insights without needing to write code.
Setup Instructions

To run this project locally, follow these steps:

    Clone the Repository:

   https://github.com/duresaguye/Solar_farm_radiation_measurment_data_analysis
  

Install Dependencies

Create a virtual environment and install the required packages:

python -m venv myenv source myenv/bin/activate # On Windows, use myenv\Scripts\activate pip install -r requirements.txt
Run the Streamlit App

Launch the Streamlit dashboard:

streamlit run app/main.py

