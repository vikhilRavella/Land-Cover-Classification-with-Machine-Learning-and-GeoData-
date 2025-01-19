# Land Cover Classification with Machine Learning and GeoData

## Project Overview
This project focuses on classifying land cover types (such as water, forest, urban areas, etc.) in the Chilkur region using Sentinel-2 satellite imagery. The classification is achieved through a machine learning approach, specifically a Random Forest classifier, applied in the Google Earth Engine (GEE) platform.

## Institution/Organization
Indian Institute of Remote Sensing

## Date
23/08/2023

## Objectives
- Classify land cover types using Sentinel-2 imagery.
- Utilize the Random Forest machine learning algorithm for classification.
- Evaluate and report the model’s performance based on accuracy metrics.
- Visualize the results on a map and export the classified data.

## Google Earth Engine Script
The complete Google Earth Engine script used for land cover classification is available in the script below or via the link:

[Land Cover Classification Script on Google Earth Engine](https://code.earthengine.google.com/c5b4cb17eaf236a9bf79caeac2fc0647)

### Script Summary
- **Data Collection**: Sentinel-2 imagery for the year 2023 (from January 1, 2023, to December 31, 2023).
- **Preprocessing**: Image filtering based on date and region of interest (ROI), followed by the calculation of the Normalized Difference Vegetation Index (NDVI).
- **Model Training**: A Random Forest classifier trained on labeled land cover data.
- **Results**: A classified land cover map with an evaluation of training and validation accuracies.

## Methodology
1. **Data Collection**:
   - Sentinel-2 imagery is selected for the region of interest (Chilkur), filtered by date range (2023), and selected bands (B2, B3, B4, B8).
   
2. **Preprocessing**:
   - NDVI is calculated using the bands B8 (Near Infrared) and B4 (Red).
   
3. **Model Training**:
   - Labeled training data (Water, Forest, Urban) are used to train the Random Forest classifier.
   
4. **Model Evaluation**:
   - Accuracy is evaluated using both training and validation datasets.
   - A confusion matrix is used to assess the classifier's performance.

## Data
- **Sentinel-2 imagery** from Google Earth Engine.
- **Training data**: Includes land cover types (Water, Forest, Urban).
- **Exported results**: Classifications in both asset and shapefile formats.

## Results
- The classifier provides a categorized map of the land cover types in the Chilkur region.
- The model achieved a **training accuracy** of 1.0 and **validation accuracy** of 0.5 (based on the confusion matrix).

## Instructions for Use
To run this project and replicate the results, follow these steps:
1. Visit [Google Earth Engine](https://code.earthengine.google.com/).
2. Import the script using the link provided above.
3. Modify the region of interest (ROI) or data as needed.
4. Execute the script to classify land cover and view the results.
5. Export the results if needed as shapefiles or other formats.

## Files in this Repository
- `README.md` – Project description and documentation.
- `scripts/` – Folder containing the Google Earth Engine scripts (e.g., `land_cover_classification.js`).
- `data/` – Folder containing training data (shapefiles, geojson, etc.).
- `results/` – Folder containing output files (classified maps, confusion matrix, etc.).

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments
- Indian Institute of Remote Sensing (IIRS) for providing valuable resources for the project.
- Google Earth Engine for providing the platform and satellite data.
- Sentinel-2 for providing free access to high-resolution satellite imagery.

## Contact Information
For any questions or feedback, feel free to reach out:
- **Name**: Ravella Vikhil
- **Email**: ravellavikhil9999@gmail.com
