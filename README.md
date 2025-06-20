Sales Dashboard with Forecasting
A dynamic and interactive Streamlit dashboard for analyzing and forecasting sales data. This app lets users explore key performance metrics, visualize trends, identify top-performing regions and products, and predict future sales using Facebook Prophet.

Features
Dashboard Tabs:

Overview – Total sales, units sold, average cost, top product, and region
Visualizations – Sales by product, time series trends, monthly breakdowns, pie chart shares
Top Insights – Top 5 regions and products by revenue, average price comparisons
Data & Export – View filtered records and download them as CSV
Forecasting – Select a product line and predict sales for the next 1–12 months using Prophet

Technologies:
Streamlit – Web app interface
pandas – Data handling
plotly – Interactive visualizations
Prophet – Time series forecasting
matplotlib – Forecast components visualization

How to Use

1. Clone the repository:
git clone https://github.com/yourusername/sales-dashboard-forecast.git
cd sales-dashboard-forecast

2. Install dependencies:
pip install -r requirements.txt

3. Run the app:
streamlit run sales_dashboard.py

4. Upload the data:
Upload the sample dataset sales_data_sample.csv from Kaggle or any sales dataset with the required columns:
ORDERDATE, PRODUCTLINE, SALES, QUANTITYORDERED, PRICEEACH, TERRITORY

Forecasting Logic

Forecast is performed on sales totals by ORDERDATE per selected PRODUCTLINE
Model: Facebook Prophet
Forecast period: Adjustable from 1 to 12 months
Output: Predicted trend line with upper/lower bounds and seasonality breakdown
Sample Output Screenshots
Include screenshots of each tab (especially the Forecast tab with charts).

requirements.txt
txt
Copy
Edit
streamlit
pandas
plotly
prophet
matplotlib

Academic Relevance
This project is suitable as a Master’s-level capstone or advanced data science portfolio project. It demonstrates:
Real-world data preprocessing
Interactive UI with dynamic filtering
Time series modeling
Business insight generation
Future Enhancements
Forecast by territory or region
Compare Prophet vs. ARIMA
Display model evaluation metrics (MAE, RMSE)
Deploy to Streamlit Cloud with custom theme
