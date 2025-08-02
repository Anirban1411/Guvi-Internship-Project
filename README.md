# CSV File Analyzer 📊

This project provides a Python script for performing a comprehensive Exploratory Data Analysis (EDA) on any given CSV file. The script automates the process of data loading, cleaning, analysis, and visualization, making it a versatile tool for initial data assessment.

---

## 📖 Description

The primary goal of this project is to offer a reusable and efficient tool for an initial analysis of tabular data. The script is designed to be adaptable, but the current implementation demonstrates its capabilities using the **Air Quality UCI dataset** as an example. It preprocesses the data by handling missing values and incorrect data types, and then generates key statistical summaries and visualizations.

This serves as a foundational step in any data science workflow, providing crucial insights into a dataset's structure and quality.

**Technologies Used:**
* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn

---

## ✨ Features

* **Custom Data Loading:** Reads CSV files with specified delimiters and handles custom missing value notations (e.g., `-200`).
* **Data Cleaning:** Automatically drops irrelevant columns and fills missing numerical data with the column's mean.
* **Data Profiling:** Displays total rows, columns, and data types for a quick overview.
* **Statistical Summary:** Calculates and prints descriptive statistics (mean, median, std, etc.) for all numerical features.
* **Visualization:**
    * Generates a **heatmap** to show the distribution of missing values before cleaning.
    * Creates a **bar chart** to visualize the mean values of each numerical column.

---

## 🛠️ Installation

To run this script on your local machine, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Anirban1411/Guvi-Internship-Project.git](https://github.com/Anirban1411/Guvi-Internship-Project.git)
    cd Guvi-Internship-Project
    ```

2.  **Install the required libraries:**
    ```bash
    pip install pandas numpy matplotlib seaborn
    ```

---

## 🏃‍♀️ How to Run

1.  **Download the Example Dataset:**
    Make sure you have the `AirQualityUCI.csv` file. You can download it from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/360/air+quality). To use your own data, simply change the file path.

2.  **Update File Path:**
    Open the Python script and update the `file_path` variable to the location of your CSV file.
    ```python
    # Example usage
    if __name__ == "__main__":
        file_path = 'path/to/your/AirQualityUCI.csv'  # <-- UPDATE THIS LINE
        csv_file_analyzer(file_path)
    ```

3.  **Execute the Script:**
    Run the script from your terminal.
    ```bash
    python your_script_name.py
    ```

---

## 📈 Expected Output

After running the script, you will see:
1.  **Console Output:** A detailed analysis printed directly to your terminal, including the data shape, data types, missing value counts, and summary statistics.
2.  **Two Plot Windows:**
    * A heatmap showing the initial state of missing values.
    * A bar chart comparing the mean of each numerical feature.

---

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
