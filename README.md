# 🌍 Sustainable Development Analysis with SQL

## 📌 Overview

This project analyzes global data to identify **opportunities for sustainable development**, focusing on energy, social indicators, and economic potential.

The goal is to support a **non-profit organization** in making data-driven decisions about where to allocate resources for maximum impact.

### 🎯 Key Questions

The analysis answers three main questions:

1. Where would investments in renewable energy have the greatest impact?
2. Which countries show the most critical social indicators?
3. Are there countries with strong economic potential but clear energy inefficiencies?

---

## 🗂️ Dataset Description

The project integrates two main datasets:

### 1. `global_country`

Contains demographic, economic, and social indicators such as:

* Population, density
* GDP and tax rates
* Life expectancy and mortality rates
* Education levels
* CO₂ emissions

### 2. `sustainable_energy`

Focuses on energy-related metrics:

* Access to electricity
* Renewable energy share
* Energy consumption
* CO₂ emissions
* GDP per capita and growth

---

## 🛠️ Database Structure

### Table Creation

Two tables are created:

* `global_country`
* `sustainable_energy`

### 🔗 Data Integration

The datasets are linked using a **foreign key relationship**:

```sql
ALTER TABLE sustainable_energy 
ADD CONSTRAINT fk_country 
FOREIGN KEY (country_id) REFERENCES global_country(id);
```

This allows combining social, economic, and energy indicators for deeper analysis.

---

## 🔍 Analysis Breakdown

## 1️⃣ Renewable Energy Investment Opportunities

### 🎯 Objective

Identify countries where renewable energy investments would generate the highest impact.

### 📊 Methodology

The analysis considers:

* Low access to electricity
* High CO₂ emissions
* High fertility rate
* Large population or high density
* Low share of renewable energy

### 🧠 Insight

Countries with:

* High emissions
* Low renewable adoption
  represent the **best opportunities for impactful interventions**.

---

## 2️⃣ Critical Social Indicators

### 🎯 Objective

Identify countries with the most urgent need for social development.

### 📊 Key Indicators

* Low life expectancy
* Low tertiary education enrollment
* Limited access to electricity
* High fertility rate

### 🧠 Insight

These countries are not necessarily the "worst", but those where:
➡️ **Targeted investments can significantly improve quality of life**

---

## 3️⃣ Economic Potential vs Energy Inefficiency

### 🎯 Objective

Find countries with:

* Strong economies
* Poor energy efficiency

### 📊 Methodology

* GDP per capita growth (2009–2019)
* High electricity access
* Low renewable energy share

### 🧠 Insight

These countries:

* Have the infrastructure and resources
* But are underperforming in sustainability

👉 Ideal candidates for **high-impact pilot projects**

---

## ⭐ Model Countries

A second analysis identifies countries with:

* High renewable energy adoption
* Strong education systems

Examples include:

* Uruguay
* Lithuania
* Iceland

These act as **benchmarks for successful energy transition**.

---

## 💡 Key Insights

* 🌱 Renewable energy investments are most effective in **high-emission, low-access countries**
* 📉 Social development is strongly linked to **education and electricity access**
* 📈 Economic growth does not guarantee sustainability
* 🎓 Higher education levels correlate with **better renewable energy adoption**

---

## 🚀 Technologies Used

* SQL (PostgreSQL-style queries)
* Data modeling
* CTEs (Common Table Expressions)
* Data integration & transformation

---

## 📁 Project Structure

```
/project
│── README.md
│── sql_queries.sql
│── dataset/
│── analysis_notes/
```

---

## 🤝 Use Cases

This project can be used for:

* Data analyst portfolio
* NGO strategic planning
* Sustainability research
* Policy-making support

---

## 📬 Contact

Created by **Luca Frittitta**
Feel free to connect or ask questions!

---
