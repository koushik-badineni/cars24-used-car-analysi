# 🚗 Cars24 Used Car Data Analysis & Web Scraping

Python-based web scraping and exploratory data analysis project that collects used car listings from Cars24 and analyzes car availability, locations, fuel types, transmission types, registration details, car models, and pricing patterns.

---

## 📌 Project Overview

The used car market in India is growing rapidly, and understanding trends across locations, car models, fuel types, and prices requires data-driven analysis.

This project uses **Python, Requests, BeautifulSoup, Pandas, Matplotlib, and Seaborn** to scrape used car data from Cars24, create a structured dataset, perform data cleaning, conduct exploratory data analysis (EDA), and generate meaningful business insights.

The project collected **773 used-car records with 8 attributes** for analysis.

---

## 🎯 Objectives

The main objectives of this project are:

1. Scrape used car data from Cars24.
2. Create a structured dataset from the scraped information.
3. Clean and preprocess the collected data.
4. Analyze used car availability across locations.
5. Analyze popular car models.
6. Analyze fuel type distribution.
7. Analyze transmission distribution.
8. Analyze registration patterns.
9. Analyze used car price patterns.
10. Generate meaningful business insights from the data.

---

## 🛠️ Technologies Used

| Technology       | Purpose                         |
| ---------------- | ------------------------------- |
| Python           | Programming and data processing |
| Requests         | Fetching website data           |
| BeautifulSoup    | Web scraping                    |
| Pandas           | Data manipulation and analysis  |
| NumPy            | Numerical operations            |
| Matplotlib       | Data visualization              |
| Seaborn          | Statistical visualization       |
| Jupyter Notebook | Development and analysis        |

---

## 🔄 Project Workflow

```text
Cars24 Website
      ↓
Web Scraping
      ↓
Dataset Creation
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
Data Visualization
      ↓
Business Insights
```

---

## 📂 Project Structure

