# 🚀 GenAI Sales Analytics Chatbot (Microsoft Fabric)

## 📌 Overview
This project demonstrates a GenAI-powered chatbot built on Microsoft Fabric that enables users to query sales data using natural language. The chatbot converts user questions into Spark SQL queries, executes them on Lakehouse data, and returns real-time insights.

---

## 🧠 Key Features
- Natural Language → SQL conversion using OpenAI
- Spark SQL execution on Fabric Lakehouse
- Optimized unified fact table for better performance
- Safe query generation with a validation layer
- Scalable data processing using PySpark

---

## 🏗️ Architecture
User Question
↓
OpenAI (LLM)
↓
SQL Query Generation
↓
Spark SQL Execution
↓
Fabric Lakehouse (Delta Tables)
↓
Result Output


---

## 🛠️ Tech Stack

- Microsoft Fabric (Lakehouse, Semantic Model)
- PySpark
- Spark SQL
- OpenAI API
- Delta Lake

---

## 📊 Data Model

- AdventureWorks Dataset (2019–2022)
- Star Schema Design
- Unified Fact Table: `fact_sales_combined_tbl`

---

## ⚙️ How It Works

1. User enters a natural language query  
2. OpenAI converts it into Spark SQL  
3. SQL is validated and cleaned  
4. Spark executes a query on Lakehouse  
5. Results are displayed  

---

## 💬 Example Queries

- Total sales by sales type  
- Sales trend by year  
- Top products by revenue  
- Compare internet vs reseller sales  

---

## 🔐 Security & Validation

- Blocked unsafe SQL operations (DROP, DELETE, etc.)
- Cleaned LLM-generated SQL (removed markdown)
- API key handled using environment variables

---

## 📁 Project Structure
genai-fabric-sales-chatbot/
│
├── notebooks/
│ └── chatbot_notebook.ipynb
│
├── src/
│ ├── generate_sql.py
│ ├── utils.py
│
├── screenshots/
│ ├── output.png
│
├── README.md
├── requirements.txt
└── .gitignore


---

## ⚙️ Setup Instructions

1. Clone the repository  
2. Install dependencies: pip install -r requirements.txt
3. Set OpenAI API key: export OPENAI_API_KEY=your_key
4. Run notebook in Microsoft Fabric  

---

## 🚀 Future Enhancements

- Streamlit UI for chatbot interface  
- Power BI integration  
- Role-based access control  
- Chat history (memory)  

---

## 🎯 Impact

Enabled self-service analytics by allowing users to query data using natural language, reducing dependency on manual reporting.

---

## 👨‍💻 Author
Keshav Lakhpati
