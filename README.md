# Milestone 2 - PySpark Data Engineering Project

## Project Overview

This project demonstrates data processing using **Apache Spark (PySpark) on Databricks**.
The main objective is to load, explore, clean, transform, and store a real-world dataset using PySpark operations.

---

## Dataset Description

**Dataset Name:** Zomato Bangalore Restaurants Dataset

**Source:** Kaggle

**Description:**
The dataset contains details about restaurants in Bangalore such as restaurant name, location, cuisine, ratings, cost, online ordering, and table booking information.

**Dataset Link:**
(Add Kaggle dataset URL)

---

## Technologies Used

* Python
* PySpark
* Apache Spark
* Databricks
* GitHub

---

# Project Steps

## 1. Data Loading

* Uploaded the dataset to Databricks using Unity Catalog Volume.
* Read the dataset into a PySpark DataFrame.
* Used **PERMISSIVE mode** to handle possible corrupted records.

---

## 2. Data Exploration

Performed basic analysis:

* Displayed column names
* Counted total rows
* Checked schema structure
* Found the number of columns

---

## 3. Corrupted Record Checking

Checked for corrupted records using the `_corrupt_record` column.

No corrupted records were found in the dataset.

---

## 4. Schema Validation

Checked the inferred schema of the dataset.

Custom schema using `StructType` and `StructField` was created wherever required to ensure correct data types.

---

## 5. Data Transformations

Applied different PySpark transformations:

* **alias()** - Renamed columns during selection
* **filter()/where()** - Filtered required records
* **lit()** - Added constant values
* **withColumn()** - Created new columns
* **withColumnRenamed()** - Renamed columns
* **cast()** - Changed data types
* **drop()** - Removed unnecessary columns

---

## 6. Handling Null Values

* Identified missing values in the dataset.
* Handled null values using suitable methods like filling or removing records based on the requirement.

---

## 7. Removing Duplicates

Checked for duplicate records and removed them if required.

---

## 8. Saving Processed Data

The final transformed DataFrame was saved using:

* **Format:** Parquet
* **Mode:** Overwrite

Parquet was selected because it provides efficient storage and faster processing.

---

# Challenges Faced

* Handling a large dataset file while uploading to GitHub.
* Understanding and fixing data quality issues.
* Managing schema and data type corrections.

---

# Repository Structure

```
Milestone-2/
│
├── README.md
│
├── notebook/
│   └── milestone2.ipynb
│
├── Screenshots/
│   ├── pic1.png
│   ├── pic2.png
│   ├── pic3.png
│   ├── pic4.png
│   └── .....
|   |__pic26.png
│
└── .gitignore
```

---

# Conclusion

This project helped in understanding real-world data engineering workflows using PySpark and Databricks, including data loading, cleaning, transformation, and storage.
