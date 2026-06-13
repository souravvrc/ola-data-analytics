🚖 Ola Rides Analytics — Power BI Dashboard

An interactive Power BI dashboard analyzing Ola cab ride data for July 2024, covering booking trends, revenue performance, cancellation patterns, vehicle type breakdown, and customer & driver ratings.

---

## 📊 Dashboard Preview

| Overall View | Vehicle Type View |
|---|---|
| Ride volume trends & booking status breakdown | Top vehicle types by distance & booking value |

| Revenue View | Cancellation View | Ratings View |
|---|---|---|
| Payment methods & top customers | Cancel reasons by customer & driver | Driver & customer ratings per vehicle |

---

## 📋 Dashboard Views & Visualizations

The report is split into **5 pages** in Power BI:

### 1. 📈 Overall
| Visual | Description |
|--------|-------------|
| **Ride Volume Over Time** | Daily count of Booking IDs across July 2024 |
| **Booking Status Breakdown** | Pie chart — Success, Cancelled by Driver, Cancelled by Customer, Driver Not Found |

> **Key Stats:** ~79.99K total bookings · ₹27M total booking value

**Booking Status Split:**
- ✅ Success — 62.04% (49.63K)
- ❌ Cancelled by Customer — 17.92% (14.39K)
- ❌ Cancelled by Driver — 10.17% (8.13K)
- ⚠️ Driver Not Found — 9.68% (7.0K)

---

### 2. 🚗 Vehicle Type
| Visual | Description |
|--------|-------------|
| **Vehicle Performance Table** | Total Booking Value, Success Booking Value, Avg. Distance, Total Distance per vehicle type |

| Vehicle | Total Booking Value | Success Value | Avg. Distance | Total Distance |
|---------|-------------------|---------------|---------------|----------------|
| Prime Sedan | 4.91M | 3.07M | 25.05 km | 138K |
| Prime SUV | 4.63M | 2.86M | 24.88 km | 131K |
| Prime Plus | 4.70M | 2.91M | 25.16 km | 132K |
| Mini | 4.64M | 2.82M | 24.98 km | 131K |
| Auto | 4.70M | 2.93M | 10.02 km | 54K |
| Bike | 4.59M | 2.91M | 25.17 km | 135K |
| E-Bike | 4.77M | 2.93M | 25.27 km | 135K |

---

### 3. 💰 Revenue
| Visual | Description |
|--------|-------------|
| **Revenue by Payment Method** | Bar chart — Cash, UPI, Credit Card, Debit Card |
| **Top 5 Customers by Total Booking Value** | Table of highest-spending customer IDs |
| **Ride Distance Distribution Per Day** | Daily sum of ride distances across the month |

**Top 5 Customers (Total spend: ₹25,469):**
| Customer ID | Booking Value |
|-------------|--------------|
| CID974848 | 5,107 |
| CID933539 | 5,314 |
| CID785112 | 5,081 |
| CID588543 | 5,007 |
| CID455502 | 4,960 |

---

### 4. ❌ Cancellation
| Visual | Description |
|--------|-------------|
| **Cancelled Rides Reasons (Customer)** | Pie chart of why customers cancelled |
| **Cancelled Rides Reasons (Driver)** | Pie chart of why drivers cancelled |

> **Total bookings:** 99.95K · **Successful:** 62.05K · **Cancelled:** 28.07K · **Cancellation Rate:** 28.09%

**Customer Cancellation Reasons:**
- Driver is not moving toward pickup — 30.3%
- Wrong Address — 25.39%
- Change of plans — 23.85%
- AC is not working — 14.87%
- Driver asked to cancel — 5.6%

**Driver Cancellation Reasons:**
- Personal & car related issue — 35.48%
- More than permitted people — 29.34%
- Customer was coughing/sick — 19.86%
- Customer related issue — 15.32%

---

### 5. ⭐ Ratings
| Visual | Description |
|--------|-------------|
| **Customer Ratings** | Average customer rating per vehicle type |
| **Driver Ratings** | Average driver rating per vehicle type |

| Vehicle | Customer Rating | Driver Rating |
|---------|----------------|---------------|
| Prime Sedan | 4.00 | 3.99 |
| Prime SUV | 4.00 | 4.01 |
| Prime Plus | 4.01 | 4.00 |
| Mini | 4.00 | 3.99 |
| Auto | 4.00 | 4.00 |
| Bike | 3.99 | 3.98 |
| E-Bike | 3.99 | 4.01 |

---

## 🗂️ Project Structure

```
ola-powerbi-dashboard/
│
├── olacabs.pbix                        # Power BI report file
├── oladata.xlsx                        # Raw ride data (source dataset)
├── oladashboard.pdf                    # Exported dashboard screenshots
├── classification_of_diff_dash.txt     # View/page classification notes
└── README.md                           # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
- Microsoft Excel (to view/edit the raw data)

### Setup

1. **Clone or download the repository**
   ```bash
   git clone https://github.com/souravvrc/ola-data-analytics.git
   ```

2. **Open the report**
   - Launch **Power BI Desktop**
   - Open `olacabs.pbix`

3. **Refresh data** *(if needed)*
   - Go to **Home → Transform Data → Data Source Settings**
   - Update the path to `oladata.xlsx` if it has moved
   - Click **Refresh**

---

## 💡 Key Insights

- 🏆 **E-Bike** has the highest average distance per ride (25.27 km) and highest total booking value (4.77M)
- 💳 **UPI and Cash** are the dominant payment methods
- ⚠️ Nearly **1 in 3 rides is cancelled** (28.09% cancellation rate)
- 🚫 The top customer cancellation reason is *"Driver not moving toward pickup"* — a fleet management signal
- ⭐ Ratings are consistently high (~4.0) across all vehicle types for both drivers and customers

---

## 🛠️ Tech Stack

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

| Tool | Role |
|------|------|
| **Power BI Desktop** | Dashboard creation, DAX measures, data modelling |
| **Microsoft Excel** | Source data storage and preprocessing |

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

> *Built to demonstrate real-world Business Intelligence and data visualization skills using Power BI.*
