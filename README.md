# Auto Marketing Analytics: Sales Call Patterns & Insurance Segmentation

![Data analytics illustration](images/hero.png)

## Project Overview

This repository contains a self‑contained project exploring marketing analytics for the automobile insurance industry.  Using a real‑world marketing dataset, the project studies sales call patterns, predicts customer responses to marketing campaigns and segments customers based on demographic and policy attributes.  The work aims to provide actionable insights for cross‑selling insurance products and improving marketing efficiency.

## Dataset

The dataset (`marketing.csv`) contains records from an auto insurance company's marketing campaigns. Each row represents a customer along with demographic variables, policy information and marketing response indicators.  Selected columns include:

- **Customer** – unique customer identifier.
- **State** – U.S. state in which the customer resides.
- **Customer Lifetime Value** – estimated lifetime value of the customer to the insurer.
- **Response** – whether the customer responded to the marketing campaign.
- **Coverage** – type of insurance coverage (Basic, Extended, Premium).
- **Education** – highest education level achieved.
- **Effective To Date** – date when the policy became effective.
- **Employment Status** – employment category (e.g., Employed, Unemployed, Retired).
- **Gender** – male or female.
- **Income** – annual income of the customer.

These variables are part of a larger set of features used in the notebook and are typical of customer‑lifetime‑value datasets【59518422723781†screenshot】.  For additional context on the kind of variables used in insurance segmentation projects, see the dataset metadata description for a similar auto insurance segmentation study【312305661522245†L324-L341】.

## Exploratory Data Analysis

The Jupyter notebook (`Project 2 – Automobile Marketing Analysis.ipynb`) walks through an extensive exploratory data analysis (EDA) of the marketing dataset.  Key steps include:

- Inspecting the distribution of numerical features such as customer lifetime value and income.
- Visualising categorical variables like coverage and response rates using bar charts and mosaics.
- Checking for missing values and performing basic data cleaning.
- Transforming date fields into useful time features.

Throughout the EDA, the notebook uses Python libraries (pandas, NumPy, seaborn, matplotlib) to highlight patterns in the data and to guide feature engineering decisions.

## Modeling & Segmentation

After exploring the data, the notebook builds predictive and unsupervised models to support marketing decisions:

- **Predictive modeling** – classification algorithms such as logistic regression and decision trees are used to predict whether customers will respond to marketing campaigns.  Model performance is evaluated using metrics like accuracy, precision and recall.
- **Customer segmentation** – clustering techniques (e.g., k‑means) are applied to group customers into distinct segments based on demographic and behavioural variables.  Segment profiles help marketing teams tailor campaigns and cross‑sell strategies.

For inspiration on how clustering is used in insurance segmentation, consult studies that employ k‑prototypes and similar algorithms【312305661522245†L324-L341】.

## Results

The analysis highlights several insights that can inform marketing strategy:

- Customers with higher lifetime value and premium coverage tend to be more responsive to cross‑selling.
- Education, employment status and income are strong differentiators between customer segments.
- Certain segments may require personalised offers or communication channels.

These findings are summarised in charts within the notebook and should be interpreted in the context of the business objectives.

## Getting Started

To reproduce the analysis on your own machine:

1. Clone this repository:

   ```bash
   git clone https://github.com/dmai287/auto_marketing_analytics.git
   cd auto_marketing_analytics
   ```

2. Create a Python environment (Python 3.8 or later) and install dependencies. If a `requirements.txt` file is provided, run:

   ```bash
   pip install -r requirements.txt
   ```

   Otherwise, install the necessary libraries manually (pandas, NumPy, scikit‑learn, matplotlib, seaborn, Jupyter Notebook).

3. Launch the notebook:

   ```bash
   jupyter notebook "Project 2 - Automobile Marketing Analysis.ipynb"
   ```

   or view the static HTML report (`Project 2 – Automobile Marketing Analysis.html`) directly in your browser.

The dataset `marketing.csv` is included for convenience; however, ensure you respect any associated data licensing or privacy considerations.

## Project Structure

```
auto_marketing_analytics/
├── Project 2 – Automobile Marketing Analysis.ipynb  # Jupyter notebook with full analysis
├── Project 2 – Automobile Marketing Analysis.html  # HTML export of the notebook
├── marketing.csv                                   # Source dataset
└── README.md                                       # Project documentation
```

Future enhancements could include adding a `requirements.txt`, modularising code into a Python package and integrating interactive dashboards.

## Contributing

Contributions are welcome!  If you find issues or have suggestions for improvements, please open an issue or submit a pull request.  When contributing:

- Ensure your code follows [PEP 8](https://pep8.org/) style guidelines.
- Provide clear commit messages and update documentation accordingly.
- Describe any changes in the pull request description so reviewers understand your motivation.

## License

This project does not currently specify a license.  To encourage reuse while protecting the author’s rights, consider adding an open‑source license (e.g., MIT License) to the repository.  See [choosealicense.com](https://choosealicense.com/) for guidance.

## Acknowledgments

- The underlying marketing dataset originates from industry‑standard auto insurance marketing data.
- Inspiration for segmentation techniques comes from academic studies on customer clustering and insurance analytics【312305661522245†L324-L341】.
<img width="1536" height="1024" alt="4a71960a-17ae-4c42-8af0-c10a5d9359a1" src="https://github.com/user-attachments/assets/30ed1832-81ac-4e67-87ff-6eb8efc4cd0d" />
