
# 📱 Smartphones SQL Case Study  

## 📖 Project Overview  
This project is a **SQL-based case study on smartphones dataset**.  
The goal is to analyze **smartphone brands, models, pricing, RAM, storage, and market insights** using SQL queries.  

Through this case study, I explored how SQL can be used to extract **meaningful business insights** from raw data.  

---

## 🛠️ Tech Stack  
- **Database:** MySQL  
- **Tools:** MySQL Workbench / SQL Server / PostgreSQL (any RDBMS works)  
- **Dataset:** Custom Smartphones Dataset (Brand, Model, Price, RAM, Storage, Battery, etc.)  

---

## 🔑 Key Queries & Insights  

### 1️⃣ Data Exploration  
```sql
SELECT * FROM smartphones LIMIT 10;
````

➡️ Get a quick overview of the dataset.

### 2️⃣ Top 5 Smartphones with Highest RAM & Storage

```sql
SELECT brand, model, ram_gb, storage_gb 
FROM smartphones 
ORDER BY ram_gb DESC, storage_gb DESC 
LIMIT 5;
```

📊 **Insight:** Shows the most powerful smartphones.

### 3️⃣ Average Price by Brand

```sql
SELECT brand, AVG(price) AS avg_price 
FROM smartphones 
GROUP BY brand 
ORDER BY avg_price DESC;
```

💡 **Insight:** Identifies premium vs budget-friendly brands.

### 4️⃣ Most Affordable 5G Smartphones

```sql
SELECT brand, model, price 
FROM smartphones 
WHERE network = '5G' 
ORDER BY price ASC 
LIMIT 5;
```

📱 **Insight:** Highlights budget 5G options.

### 5️⃣ Count of Models by Each Brand

```sql
SELECT brand, COUNT(model) AS total_models 
FROM smartphones 
GROUP BY brand 
ORDER BY total_models DESC;
```

📊 **Insight:** Reveals the most diverse product line-up.

---

## 📈 Business Use Cases

✔️ Helps customers compare smartphones before buying
✔️ Assists retailers in **identifying top-selling specs & price ranges**
✔️ Useful for analysts to study **brand positioning & market trends**

---

## ✨ Key Learnings

* Writing **SQL queries for real-world scenarios**
* Using **aggregation, filtering, ordering, and subqueries**
* Transforming **raw smartphone data into actionable insights**

---

## 🚀 Future Scope

* Create **interactive dashboards** (Excel / Power BI / Tableau)
* Apply **Window Functions & CTEs** for deeper analysis
* Expand dataset with **customer reviews & sales data**

---

## 📌 Author

👤 **Piyush Singh**
💼 Aspiring **Data Analyst** | SQL | Excel | Power BI | Tableau