```text
cars24-used-car-analysis/
│
├── data/
│   └── cars_data.csv
│
├── notebooks/
│   ├── 01_cars24_web_scraping.ipynb
│   └── 02_cars24_eda_visualization.ipynb
│
├── presentation/
│   └── Cars24_Used_Car_Data_Analysis.pdf
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 📊 Dataset

The scraped dataset contains information about used cars listed on Cars24.

### Dataset Information

* **Rows:** 773
* **Columns:** 8
* **Source:** Cars24
* **Format:** CSV

### Features

| Column         | Description                   |
| -------------- | ----------------------------- |
| `Car Name`     | Name/model of the car         |
| `Kilometers`   | Distance travelled by the car |
| `Fuel`         | Fuel type                     |
| `Transmission` | Transmission type             |
| `Registration` | Vehicle registration code     |
| `EMI`          | Listed EMI information        |
| `Final Price`  | Final listed price            |
| `Location`     | Location of the car listing   |

---

## 🕷️ Web Scraping

The `01_cars24_web_scraping.ipynb` notebook performs the data collection process.

### Scraping Process

* Sends HTTP requests to Cars24.
* Uses request headers to fetch website content.
* Parses HTML using BeautifulSoup.
* Extracts:

  * Car name
  * Kilometers
  * Fuel type
  * Transmission
  * Registration
  * EMI
  * Final price
  * Location
* Cleans and structures the extracted information.
* Creates a Pandas DataFrame.
* Saves the final dataset as `cars_data.csv`.

---

## 🧹 Data Cleaning & Preprocessing

The collected data was processed before performing analysis.

Major preprocessing steps include:

* Checking dataset shape and data types.
* Checking missing values.
* Checking duplicate records.
* Extracting numerical kilometer values.
* Identifying fuel types.
* Identifying transmission types.
* Extracting registration codes.
* Cleaning the `Final Price` column.
* Converting price values into numeric format.
* Preparing categorical and numerical columns for analysis.

---

## 📈 Exploratory Data Analysis

The `02_cars24_eda_visualization.ipynb` notebook performs exploratory data analysis and visualization.

### 1. Price Distribution

Analyzed the distribution of used car prices to understand the general price range of the collected listings.

### 2. Average Price by Registration

Calculated the average final price for different registration codes to observe price differences across registration categories.

### 3. Fuel Type Distribution

Analyzed the distribution of different fuel types available in the dataset.

### 4. Transmission Distribution

Compared the number of cars with different transmission types such as:

* Manual
* Automatic

### 5. Location-wise Analysis

Identified the **top 10 locations** with the highest number of used-car listings.

### 6. Car Model Analysis

Identified the **top 10 most frequently listed car models**.

### 7. Registration Analysis

Analyzed the distribution of cars across registration categories.

### 8. Price by Registration

Used box plots to compare the price distribution across different registration categories.

---

## 📊 Visualizations

The project includes the following visualizations:

* Price Distribution
* Average Price by Registration
* Fuel Type Distribution
* Transmission Distribution
* Top 10 Locations
* Top 10 Car Models
* Cars by Registration
* Price by Registration

---

## 🔍 Key Business Insights

### 1. Petrol Cars Dominate the Listings

Petrol vehicles represent a major portion of the collected used-car listings, indicating strong availability in the analyzed dataset.

### 2. Used Car Market is Budget-Oriented

A significant number of vehicles are concentrated in the lower price range, indicating strong representation of affordable used cars.

### 3. Certain Car Models Appear Frequently

Models from brands such as **Maruti, Hyundai, Tata, and Honda** appear repeatedly in the dataset, indicating strong representation among the collected listings.

### 4. Fuel Type is Related to Price

Different fuel types show differences in pricing, making fuel type an important factor to consider when analyzing used-car prices.

### 5. Location Influences Inventory Availability

Some locations contain considerably more listings than others, showing that used-car inventory varies across different areas.

### 6. Registration Categories Show Market Concentration

Certain registration categories contain a larger number of listings, indicating concentration of the collected inventory in particular registration regions.

---

## 💡 Business Value

This analysis can help understand:

* Where used cars are more widely available.
* Which car models are frequently listed.
* Which fuel types are commonly available.
* How transmission types are distributed.
* How used-car prices vary.
* How location and registration relate to inventory.
* Potential areas for further used-car market analysis.

---

## 🚀 Future Scope

The project can be extended with:

### 1. Used Car Price Prediction

Build a machine learning model to predict the price of a used car based on features such as:

* Car model
* Kilometers
* Fuel type
* Transmission
* Registration
* Location

### 2. Machine Learning Recommendations

Develop a recommendation system that suggests suitable used cars based on user preferences and budget.

### 3. Interactive Dashboard

Create an interactive dashboard using **Streamlit** or **Power BI** to allow users to explore the collected data.

### 4. Real-Time Data Collection

Automate the scraping and data-processing pipeline to collect updated used-car listings periodically.

### 5. Advanced Price Analysis

Develop more detailed analysis to understand how mileage, registration, location, fuel type, and car model affect used-car prices.

---

## ▶️ How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/cars24-used-car-analysis.git
```

### 2. Navigate to the Project

```bash
cd cars24-used-car-analysis
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate the Virtual Environment

#### Windows

```bash
venv\Scripts\activate
```

#### macOS/Linux

```bash
source venv/bin/activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

### 6. Launch Jupyter Notebook

```bash
jupyter notebook
```

Then open:

```text
notebooks/01_cars24_web_scraping.ipynb
```

for the scraping process and:

```text
notebooks/02_cars24_eda_visualization.ipynb
```

for data analysis and visualization.

---

## 📦 Requirements

The project requires the following Python libraries:

```text
pandas
numpy
matplotlib
seaborn
requests
beautifulsoup4
jupyter
```

Install them using:

```bash
pip install -r requirements.txt
```

---

## ⚠️ Disclaimer

This project was developed for **educational and data-analysis purposes**.

The dataset represents the Cars24 listings collected during the project and may not represent the current availability, prices, or inventory on the Cars24 website.

Web scraping should always be performed responsibly and in accordance with the target website's terms, policies, and applicable laws.

---

## 📄 Project Presentation

The project presentation is available in the `presentation/` folder.

It contains:

* Problem Statement
* Objectives
* Technologies Used
* Methodology
* Dataset Overview
* Area-wise Analysis
* Brand/Model-wise Analysis
* Key Insights
* Future Scope

---

## 👨‍💻 Author

### Badineni Manikanta Koushik

**Batch:** 513

* GitHub: https://github.com/koushik-badineni
* LinkedIn:https://www.linkedin.com/in/manikanta-koushik-61a935267/

---

## ⭐ If You Find This Project Useful

If you find this project helpful or interesting, consider giving the repository a ⭐ star.
