# 🛒 Market Basket Analysis using SON Algorithm with PySpark

This project implements a scalable **Market Basket Analysis** using the **SON (Savasere, Omiecinski, and Navathe)** algorithm, powered by **Apache Spark** and written in **Python**. It is designed to analyze large transaction datasets to identify frequent itemsets (association rules) across distributed systems using **MapReduce architecture**.

## 📌 Project Overview

This analysis focuses on transaction data (such as procurement logs, purchase records, or trade data). The SON algorithm is used to efficiently mine frequent itemsets by dividing the dataset into smaller chunks and applying the **Apriori algorithm** in a distributed manner.

The project is particularly relevant for large-scale procurement analysis, such as data provided by international financial institutions like the **Asian Development Bank (ADB)**.

---

## ⚙️ Technologies Used

- **Python**
- **Apache Spark (PySpark)**
- **Hadoop Distributed File System (HDFS)**
- **MapReduce**
- **CSV Data Processing**

---

## 📁 Project Structure

```plaintext
.
├── son_market_basket_analysis.py   # Main script implementing SON algorithm
├── data/                           # Directory for input datasets
├── output/                         # Directory for generated results
├── README.md                       # This file

3. Run the script
bash
Copy
Edit
spark-submit son_market_basket_analysis.py <case> <input_file.csv> <support>
Arguments:
<case>: 1 or 2, defines how input is grouped.

<input_file.csv>: Path to your input CSV file.

<support>: Minimum support threshold for frequent itemsets.
