# Business-Wise Analysis

A comprehensive data analysis toolkit for business intelligence and maintenance analytics, featuring advanced machine learning capabilities, AI-powered insights, and automated report generation.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Sample Data](#sample-data)
- [Installation](#installation)
- [Usage](#usage)
- [Output Types](#output-types)
- [Technologies Used](#technologies-used)
- [Configuration](#configuration)
- [Contributing](#contributing)

## 🔍 Overview

This project provides two main analysis approaches for business data, with a focus on maintenance analytics and general business intelligence:

1. **Project 1**: Advanced maintenance analysis system with comprehensive AI/ML capabilities
2. **Project 2**: Streamlined maintenance analysis with enhanced reporting features

Both projects are designed to automatically analyze datasets, generate insights, and produce professional reports in HTML and PDF formats.

## ✨ Features

### Core Analysis Capabilities
- **Automatic Data Type Inference**: Intelligently detects column types and suggests appropriate analyses
- **Comprehensive Statistical Analysis**: Correlation analysis, distribution analysis, and descriptive statistics
- **Anomaly Detection**: Multiple algorithms (Isolation Forest, LOF, Statistical methods)
- **Time Series Analysis**: Temporal pattern detection and forecasting
- **Predictive Modeling**: Multiple ML algorithms (Random Forest, LightGBM, XGBoost)
- **Text Analytics**: NLP processing with sentiment analysis and entity extraction
- **Data Quality Assessment**: Missing value analysis, duplicate detection, and quality scoring

### AI-Powered Features
- **LLM Integration**: OpenAI GPT and local models for intelligent insights
- **Business Recommendations**: AI-generated actionable recommendations
- **Pattern Recognition**: Automated identification of business patterns
- **Smart Reporting**: Context-aware report generation

### Visualization & Reporting
- **Interactive Visualizations**: Plotly-based charts and graphs
- **Professional Reports**: HTML and PDF report generation
- **Executive Summaries**: AI-generated executive summaries
- **Dashboard Components**: Statistical cards, charts, and tables

## 📁 Project Structure

```
business-wise-analysis/
├── project1.py              # Advanced analysis system with full AI/ML pipeline
├── project2.py              # Streamlined analysis with enhanced reporting
├── requirements.txt         # Python dependencies
├── sample.csv              # Primary maintenance dataset
├── sample2.csv             # Secondary work order dataset
├── output_results/         # Project 2 output directory
│   ├── maintenance_report.html
│   ├── maintenance_report.pdf
│   └── images/
│       ├── category_costs.png
│       ├── cost_analysis.png
│       └── maintenance_types.png
├── output_results2/        # Alternative output directory
├── output_results_project1_dataset1/  # Project 1 comprehensive output
│   ├── report.html
│   ├── report.pdf
│   ├── anomalies.png
│   ├── correlation_matrix.png
│   ├── numerical_distributions.png
│   ├── time_series.png
│   ├── box_plots.html
│   ├── interactive_correlation.html
│   ├── scatter_matrix.html
│   └── predictive_analysis.html
└── output_results_project1_dataset2/  # Project 1 secondary analysis
```

## 📊 Sample Data

The project includes two sample datasets:

### Primary Dataset (sample.csv)
- **Records**: 502 maintenance records
- **Columns**: Equipment Name, Equipment ID, Criticality Level, Task ID, Task Description, Start Date, End Date, Duration, Maintenance Cost
- **Use Case**: Equipment maintenance analysis, cost optimization, predictive maintenance

### Secondary Dataset (sample2.csv)  
- **Records**: 157 work order records
- **Columns**: Work Order ID, Technician Name, Technician ID, Parts Used, Parts Cost, Work Hours, Task Status, Completion Notes, Equipment ID, Task ID
- **Use Case**: Work order analysis, technician performance, parts usage tracking

## 🚀 Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Setup

1. **Clone the repository**:
```bash
git clone https://github.com/ahmed-hesham07/business-wise-analysis.git
cd business-wise-analysis
```

2. **Install dependencies**:
```bash
pip install -r requirements.txt
```

3. **Download NLTK data** (automatically handled by the scripts):
```python
import nltk
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('averaged_perceptron_tagger')
```

4. **Install system dependencies** (optional for PDF generation):
```bash
# For wkhtmltopdf (PDF generation)
# Windows: Download from https://wkhtmltopdf.org/downloads.html
# Linux: sudo apt-get install wkhtmltopdf
# macOS: brew install wkhtmltopdf
```

## 💻 Usage

### Project 1: Advanced Analysis System

```bash
# Basic usage with default dataset
python project1.py

# Custom configuration
python project1.py --data-path your_data.csv --output-folder custom_output
```

**Features**:
- Comprehensive AI/ML pipeline
- Multiple predictive models
- Advanced anomaly detection
- Text analytics with NLP
- LLM-powered insights
- Interactive visualizations

### Project 2: Streamlined Analysis

```bash
# Analyze default dataset
python project2.py

# Analyze custom dataset
python project2.py path/to/your/data.csv
```

**Features**:
- Enhanced HTML/PDF reporting
- Business recommendation engine
- Executive summary generation
- Cost analysis and optimization
- Equipment performance analysis

### Configuration Options

#### Project 1 Configuration
```python
config = {
    'target_column': 'maintenance_cost',
    'date_column': 'maintenance_date',
    'random_state': 42,
    'test_size': 0.2,
    'categorical_threshold': 10,
    'anomaly_contamination': 0.1
}

llm_config = {
    'model_name': 'gpt-3.5-turbo',
    'temperature': 0.7,
    'local_llm': True,  # Use local models
    'api_key': 'your_openai_key'  # For OpenAI models
}
```

## 📈 Output Types

### Analysis Reports
- **HTML Reports**: Interactive reports with embedded visualizations
- **PDF Reports**: Professional printable versions
- **Executive Summaries**: AI-generated business insights

### Visualizations
- **Correlation Matrices**: Feature relationship analysis
- **Time Series Plots**: Temporal pattern visualization
- **Cost Analysis Charts**: Financial trend analysis
- **Anomaly Detection Plots**: Outlier identification
- **Distribution Analysis**: Statistical distributions
- **Predictive Model Performance**: ML model comparisons

### Business Intelligence
- **Recommendation Cards**: Prioritized action items
- **Performance Metrics**: KPI dashboards
- **Quality Assessments**: Data quality scoring
- **Pattern Recognition**: Automated insights

## 🛠 Technologies Used

### Core Technologies
- **Python 3.8+**: Primary programming language
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Scikit-learn**: Machine learning algorithms

### Visualization
- **Matplotlib**: Static plotting
- **Seaborn**: Statistical visualizations
- **Plotly**: Interactive charts and dashboards

### Machine Learning
- **LightGBM**: Gradient boosting framework
- **XGBoost**: Extreme gradient boosting
- **Prophet**: Time series forecasting
- **Isolation Forest**: Anomaly detection
- **SHAP**: Model interpretability

### AI/NLP
- **Transformers**: Hugging Face transformers
- **NLTK**: Natural language processing
- **spaCy**: Advanced NLP capabilities
- **OpenAI**: GPT model integration
- **LangChain**: LLM application framework

### Reporting
- **Jinja2**: Template engine
- **pdfkit**: PDF generation
- **WeasyPrint**: Alternative PDF generation
- **HTML/CSS**: Professional styling

### Additional Libraries
- **Optuna**: Hyperparameter optimization
- **Yellowbrick**: ML visualization
- **Feature Engine**: Feature engineering
- **Imbalanced-learn**: Handling imbalanced datasets

## ⚙️ Configuration

### Environment Variables
```bash
# For OpenAI integration
export OPENAI_API_KEY="your_api_key_here"

# For custom model paths
export HF_MODEL_PATH="/path/to/local/models"
```

### Custom Analysis Parameters
- **Categorical Threshold**: Determines categorical vs. continuous variables
- **Anomaly Contamination**: Expected proportion of outliers
- **Cross-validation Folds**: For model evaluation
- **Test Size**: Train/test split ratio
- **Feature Importance Threshold**: Minimum importance for feature selection

### LLM Configuration
- **Local Models**: Use Hugging Face transformers locally
- **OpenAI Integration**: Cloud-based GPT models
- **Temperature**: Controls randomness in AI responses
- **Max Tokens**: Limits response length

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines
- Follow PEP 8 style guidelines
- Add docstrings for all functions
- Include unit tests for new features
- Update documentation for API changes

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🎯 Use Cases

### Maintenance Analytics
- Equipment performance optimization
- Predictive maintenance scheduling
- Cost reduction strategies
- Resource allocation planning

### Business Intelligence
- Operational efficiency analysis
- Risk assessment and management
- Performance benchmarking
- Strategic decision support

### Data Science Applications
- Automated exploratory data analysis
- Feature engineering and selection
- Model selection and evaluation
- Insight generation and reporting

## 📞 Support

For questions, issues, or contributions:

- **GitHub Issues**: [Report bugs or request features](https://github.com/ahmed-hesham07/business-wise-analysis/issues)
- **Documentation**: Check inline code documentation
- **Examples**: Review sample outputs in the project directories

---

**Note**: This toolkit is designed for business analysts, data scientists, and maintenance professionals who need comprehensive, automated analysis capabilities with professional reporting features.
