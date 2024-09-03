# Used Car Price Analysis Project

## Project Overview
This project analyzes a dataset of used car listings to identify key factors influencing car prices. The goal is to provide actionable insights to a used car dealership for optimizing their inventory and pricing strategies.

## Table of Contents
* Project Structure
* Key Findings
* Recommendations
* Methodology
* Tools Used
* How to Use This Repository
* Future Work
* License

## Project Structure
* used_car_price_analysis.ipynb: Jupyter notebook containing the full analysis
* data/vehicles.csv: Dataset of used car listings
* images/: Directory containing images used in the notebook
   * crisp.png: Image of the CRISP-DM process
   * kurt.jpeg: Sample image
* requirements.txt: List of Python packages required for this project

## Key Findings

1. **Model Performance:** Our Random Forest model achieved the best performance with an R² of 0.93, indicating that our model can explain 93% of the variance in car prices. This high accuracy suggests that our model can provide reliable price estimates for used cars.

2. **Most Important Factors Affecting Car Prices:**
   * **Age and Year:** The age of the car and its year of manufacture are the two most crucial factors in determining price. Newer cars would be obvious to command higher prices.
   * **Mileage:** The odometer reading is the third most important factor. Lower mileage vehicles are generally priced higher.
   * **Drive Type:** Front-wheel drive (FWD) vehicles have a significant impact on pricing.
   * **Fuel Type:** Diesel vehicles have distinct pricing characteristics compared to other fuel types.

3. **Non-linear Relationships:** Non-linear models such as Random Forest and Decision Tree performed much better than the linear model, which suggest that the relationship between the features and car prices are complex and non-linear.

## Recommendations
1. **Focus on Newer, Low-Mileage Vehicles:** Prioritize stocking newer cars with lower mileage, as these factors most strongly influence price and potential profit margins.
2. **Diverse Drive Types:** Maintain a balance of different drive types in your inventory, with a slight emphasis on front-wheel drive vehicles.
3. **Fuel Type Considerations:** Pay special attention to diesel vehicles when pricing, as they have distinct value characteristics.
4. **Regular Revaluation:** Given the importance of age and mileage, regularly update your pricing to reflect these changing factors.

## Methodology
1. **Data Cleaning:** Handled missing values, removed outliers, and engineered new features.
2. **Exploratory Data Analysis:** Visualized distributions and relationships between variables.
3. **Feature Engineering:** Created 'car_age' feature and simplified the 'model' column.
4. **Modeling:** Trained and compared Linear Regression, Decision Tree, and Random Forest models.
5. **Hyperparameter Tuning:** Performed grid search for Random Forest hyperparameters.
6. **Feature Importance Analysis:** Identified the most influential factors in determining car prices.

## Tools Used
* Python
* Pandas for data manipulation
* Scikit-learn for machine learning models
* Matplotlib and Seaborn for data visualization

## How to Use This Repository
1. Clone the repository to your local machine:
   ```
   git clone https://github.com/your-username/used-car-price-analysis.git
   ```
2. Navigate to the project directory:
   ```
   cd used-car-price-analysis
   ```
3. Install the required packages:
   ```
   pip install -r requirements.txt
   ```
4. Open the `used_car_price_analysis.ipynb` notebook in Jupyter Lab or Jupyter Notebook:
   ```
   jupyter notebook used_car_price_analysis.ipynb
   ```
5. Ensure that the data and images directories are in the same directory as the notebook. 
6. Run the cells in order to reproduce the analysis.

## Future Improvements
* Expand the grid search to include more hyperparameters for model optimization.
* Explore more advanced ensemble methods or deep learning approaches.
  
## License
This project is licensed under the MIT License - see the LICENSE.md file for details.
