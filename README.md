# COVID-19 Vaccination Analysis

## 🧾 Overview
This project analyzes COVID-19 vaccination data to compare vaccination progress in **India**, the **United Kingdom**, and **France**. The dataset is sourced from **Kaggle** ("Data on COVID19 (coronavirus)") and includes information on vaccination metrics over time.  
The analysis includes **data profiling, cleaning, and visualization** using R.

---

## ✅ Features

The project performs the following tasks:

- **Data Profiling**: Checks for missing values, zeros, data types, and unique values using `funModeling` and `Hmisc`.
- **Data Selection**: Filters data for India, the UK, and France, focusing on key vaccination metrics:
  - `total_vaccinations`
  - `people_vaccinated_per_hundred`
  - `people_fully_vaccinated_per_hundred`
- **Visualization**: Creates a line plot showing the **percentage of people vaccinated (at least one dose)** over time for the selected countries.

---

## ⚙️ Technologies Used

- R (version 4.0 or higher)
- Packages:
  - `data.table`
  - `tidyverse`
  - `funModeling`
  - `Hmisc`
  - `ggplot2`

Install them using:
```r
install.packages(c("data.table", "tidyverse", "funModeling", "Hmisc", "ggplot2"))
```

---

## 📁 Data

The dataset is sourced from Kaggle:  
👉 [Data on COVID19 (coronavirus)](https://www.kaggle.com/tunguz/data-on-covid19-coronavirus)

### Steps to Obtain the Data:

1. Visit the Kaggle dataset page.
2. Download the dataset (e.g., `owid-covid-data.csv`).
3. Rename the file to: `covid-data.csv`
4. Place it inside a `data/` folder in the project directory:  
   `data/covid-data.csv`

> ⚠️ *Note*: The dataset is not included in this repository due to size and licensing. Please download it manually from Kaggle.

---

## 📂 Directory Structure

```
covid_vaccination_analysis/
│
├── covid_vaccination_analysis.R    # Main R script
├── data/
│   └── covid-data.csv              # Dataset (download manually)
├── README.md                       # Project documentation
├── .gitignore                      # Git ignore file
└── LICENSE                         # MIT License
```

---

## 🚀 Usage

1. Clone the repository:
```bash
git clone https://github.com/[Your-Username]/covid_vaccination_analysis.git
cd covid_vaccination_analysis
```

2. Download the dataset and place it in the `data/` folder as `covid-data.csv`.

3. Open R or RStudio and set the working directory to the project folder:
```r
setwd("path/to/covid_vaccination_analysis")
```

4. Run the script:
```r
source("covid_vaccination_analysis.R")
```

### The script will:
- Load and profile the dataset
- Filter data for India, the UK, and France
- Generate a line plot showing vaccination progress

---

## 🔍 Analysis Details

### 🧮 Data Profiling
- Uses `funModeling` and `Hmisc`
- Checks:
  - Missing values
  - Zeros
  - Data types
  - Unique values

### 🔎 Data Selection
- Filters for countries: India, UK, France
- Selected columns:
  - `iso_code`
  - `location`
  - `date`
  - `total_vaccinations`
  - `people_vaccinated_per_hundred`
  - `people_fully_vaccinated_per_hundred`
- Removes rows with missing values in `people_vaccinated_per_hundred`

### 📊 Visualization
- Creates a line plot using `ggplot2`
- Compares of people vaccinated (at least one dose)** over time

---

## 📈 Example Output

The script generates a line plot titled:

> **"% of vaccinated people in India, UK, and France"**

- **X-axis**: Date  
- **Y-axis**: % of people vaccinated per hundred (at least one dose)  
- **Lines**: One for each country (color-coded)

---

## 🤝 Contributing

Contributions are welcome!  
Please fork the repository, make your changes, and submit a pull request.  
Ensure your code follows the existing style and includes comments where needed.

---

## 🧾 License

This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**[Darshan]**  
Created on **June 16, 2025**

---

## 🙏 Acknowledgments

- **Data Source**: [Kaggle - Data on COVID19 (coronavirus)](https://www.kaggle.com/tunguz/data-on-covid19-coronavirus)
- **Libraries Used**:
  - data.table
  - tidyverse
  - funModeling
  - Hmisc
  - ggplot2
