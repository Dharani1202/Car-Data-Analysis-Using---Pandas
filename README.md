# Cars Dataset Analysis Project

## Project Overview

* The **Cars Dataset Analysis Project** focuses on analyzing car-related data to extract insights about **make, origin, drivetrain, and engine specifications**.
* The project covers **data cleaning, filtering, and transformation** using Python and Pandas.
* It demonstrates techniques for handling **null values, conditional filtering, and column transformations** in a dataset.

🔗 <a href="https://github.com/Dharani1202/Car-Data-Analysis-Using---Pandas/blob/main/Cars%20Project_1.ipynb"> View the Project </a>

---

## Objective

* To clean and preprocess the Cars dataset.
* To perform analysis on car **makes, origins, wheelbase, engine size, drivetrain, and MPG**.
* To answer specific business questions related to car specifications and attributes.

---

## Tools and Libraries Used

* **Python**
* **Pandas** – for data cleaning and analysis
* **NumPy** – for numerical operations

---

## Steps and Tasks Performed

### ## Data Preprocessing

* Removed all **null values** to ensure clean data for analysis.

  ```python
  df.dropna(inplace=True)
  ```
* Checked dataset info using `.info()` and `.describe()` to understand column types and statistics.

---

### ## Exploratory Data Analysis (EDA) & Filtering

1. **Different types of make in the dataset and their counts**

   * Used `.value_counts()` to count the number of records for each car **make**.

2. **Show all records where origin is Asia or Europe**

   * Filtered dataset using:

     ```python
     df[(df['Origin'] == 'Asia') | (df['Origin'] == 'Europe')]
     ```

3. **Remove all records where weight is above 4000**

   * Filtered dataset using:

     ```python
     df = df[df['Weight'] <= 4000]
     ```

4. **Increase all values in MPG_City column by 3**

   * Performed transformation:

     ```python
     df['MPG_City'] = df['MPG_City'] + 3
     ```

5. **Show the wheelbase of 105.0 in the origin of Asia**

   * Filtered dataset:

     ```python
     df[(df['Wheelbase'] == 105.0) & (df['Origin'] == 'Asia')]
     ```

6. **Show all different types of drivetrain and their counts**

   * Used `.value_counts()` on **Drivetrain** column to see distribution.

7. **Show wheelbase of 105, cylinder equal to 6.0, and engine size 3.0**

   * Filtered dataset:

     ```python
     df[(df['Wheelbase'] == 105.0) & (df['Cylinders'] == 6.0) & (df['Engine_size'] == 3.0)]
     ```

---

## Insights Gained

* Identified the **most common car makes** and distribution by **origin**.
* Observed **weight trends** and filtered out heavy vehicles above 4000 lbs.
* Enhanced MPG values for city driving to understand performance changes.
* Explored drivetrain types and engine-wheelbase combinations for targeted analysis.

---

## Conclusion

* This project provides a **complete workflow for cleaning, filtering, and analyzing car dataset attributes**.
* It demonstrates how to handle **missing data, apply conditional filtering, and transform columns** for better insights.
* The techniques applied can be used for other automotive datasets or similar structured data projects.

---

🔗 <a href="https://github.com/Dharani1202/Car-Data-Analysis-Using---Pandas/blob/main/Cars%20Project_1.ipynb"> View the Project </a>

---

