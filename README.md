# Earthquake Risk Analysis (Team Project)

This repository is a fork of a team project focused on analyzing earthquake data and predicting seismic risk in North America. I maintain this fork to showcase my individual contributions across **machine learning, data processing and application integration.

## My Contributions
- Performed data preprocessing and feature engineering on large-scale earthquake datasets (USGS)
- Built and evaluated machine learning models for magnitude prediction (Random Forest, XGBoost, LightGBM) using RMSE and R²
- Assisted in integrating trained ML models into the Streamlit application for interactive analysis and predictions
- Contributed to visualization components (heatmaps, risk insights) and end-to-end testing of the application

**Key Results**
- Achieved RMSE ≈ 4–5 and R² ≈ 0.5 for earthquake magnitude prediction
- Delivered a fully functional interactive web application for earthquake risk analysis

## Features

- Interactive heatmap of earthquake activity
- Zipcode-based risk assessment
- Machine learning model for magnitude prediction
- Insights and statistical analysis

## Deployment Instructions

### Local Deployment

1. Ensure Python 3.8+ is installed
2. Clone this repository
3. Run setup.bat (Windows) or setup.sh (Linux/Mac) to ensure data files are in the correct location
4. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
5. Run the application:
   ```
   streamlit run app.py
   ```

### Streamlit Cloud Deployment

1. Push this repository to GitHub
2. Connect to Streamlit Cloud (https://streamlit.io/cloud)
3. Deploy your app by pointing to the GitHub repository
4. Ensure the data file (`earthquake_cleandata_posteda.csv`) is in the `src` directory
5. The app should automatically use the setup scripts during deployment

## Troubleshooting

If you encounter "Data file not found" errors:
1. Make sure `earthquake_cleandata_posteda.csv` is in the `src` directory
2. If using Streamlit Cloud, check that the file is properly pushed to your GitHub repository
3. You can always upload your own CSV file through the application interface

## Data Format

The application expects a CSV file with the following columns:
- LATITUDE: decimal degrees
- LONGITUDE: decimal degrees
- MAGNITUDE: earthquake magnitude
- DATE: date/time of the earthquake
- Other columns like DEPTH, PLACE, etc. are optional but enhance functionality

## Technologies Used

- Python
- Streamlit
- Pandas
- Scikit-learn (Random Forest & Gradient Boosting)
- Plotly
- GeoPy

## Contributors

- Naveen Manikandan 
- Karthik Manjunath
- Hariharan Nadanasabapathi
