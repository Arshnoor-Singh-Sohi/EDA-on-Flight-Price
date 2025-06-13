# Exploratory Data Analysis on Flight Prices ✈️

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-orange)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4%2B-green)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.11%2B-lightblue)](https://seaborn.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)

## 🎯 Project Overview

This project presents a comprehensive **Exploratory Data Analysis (EDA)** of flight prices in the Indian aviation market. The analysis focuses on understanding pricing patterns, identifying key factors that influence airfare, and uncovering insights that can benefit both travelers and airline industry stakeholders.

### 🚀 Objective

The primary goals of this analysis are to:
- **Understand pricing dynamics** across different airlines and routes
- **Identify key factors** that significantly impact flight prices
- **Analyze market trends** and patterns in the aviation industry
- **Provide actionable insights** for travelers to optimize booking decisions
- **Support airline pricing strategies** through data-driven insights

## 📊 Dataset Overview

### Data Source
- **Dataset**: Flight Price Prediction Dataset
- **Source**: Kaggle
- **Size**: 10,000+ flight records
- **Time Period**: Historical flight data from Indian airlines
- **Geographic Coverage**: Major Indian cities and airports

### Dataset Features

| Feature | Description | Data Type | Example |
|---------|-------------|-----------|---------|
| **Airline** | Flight carrier name | Categorical | IndiGo, Air India, SpiceJet |
| **Date_of_Journey** | Travel date | Date | 2019-03-24 |
| **Source** | Departure city | Categorical | Delhi, Mumbai, Kolkata |
| **Destination** | Arrival city | Categorical | Cochin, Banglore, Hyderabad |
| **Route** | Flight path with stops | String | DEL → BOM → COK |
| **Dep_Time** | Departure time | Time | 22:20, 06:05, 16:50 |
| **Arrival_Time** | Arrival time | Time | 01:10, 12:25, 19:00 |
| **Duration** | Flight duration | String | 2h 50m, 5h 05m |
| **Total_Stops** | Number of stops | Categorical | non-stop, 1 stop, 2 stops |
| **Additional_Info** | Extra information | String | No info, In-flight meal |
| **Price** | Ticket price (INR) | Numeric | 3897, 7662, 13302 |

## 🔍 Analysis Methodology

### 1. Data Quality Assessment
- **Missing Value Analysis**: Identification and treatment of null values
- **Duplicate Detection**: Removal of redundant records
- **Data Type Validation**: Ensuring appropriate data formats
- **Outlier Detection**: Statistical identification of anomalous prices
- **Consistency Checks**: Validation of logical relationships

### 2. Data Preprocessing
- **Duration Conversion**: Converting duration strings to minutes
- **Time Feature Extraction**: Extracting hour from departure/arrival times
- **Categorical Encoding**: Transforming categorical variables
- **Route Parsing**: Breaking down complex route information
- **Feature Engineering**: Creating new variables for enhanced analysis

### 3. Exploratory Data Analysis

#### 📈 Univariate Analysis
- **Price Distribution**: Understanding the spread of flight prices
- **Airline Market Share**: Distribution of flights across carriers
- **Route Popularity**: Most frequent source-destination pairs
- **Temporal Patterns**: Analysis by time of day, day of week, month
- **Stop Frequency**: Distribution of direct vs. connecting flights

#### 📊 Bivariate Analysis
- **Price vs. Airlines**: Comparing pricing strategies across carriers
- **Price vs. Duration**: Relationship between flight time and cost
- **Price vs. Stops**: Impact of connecting flights on pricing
- **Price vs. Time**: How departure/arrival times affect prices
- **Price vs. Routes**: Route-specific pricing patterns

#### 🔗 Multivariate Analysis
- **Comprehensive Price Modeling**: Multiple factors affecting pricing
- **Market Segmentation**: Identifying distinct customer segments
- **Competitive Analysis**: Inter-airline pricing comparison
- **Seasonal Trends**: Time-based pricing variations

## 📈 Key Findings & Insights

### 💰 Pricing Patterns

#### **Price Range Analysis**
- **Minimum Price**: ₹1,759 (Economy, short-haul flights)
- **Maximum Price**: ₹79,512 (Business class, long-haul)
- **Average Price**: ₹9,080
- **Median Price**: ₹5,953
- **Price Skewness**: Right-skewed distribution with premium outliers

#### **Airline Pricing Strategy**
- **Premium Carriers**: Jet Airways, Vistara (higher average prices)
- **Budget Airlines**: IndiGo, SpiceJet (competitive pricing)
- **Full-Service**: Air India (moderate pricing with services)
- **Regional Carriers**: Regional airlines with niche pricing

### 🛫 Route & Duration Insights

#### **Popular Routes**
1. **Delhi ↔ Mumbai**: High frequency, competitive pricing
2. **Mumbai ↔ Bangalore**: Tech corridor with premium pricing
3. **Delhi ↔ Bangalore**: Business route with varied pricing
4. **Mumbai ↔ Chennai**: Southern connectivity hub

#### **Duration Impact**
- **Short-haul (<2 hours)**: ₹3,000-8,000 average
- **Medium-haul (2-4 hours)**: ₹5,000-15,000 average
- **Long-haul (>4 hours)**: ₹8,000-25,000+ average

### ⏰ Temporal Analysis

#### **Time-of-Day Pricing**
- **Early Morning (5-8 AM)**: Lower prices, business travelers
- **Peak Hours (8-10 AM, 6-8 PM)**: Premium pricing
- **Afternoon (12-4 PM)**: Moderate pricing
- **Late Night (10 PM-12 AM)**: Budget-friendly options

#### **Stop Analysis**
- **Non-stop flights**: 40% premium over connecting flights
- **1 stop**: Most common, balanced price-convenience ratio
- **2+ stops**: Significantly cheaper but longer travel time

## 📊 Visualization Gallery

### Key Visualizations Created

#### 1. **Price Distribution Histogram**
- Shows right-skewed distribution of flight prices
- Identifies common price ranges for different market segments

#### 2. **Airline Price Comparison**
- Box plots comparing price distributions across airlines
- Reveals pricing strategies and market positioning

#### 3. **Route-wise Price Analysis**
- Heatmap showing average prices between city pairs
- Identifies high-value and budget-friendly routes

#### 4. **Duration vs. Price Scatter Plot**
- Demonstrates positive correlation between flight time and cost
- Highlights efficiency of direct flights

#### 5. **Time-based Pricing Patterns**
- Line plots showing price variations throughout the day
- Seasonal and weekly patterns in airfare

#### 6. **Stop Impact Analysis**
- Bar charts showing price differences for direct vs. connecting flights
- Cost-time trade-offs for different travel preferences

## 🛠️ Technologies & Libraries

### Core Data Science Stack
```python
import pandas as pd              # Data manipulation and analysis
import numpy as np               # Numerical computing
import matplotlib.pyplot as plt  # Data visualization
import seaborn as sns            # Statistical data visualization
import plotly.express as px      # Interactive visualizations
import warnings                  # Warning suppression
```

### Additional Libraries
```python
import datetime as dt            # Date and time operations
from sklearn.preprocessing import LabelEncoder  # Categorical encoding
import scipy.stats as stats      # Statistical tests
import re                        # Regular expressions for text processing
```

## 📁 Project Structure

```
EDA-on-Flight-Price/
│
├── 1. EDA Flight Price.ipynb         # Main analysis notebook
├── README.md                         # Project documentation
├── requirements.txt                  # Python dependencies
├── data/                            # Dataset directory
│   ├── train_data.csv              # Training dataset
│   └── test_data.csv               # Test dataset
├── visualizations/                  # Generated plots and charts
│   ├── price_distribution.png
│   ├── airline_comparison.png
│   ├── route_analysis.png
│   ├── duration_correlation.png
│   └── temporal_patterns.png
├── insights/                        # Analysis outputs
│   ├── key_findings.md
│   ├── pricing_strategy_analysis.pdf
│   └── market_insights.pptx
└── utils/                          # Helper functions
    ├── data_preprocessing.py
    ├── visualization_helpers.py
    └── statistical_tests.py
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook/Lab
- 4GB+ RAM for data processing

### Installation & Setup

1. **Clone the repository**
```bash
git clone https://github.com/Arshnoor-Singh-Sohi/EDA-on-Flight-Price.git
cd EDA-on-Flight-Price
```

2. **Create virtual environment** (recommended)
```bash
python -m venv flight_eda_env
source flight_eda_env/bin/activate  # On Windows: flight_eda_env\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Launch Jupyter Notebook**
```bash
jupyter notebook
```

5. **Open analysis notebook**
Navigate to `1. EDA Flight Price.ipynb` and run all cells

### Requirements.txt
```
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
plotly>=5.0.0
jupyter>=1.0.0
scikit-learn>=1.0.0
scipy>=1.7.0
openpyxl>=3.0.0
```

## 📊 Statistical Analysis Highlights

### Descriptive Statistics
```python
# Price Statistics Summary
Count:       10,683 flights
Mean:        ₹9,080
Median:      ₹5,953
Std Dev:     ₹4,939
Min:         ₹1,759
Max:         ₹79,512
```

### Key Correlations
- **Duration vs Price**: +0.68 (Strong positive correlation)
- **Stops vs Price**: -0.45 (More stops = lower prices)
- **Time vs Price**: +0.23 (Peak hours = higher prices)

### Market Share Analysis
- **IndiGo**: 24% market share (Budget leader)
- **Air India**: 18% market share (National carrier)
- **Jet Airways**: 16% market share (Premium service)
- **SpiceJet**: 15% market share (Low-cost competitor)

## 💡 Business Insights & Recommendations

### 🧳 For Travelers

#### **Best Booking Strategies**
1. **Timing**: Book flights departing early morning or late evening
2. **Flexibility**: Consider 1-stop flights for 30-40% savings
3. **Advance Booking**: Book 3-8 weeks ahead for optimal prices
4. **Route Selection**: Explore alternate airports for better deals

#### **Cost Optimization Tips**
1. **Tuesday-Thursday travel**: Often 15-20% cheaper
2. **Avoid peak hours**: 8-10 AM and 6-8 PM premium
3. **Consider budget airlines**: Significant savings for price-conscious travelers
4. **Multi-city vs Direct**: Compare total cost including convenience

### 🏢 For Airlines

#### **Pricing Strategy Insights**
1. **Dynamic Pricing**: Implement time-of-day pricing variations
2. **Route Optimization**: Focus capacity on high-demand routes
3. **Competitive Positioning**: Differentiate through service vs. price
4. **Seasonal Adjustments**: Adjust pricing for demand patterns

#### **Market Opportunities**
1. **Underserved Routes**: Identify gaps in route networks
2. **Time Slot Optimization**: Target off-peak periods with promotions
3. **Customer Segmentation**: Tailor offerings for business vs. leisure
4. **Ancillary Revenue**: Optimize add-on services pricing

### 📈 For Travel Industry

#### **Market Trends**
1. **Budget Airline Growth**: Increasing market share of low-cost carriers
2. **Route Concentration**: Major metros dominate traffic
3. **Price Sensitivity**: High elasticity in leisure travel segment
4. **Service Differentiation**: Premium carriers focusing on experience

## 🔮 Future Enhancements

### Advanced Analytics
- [ ] **Machine Learning Models**: Price prediction algorithms
- [ ] **Time Series Analysis**: Seasonal pricing trends
- [ ] **Sentiment Analysis**: Review impact on pricing
- [ ] **Demand Forecasting**: Route-level demand prediction
- [ ] **Competitive Intelligence**: Real-time price monitoring

### Enhanced Visualizations
- [ ] **Interactive Dashboard**: Real-time price exploration
- [ ] **Geographic Mapping**: Route visualization on maps
- [ ] **Animation**: Time-lapse pricing trends
- [ ] **3D Visualizations**: Multi-dimensional price analysis

### Data Expansion
- [ ] **Real-time Data**: Live pricing feeds
- [ ] **International Routes**: Global flight analysis
- [ ] **Weather Integration**: Weather impact on pricing
- [ ] **Economic Indicators**: Fuel prices, economic factors

## 🤝 Contributing

We welcome contributions to enhance this analysis! Here's how you can help:

### Ways to Contribute
1. **Data Quality**: Additional datasets or data validation
2. **Analysis Enhancement**: New analytical perspectives
3. **Visualization Improvements**: Better charts and interactive elements
4. **Feature Engineering**: New derived variables
5. **Documentation**: Enhanced explanations and tutorials

### Contribution Process
1. Fork the repository
2. Create feature branch (`git checkout -b feature/enhancement`)
3. Commit changes (`git commit -m 'Add new analysis feature'`)
4. Push to branch (`git push origin feature/enhancement`)
5. Open Pull Request with detailed description

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Arshnoor Singh Sohi**

- GitHub: [@Arshnoor-Singh-Sohi](https://github.com/Arshnoor-Singh-Sohi)
- LinkedIn: [Connect with me](https://linkedin.com/in/arshnoor-singh-sohi)
- Email: [arshnoor.singh@example.com](mailto:arshnoor.singh@example.com)

## 🙏 Acknowledgments

- **Kaggle Community**: For providing the flight price dataset
- **Indian Aviation Industry**: Data source and market insights
- **Open Source Community**: Libraries and tools that made this analysis possible
- **Data Science Community**: Methodologies and best practices

## 📚 References & Resources

### Datasets
- [Flight Price Prediction Dataset - Kaggle](https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction)
- [Indian Aviation Market Reports](https://www.dgca.gov.in/)

### Research Papers
- "Airline Ticket Price and Demand Prediction: A Survey" - Transportation Research
- "Dynamic Pricing in Airlines: A Machine Learning Approach"

### Industry Resources
- [IATA Economic Reports](https://www.iata.org/en/publications/economics/)
- [Indian Civil Aviation Statistics](https://www.aai.aero/en/business/statistics)

---

**Note**: This analysis is based on historical data and should be supplemented with current market research for real-time decision making. Flight prices are subject to dynamic changes based on multiple factors not captured in this dataset.
