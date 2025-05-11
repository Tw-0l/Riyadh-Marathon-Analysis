# Riyadh Marathon Analysis

![Riyadh Marathon](https://img.shields.io/badge/Riyadh-Marathon-darkgreen?style=for-the-badge)
![Data Analysis](https://img.shields.io/badge/Data-Analysis-blue?style=for-the-badge)
![Sports Analytics](https://img.shields.io/badge/Sports-Analytics-orange?style=for-the-badge)

## 🏃‍♂️ Project Overview
A comprehensive data analysis project examining the Riyadh Marathon, one of Saudi Arabia's premier sporting events. This analysis explores participant demographics, performance metrics, race conditions, and event growth to provide insights for runners, organizers, and sports analysts.

## 🎯 Project Objectives
- Analyze performance patterns across different demographics and race categories
- Identify factors influencing marathon completion times
- Visualize participant distribution and growth trends
- Examine the economic and social impact of the Riyadh Marathon
- Provide actionable insights for race organizers and future participants

## 📊 Data Insights

### Participant Analytics
- Demographic breakdown (age, gender, nationality)
- First-time vs. returning runner analysis
- International participation trends
- Registration patterns and category preferences

### Performance Analysis
- Finish time distributions by category
- Pace analysis and split time trends
- Correlation between training data and race performance
- DNF (Did Not Finish) rate analysis and factors

### Course & Conditions Impact
- Weather effects on performance metrics
- Elevation profile analysis and its impact on pacing
- Hydration station effectiveness
- Crowd support zones and their influence on runner performance

### Event Growth & Development
- Year-over-year participation growth
- Economic impact on Riyadh tourism and local businesses
- Social media engagement and event visibility
- Comparison with other major Middle Eastern marathons

## 📈 Key Findings
- The Riyadh Marathon has seen a X% year-over-year growth in participants
- International runner participation has increased significantly, with participants from X countries
- Temperature has a statistically significant impact on average finish times (p < 0.05)
- Peak performance age brackets differ between male and female participants
- Hydration station placement optimization could improve overall finish times
- Local community engagement has increased Y% based on volunteer participation metrics

## 🔍 Methodology
- Data collection from official race results and participant surveys
- Cleaning and preprocessing of timing data
- Statistical analysis using Python (pandas, scipy, statsmodels)
- Geospatial analysis of runner distributions and course elements
- Visualization with matplotlib, seaborn, and interactive plotly dashboards
- Comparative analysis with international marathon benchmarks

## 🛠️ Technologies Used
- **Python**: Core programming language
- **Pandas & NumPy**: Data manipulation and analysis
- **Matplotlib & Seaborn**: Static visualizations
- **Plotly & Dash**: Interactive visualizations and dashboards
- **GeoPandas**: Geospatial analysis
- **Scikit-learn**: Predictive modeling (for performance prediction)
- **Jupyter Notebooks**: Interactive development and presentation

## 📁 Repository Structure
```
Riyadh-Marathon-Analysis/
├── data/
│   ├── raw/                      # Original race data
│   ├── processed/                # Cleaned and transformed data
│   └── external/                 # Additional relevant datasets
├── notebooks/
│   ├── 01_data_exploration.ipynb # Initial exploratory analysis
│   ├── 02_demographic_analysis.ipynb
│   ├── 03_performance_metrics.ipynb
│   ├── 04_weather_impact.ipynb
│   └── 05_growth_trends.ipynb
├── src/
│   ├── data/                     # Data processing scripts
│   ├── visualization/            # Visualization utilities
│   └── analysis/                 # Analysis modules
├── reports/
│   ├── figures/                  # Generated visualizations
│   └── summaries/                # Analysis summaries and reports
├── dashboard/                    # Interactive Dash application
├── requirements.txt              # Project dependencies
└── README.md                     # Project documentation
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- pip package manager

### Installation
1. Clone the repository
   ```bash
   git clone https://github.com/Tw-0l/Riyadh-Marathon-Analysis.git
   cd Riyadh-Marathon-Analysis
   ```

2. Create and activate a virtual environment
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. Install required dependencies
   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter to explore notebooks
   ```bash
   jupyter notebook
   ```

5. Run the interactive dashboard (if implemented)
   ```bash
   cd dashboard
   python app.py
   ```

## 💻 Usage Examples

### Performance Analysis
```python
# Example code for analyzing finish times
from src.analysis.performance import PerformanceAnalyzer

# Initialize analyzer with data
analyzer = PerformanceAnalyzer('data/processed/race_results.csv')

# Analyze finish time distributions by age group
analyzer.plot_finish_time_by_age_group()

# Compare male vs female pace strategies
analyzer.compare_gender_pacing_strategy()
```

### Weather Impact
```python
# Example code for analyzing weather impacts
from src.analysis.environmental import WeatherImpactAnalyzer

# Initialize analyzer with race and weather data
analyzer = WeatherImpactAnalyzer(
    'data/processed/race_results.csv',
    'data/external/weather_data.csv'
)

# Analyze temperature impact on performance
analyzer.plot_temperature_vs_finish_time()

# Calculate performance degradation per degree
degradation = analyzer.calculate_time_degradation_per_degree()
print(f"Average performance degradation: {degradation:.2f} sec/°C")
```

## 🌐 Interactive Dashboard
The project includes an interactive dashboard that allows users to:
- Filter and explore race results by multiple dimensions
- Compare year-over-year performance metrics
- Visualize the marathon course with performance hotspots
- Generate personalized insights for specific demographic groups

## 🇸🇦 Local Context
This analysis incorporates several factors specific to the Riyadh context:
- Impact of desert climate and seasonal conditions
- Cultural factors influencing participation demographics
- Saudi Vision 2030's sports and wellness initiatives
- Urban development around the marathon route
- Growth of running as a sport in Saudi Arabia

## 🏆 Practical Applications
- **Runners**: Training recommendations and performance benchmarking
- **Race Organizers**: Logistics optimization and participant experience enhancement
- **Sponsors**: Targeted engagement opportunities
- **City Planners**: Urban impact assessment and future planning
- **Tourism Board**: Event promotion and economic impact analysis

## 🔮 Future Enhancements
- Integration with wearable device data for deeper performance insights
- Machine learning models to predict individual finish times
- Real-time dashboard for future race monitoring
- Sentiment analysis of social media engagement
- Expanded analysis comparing with other Saudi sporting events

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request or open an Issue to suggest improvements or additional analyses.

## 📊 Data Sources
- Official Riyadh Marathon results
- Weather data from meteorological services
- Participant surveys and feedback
- Saudi General Authority for Statistics demographic data
- Social media engagement metrics
- *Note: Specific data sources and collection methodologies are detailed in the data documentation*


## 📞 Contact
- GitHub: [@Tw-0l](https://github.com/Tw-0l)

---

*This project aims to provide data-driven insights into the Riyadh Marathon, contributing to the growth of running culture in Saudi Arabia and supporting the Kingdom's Vision 2030 goals for promoting health, wellness, and an active lifestyle among its citizens.*
