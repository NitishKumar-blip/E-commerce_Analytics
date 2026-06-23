#📦 E-commerce_Analytics
Finding the best route possible base on the efficiency score and  average route lead time.


## 📌 Project Overview
The **E-Commerce Analytics Dashboard** is a Power BI project designed to analyze shipping performance, route efficiency, delivery delays, and transportation trends in an e-commerce supply chain. The dashboard helps businesses monitor logistics KPIs and identify opportunities to improve delivery operations.

---

## 🎯 Objectives
- Monitor shipping lead times across different routes.
- Measure route efficiency and identify underperforming locations.
- Track delivery delays and delay frequency.
- Compare shipping modes based on lead time and efficiency.
- Support data-driven logistics decision-making.

---

## 🛠️ Tools & Technologies
- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Power Query**
- **Microsoft Excel / CSV Dataset**
- **Data Modeling**

---

## 📊 Dashboard Features

### 1. Shipping Lead Time
Displays the total shipping lead time across all orders.

**Current Value:** 11.3M

---

### 2. Average Lead Time
Shows the average time required for order delivery.

**Current Value:** 1.32K

---

### 3. Route Volume Analysis
Visualizes shipment distribution across routes and cities.

**Insights:**
- Identifies high-volume shipping routes.
- Helps optimize transportation planning.

---

### 4. Delay Frequency
Measures the percentage of delayed deliveries.

**Current Value:** 33.3%

**Formula:**
```DAX
Delay Frequency =
DIVIDE(
    COUNTROWS(FILTER(Orders, Orders[Delayed] = 1)),
    COUNTROWS(Orders)
)
```
5. Route Efficiency Score

Evaluates route performance using lead time and delay metrics.

Current Value: 0.61

Sample Formula:

Route Efficiency Score =
(1 - [Delay Frequency]) *
(1 - ([Average Lead Time] / [Maximum Lead Time]))
6. High Efficiency Cities

Displays cities with the best route efficiency scores.

Examples:

1.Kenner
2.Rock Hill
3.Southfield
4.Hickory
5.Apopka

7. Low Efficiency Cities

Highlights cities requiring logistics improvements.

Examples:

1.Port Arthur
2.3.The Colony
Lansing
4.Greenville
5.Bryan

8. Average Route Lead Time by City

Ranks cities according to average shipping lead time.

Top Cities:

1.Rock Hill
2.San Marcos
3.Mason
4.Billings
5.Portage

9. Ship Mode Analysis

Compares shipping methods:

First Class , 
Same Day , 
Second Class , 
Standard Class

Metrics:

1.Lead Time by Ship Mode
2.Efficiency Score by Ship Mode

📈 Key Performance Indicators (KPIs)

KPI	Description :

1.Shipping Lead Time	Total delivery duration
2.Average Lead Time	Average delivery duration
3.Delay Frequency	Percentage of delayed orders
4.Route Efficiency Score	Logistics performance index
5.Route Volume	Number of shipments per route


🚀 Business Benefits
1.Reduces delivery delays.
2.Improves route planning.
3.Enhances customer satisfaction.
4.Optimizes transportation costs.
5.Enables performance monitoring through real-time insights.

## 📸 Dashboard Preview
![E-Commerce Analytics Dashboard](Snapshot.png)
