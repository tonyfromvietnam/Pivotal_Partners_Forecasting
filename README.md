
# Final Year Project: Forecasting Stock Volatility Using Machine Learning and Hybrid GARCH-Deep Learning Models

## Overview
This project explores the effectiveness of different modelling techniques in forecasting the volatility of the TOPIX-1000 stock index using daily, weekly, and monthly return data. The models implemented include:
- GARCH-family models (GARCH(1,1), GARCH(1,2), GARCH(2,1), GARCH(2,2))
- Light Gradient Boosting Machine (LightGBM)
- Gated Recurrent Unit (GRU)
- Hybrid GARCH-GRU model

The project is designed to support decision-making for different investment horizons by evaluating the performance of each model on various frequencies.

## Project Structure
- `Final_Year_Project.ipynb`: Main Jupyter notebook implementing the forecasting models.
- `requirements.txt`: List of required Python packages.
- `TOPIX1000.json.bz2`: The dataset for this project, containing daily return data of the TOPIX-1000 index used for multi-frequency volatility forecasting.

## Dependencies
To run the notebook, install the dependencies using:
```bash
pip install -r requirements.txt
```

## Instructions to Run
1. Launch Google Colab and upload the dataset to Google Drive.
2. Open `Final_Year_Project.ipynb`.
3. Run all cells in order to reproduce the results and visualisations.
4. Forecasts are generated using the trained models for 12 months/weeks/days ahead based on the dataset.

## Data
The dataset used is the TOPIX-1000 index, covering the period from January 2009 to January 2023. Data is preprocessed into daily, weekly, and monthly return formats.

## Notes
- The notebook uses the `Nixtla` forecasting libraries (StatsForecast and NeuralForecast).
- If a model fails to run, please verify you are using a compatible Python version (Python 3.8+ recommended).
- Results may be slightly different on other systems if random seed settings are not enforced.

## Acknowledgements
This project was supervised by Dr. Yongxin Yang and uses public data and open-source Python packages.
