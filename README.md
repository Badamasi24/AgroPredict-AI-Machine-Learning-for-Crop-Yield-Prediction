# 🌱 AgroPredict AI: Machine Learning for Crop Yield Prediction

**AgroPredict AI** is a machine learning project focused on predicting agricultural crop yields using data science and artificial intelligence.

The project explores how agricultural data, environmental conditions, soil characteristics, and farming practices can be used to estimate crop yields and support better farming decisions.

My long-term vision is to develop an intelligent agricultural decision-support system that contributes to **precision farming in Zamfara State and Nigeria at large.**

> **Project Status:** Initial model development and evaluation completed. Data enrichment, local validation, and model improvement are ongoing.

---

## 🎯 Project Objectives

- Develop machine learning models for agricultural crop yield prediction.
- Investigate the relationship between environmental conditions, soil characteristics, farming practices, and crop yields.
- Identify important factors associated with agricultural productivity.
- Improve prediction performance using reliable agricultural and locally relevant datasets.
- Build a decision-support system that can help farmers make more informed agricultural decisions.

## 📊 Dataset

The initial development uses the [Agriculture Crop Yield Dataset from Kaggle](https://www.kaggle.com/datasets/samuelotiattakorah/agriculture-crop-yield).

The dataset contains agricultural observations covering six crop types:

- Maize
- Rice
- Wheat
- Barley
- Soybean
- Cotton

### Dataset Features

| Feature | Description |
|---|---|
| Region | Agricultural region |
| Soil_Type | Soil classification |
| Crop | Type of crop cultivated |
| Rainfall_mm | Rainfall measurement in millimetres |
| Temperature_Celsius | Temperature in Celsius |
| Fertilizer_Used | Whether fertilizer was used |
| Irrigation_Used | Whether irrigation was used |
| Weather_Condition | Weather condition |
| Days_to_Harvest | Number of days to harvest |
| Yield_tons_per_hectare | Target variable |

**Important data note:** The downloaded dataset contains 89,810 records, although the Kaggle description advertises 1,000,000 samples. Its provenance and suitability for real-world agricultural applications still require further verification. The initial results should therefore be interpreted as experimental model performance, not validated farm-level predictions.

## 🔍 Project Workflow

The project follows a structured machine learning workflow:

1. **Data Collection:** Downloading and loading the agricultural dataset.
2. **Data Cleaning:** Identifying missing values, invalid yield observations, and duplicate records.
3. **Exploratory Data Analysis (EDA):** Examining distributions, relationships, and patterns in agricultural variables.
4. **Feature Analysis:** Investigating relationships between rainfall, temperature, soil type, fertilizer use, irrigation, and yield.
5. **Model Development:** Training Linear Regression and Random Forest models.
6. **Model Evaluation:** Comparing models using MAE, RMSE, and R².
7. **Prediction:** Developing an interface for entering agricultural conditions and generating yield estimates.

## 📈 Exploratory Data Analysis

Some of the initial findings include:

- Rainfall showed a strong positive correlation with crop yield in the dataset.
- Temperature had a relatively weak linear correlation with yield.
- Fertilizer use and irrigation were associated with higher average yields.
- Crop yield distribution was approximately symmetric.
- Yield differences across the six crop types were relatively small.

These findings describe patterns in the dataset and should not be interpreted as proof of causal relationships or universal agronomic recommendations.

## 🤖 Machine Learning Models

Two regression algorithms were developed and evaluated:

1. Linear Regression
2. Random Forest Regressor

### Model Evaluation Results

| Evaluation Metric | Linear Regression | Random Forest |
|---|---:|---:|
| MAE | **0.398** | 0.413 |
| RMSE | **0.497** | 0.517 |
| R² Score | **91.42%** | 90.74% |

### Interpretation

**Linear Regression** currently performs slightly better than Random Forest on the test dataset.

Its evaluation results indicate:

- Mean Absolute Error of approximately 0.398 tons/hectare.
- Root Mean Squared Error of approximately 0.497 tons/hectare.
- R² score of approximately 91.42%.

Based on the current evaluation, Linear Regression is selected as the baseline model for further investigation.

These results are preliminary and will be subjected to additional validation, including cross-validation and further error analysis.

## 🛠️ Technologies and Tools

- **Python:** Data analysis and machine learning.
- **Pandas:** Data manipulation and preprocessing.
- **NumPy:** Numerical computations.
- **Matplotlib & Seaborn:** Data visualization.
- **Scikit-learn:** Machine learning model development and evaluation.
- **Jupyter Notebook:** Experimentation and documentation.
- **Git & GitHub:** Version control and project collaboration.

## 🚀 Future Development Roadmap

The current dataset provides a starting point. However, my ambition is to develop AgroPredict AI into a locally relevant agricultural prediction and decision-support system.

### Phase 1: Improve the Initial Model
- Conduct cross-validation.
- Perform further residual and prediction error analysis.
- Investigate feature importance and model interpretability.
- Explore additional regression algorithms and hyperparameter tuning.

### Phase 2: Agricultural Data Enrichment

Integrate more reliable agricultural, geographical, soil, and climate information from established sources:

| Data Source | Planned Application |
|---|---|
| [FAO](https://www.fao.org/faostat/en/) | Agricultural production and crop yield statistics |
| [NASA POWER](https://power.larc.nasa.gov/) | Historical weather and climate data |
| [ISRIC SoilGrids](https://soilgrids.org/) | Soil properties and geographical soil information |
| [FAO GAEZ](https://gaez.fao.org/) | Agro-ecological zones and crop suitability |

These datasets will be assessed for geographical coverage, resolution, time period, and compatibility before integration.

### Phase 3: Local Agricultural Data Collection

A major part of the project will involve collecting farm-level data directly from farmers in Zamfara State and other parts of Nigeria.

The proposed data collection variables include:

| Category | Variables |
|---|---|
| Farm Information | Farm size, geographical location, and planting date |
| Crop Information | Crop type, variety, and seed type |
| Soil Information | Soil type, pH, and nutrient composition |
| Fertilizer Information | Fertilizer type, quantity, and application method |
| Planting Information | Row spacing, plant spacing, and plant population |
| Weather Information | Rainfall and temperature |
| Farm Management | Irrigation, weed, and pest management |
| Harvest Information | Harvest quantity and yield per hectare |

Actual harvest records will be particularly important for training and validating models against real farming outcomes.

### Phase 4: Zamfara-Specific Crop Yield Prediction

Develop and validate models using locally collected agricultural data, initially focusing on maize production in Zamfara State.

The model will progressively incorporate local soil conditions, climate patterns, farming practices, and crop varieties.

### Phase 5: Precision Agriculture Decision-Support System

The long-term objective is to develop a user-friendly application that can help farmers:

- Estimate expected crop yields.
- Understand factors associated with crop productivity.
- Explore the implications of different farming conditions.
- Make better-informed farm management decisions.
- Access agricultural insights relevant to their locations.

---

## 🌍 Long-Term Vision

I believe that combining machine learning, reliable agricultural datasets, local farming knowledge, and agronomic expertise can create meaningful opportunities for agricultural transformation.

AgroPredict AI is an ongoing effort to explore how data science can contribute to improved agricultural productivity, informed decision-making, and precision agriculture in Zamfara State and Nigeria at large.

## 🤝 Contributions and Collaboration

I welcome collaboration with:

- Data scientists and machine learning engineers.
- Agricultural researchers and agronomists.
- Farmers and agricultural extension workers.
- Agricultural technology organisations.
- Institutions and organisations with relevant agricultural datasets.

If you have ideas, datasets, or expertise that can contribute to this project, I welcome your collaboration.

## 👨‍💻 Project Author

**Muhammad Yunusa Badamasi**

Data Analyst | Data Scientist | Machine Learning Enthusiast | Agricultural Technology Advocate



---

**AgroPredict AI — Turning Agricultural Data into Better Farming Decisions.** 🌱
