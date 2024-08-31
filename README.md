Stock Price Prediction using Linear Regression
This project involves predicting the closing stock prices of Netflix (NFLX) using Linear Regression. The dataset is processed, and a linear model is built to predict the closing prices based on historical stock data.

Project Structure
stock_price_prediction.ipynb: The Jupyter Notebook containing the code for data preprocessing, model building, training, evaluation, and visualization.
Dataset
NFLX.csv: The dataset used in this project, containing historical stock prices of Netflix, including features like Open, High, Low, Volume, and Close prices.
Setup and Installation
Clone the Repository:

bash
Copy code
git clone https://github.com/yourusername/stock-price-prediction.git
cd stock-price-prediction
Create a Virtual Environment (Optional but Recommended):

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
Install the Required Libraries:

Ensure you have the necessary Python libraries installed:

bash
Copy code
pip install numpy pandas matplotlib scikit-learn
Data Processing Steps
Loading the Data:

The dataset NFLX.csv is loaded into a Pandas DataFrame.
Exploratory Data Analysis:

The first few and last few rows of the dataset are displayed using df.head() and df.tail().
Missing values are checked with df.isna().sum().
Basic dataset information is viewed using df.shape(), df.info(), and df.describe().
Feature Selection:

The features Open, High, Low, Volume are selected as inputs (X), and Close is selected as the target variable (y).
The Date, Adj Close, and Close columns are dropped from the feature set.
Splitting the Data:

The data is split into training and testing sets using train_test_split().
Model Building
Linear Regression Model:

A Linear Regression model is instantiated and trained using the training data.
Predictions are made on the test set.
Model Evaluation:

The model is evaluated using various metrics, including Mean Squared Error (MSE), Mean Absolute Error (MAE), Mean Absolute Percentage Error (MAPE), and R-Squared Score.
Visualization:

A custom style() function is defined to set the visual style of plots with a black background and white text.
Various plots are generated to visualize the closing stock prices over time and to compare actual vs. predicted values.
Saving Results:

The actual and predicted stock prices are saved to a CSV file output_stock.csv.
Results
The model's performance metrics are displayed, and visualizations help to assess how well the model predicts the stock prices.
A final output CSV file contains the actual vs. predicted closing stock prices.
Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

License
This project is licensed under the MIT License - see the LICENSE file for details.
