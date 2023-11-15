# Wildfire Prediction and Burned Scars Segmentation System
This project aims to establish a comprehensive system for predicting wildfires and segmenting burned areas using various data collection, visualization, and advanced modeling techniques.

# Objective
The main objective of this project is to provide a platform capable of predicting wildfires while identifying and segmenting areas affected by fires, potentially serving as a tool for natural disaster management and prevention.

# Project Contents :
## 1. Data Collection
The data collection process involved initial data containing various details about each wildfire. We refined this data to include essential columns: wildfire start date, burned area in hectares, latitude, and longitude.
Using geographical coordinates (latitude and longitude), we collected satellite images via the Mapbox API. These images covered areas affected by wildfires and specific non-affected urban zones.
The collected images were prepared, cleaned, and split into training and validation sets. Our final dataset comprised 22,710 "wildfire" class images (representing 53% of the total) and 20,140 "non-wildfire" class images (representing 47% of the total). This balanced distribution will aid in training a robust model capable of accurately predicting both classes.

## 2. Data Visualization
Data visualization played a pivotal role in comprehending the complex patterns and trends within our wildfire dataset. Leveraging Python libraries such as Matplotlib, Seaborn, and Plotly, we conducted an in-depth exploratory analysis.

## 3. Wildfire Prediction model
The Wildfire Prediction Model is a Convolutional Neural Network (CNN) meticulously trained on satellite imagery. This model serves the critical function of discerning the susceptibility of specific locations to wildfires, leveraging intricate patterns and features extracted from the imagery.

## 4. Burned Scars Segmentation Model
The Burned Scars Segmentation Model utilizes the SegNet architecture and annotated satellite imagery to generate precise masks highlighting areas affected by burn scars within satellite images. 

## 5. Streamlit Application 
The Streamlit app offers two interfaces: one for the Wildfire Prediction Model allowing instant risk assessment based on geographical coordinates or uploaded satellite images, and another for the Burned Scars Segmentation Model that generates precise masks highlighting areas affected by burn scars within uploaded satellite images.
