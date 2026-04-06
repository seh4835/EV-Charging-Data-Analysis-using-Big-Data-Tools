# ⚡ EV Charging Data Analysis using Big Data Ecosystem

## 📌 Overview
This project presents an **end-to-end Big Data pipeline** for analyzing Electric Vehicle (EV) charging data. It integrates multiple technologies from the Hadoop ecosystem along with real-time streaming and visualization tools to extract meaningful insights from large-scale data.

The system processes **~500K+ records with 30+ features**, covering energy consumption, charging behavior, efficiency, time patterns, and geographical distribution.

---

## 🎯 Objectives
- Analyze EV charging behavior and usage trends  
- Perform distributed data processing on large datasets  
- Implement both **batch and real-time data pipelines**  
- Visualize insights through an interactive dashboard  

---

## 🛠️ Tech Stack

| Layer | Technology |
|------|-----------|
| Storage | HDFS |
| Processing | MapReduce, PySpark |
| Querying | Hive |
| ETL | Pig |
| Data Integration | Sqoop (MySQL ↔ Hadoop) |
| NoSQL | HBase |
| Streaming | Kafka |
| Real-Time DB | Cassandra |
| Visualization | Power BI |
| UI | Hue |

---

## 📊 Dataset
- **Type:** Structured CSV  
- **Size:** ~500,000+ records  
- **Attributes:** 30+ columns  

### Key Features:
- `energy_kwh`
- `charging_efficiency`
- `city`, `country`
- `charging_time_sec`
- `hour`, `month`
- `port_type`

---

## 🧱 Architecture
CSV Dataset
↓
HDFS (Storage)
↓
MapReduce / Hive / Pig (Batch Processing)
↓
PySpark (Fast Processing)
↓
Kafka (Streaming)
↓
Cassandra (Real-Time Storage)
↓
Power BI (Visualization)


---

## ⚙️ Implementation Details

### 🔹 HDFS
- Stored large dataset in distributed environment  
- Managed file system operations using HDFS commands  

### 🔹 MapReduce
- Implemented custom programs to compute:
  - Energy consumption by city  
  - Energy consumption by country  
  - Average charging efficiency per user  

### 🔹 Hive
- Created structured tables from CSV  
- Performed SQL-based analytics:
  - Total energy consumption  
  - Monthly trends  
  - Peak charging hours  

### 🔹 PySpark
- Used DataFrames for efficient processing  
- Performed aggregation and transformations  
- Achieved faster execution compared to MapReduce  

### 🔹 Pig
- Used Pig Latin for ETL operations  
- Performed filtering, grouping, and aggregation  

### 🔹 Sqoop
- Imported data from MySQL into Hadoop ecosystem  
- Exported structured data into Hive  

### 🔹 HBase
- Designed column-family schema  
- Enabled real-time read/write operations  

### 🔹 Kafka
- Simulated real-time EV charging data streaming  

### 🔹 Cassandra
- Stored streaming data for scalable querying  

### 🔹 Hue
- Used web UI for:
  - Query execution  
  - Monitoring jobs  
  - Managing HDFS  

---

## 📈 Power BI Dashboard

The final dashboard includes:

- ⚡ Total Energy Consumption  
- 📊 Total Sessions & Revenue  
- 📈 Monthly Trends  
- 🕒 Peak Charging Hours  
- 🔌 Port Type Distribution  
- 📍 City-wise Energy Analysis  
- ⚙️ Energy vs Charging Time (Correlation)  

---

## 🔍 Key Insights

- High energy consumption concentrated in specific urban locations  
- Peak charging activity observed during mid-day hours  
- Strong correlation between charging time and energy usage  
- Majority of sessions exhibit high charging efficiency  
- Real-time pipeline supports scalable EV infrastructure analysis  

---

## 🚀 Results

- Built a **scalable big data pipeline**  
- Integrated **batch + real-time processing**  
- Delivered **actionable insights via visualization**  

---

## 📂 Project Structure


/data
└── EV_Cleaned_Data.csv

/hadoop
├── hdfs_commands.txt
├── hive_queries.sql
├── pig_scripts.pig

/mapreduce
├── mapper1.py
├── reducer1.py
├── mapper2.py
├── reducer2.py

/spark
└── pyspark_analysis.py

/dashboard
└── powerbi.pbix

/streaming
├── kafka_producer.py
├── kafka_consumer.py

/README.md


---

## 🧠 Learnings

- Hands-on experience with full Hadoop ecosystem  
- Understanding of distributed storage and processing  
- Implementation of real-time data pipelines  
- Data visualization and storytelling  

---

## 📌 Future Improvements

- Deploy pipeline on cloud (AWS / Azure)  
- Integrate real-time dashboards  
- Apply machine learning for prediction  

---
## 👤 Author
**Seher Sanghani**
Big Data | Data Analytics | Data Engineering  

---

⭐ If you found this project useful, consider giving it a star!
