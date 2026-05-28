# 📊 Data Jobs Dashboard — Power BI

An interactive Power BI dashboard exploring the data jobs market — covering salaries, job counts, hiring platforms, work-from-home trends, and global distribution across data roles.

---

## 🖥️ Dashboard Overview

The report consists of **2 pages**:

### Page 1 — Data Jobs Dashboard
The main overview page with high-level KPIs and trend analysis.

| Visual | Description |
|--------|-------------|
| 🔢 KPI Cards | Job title count, avg yearly salary, avg hourly salary, salary star rating |
| 📊 Bar Chart | Job counts by title |
| 📈 Line Chart | Job postings over time (by Year / Quarter / Month) |
| 💠 Scatter Chart | Hourly vs. yearly salary comparison by job title |
| 📋 Pivot Table | Job stats — title, quarter, avg salary |
| 🎛️ Slicer | Filter all visuals by job title |

### Page 2 — Job Title Drill Through
A drill-through detail page — click any job title on Page 1 to explore it in depth.

| Visual | Description |
|--------|-------------|
| ⏱️ Gauge | Avg / Min / Max yearly salary |
| ⏱️ Gauge | Avg / Min / Max hourly salary |
| 🍩 Donut Chart | Work-from-home (%) breakdown |
| 🥧 Pie Chart | No degree mention (%) |
| 🍩 Donut Chart | Health insurance offered (%) |
| 🗺️ Map | Global job distribution by country |
| 🌳 Treemap | Job schedule types (full-time, contract, etc.) |
| 📊 Bar Chart | Job postings by hiring platform |

---

## 🗂️ Data Source

All visuals are powered by a single flat table: **`job_postings_flat`**

| Column | Description |
|--------|-------------|
| `job_title_short` | Shortened job title (e.g., Data Analyst, Data Engineer) |
| `salary_year_avg` | Average yearly salary (USD) |
| `salary_hour_avg` | Average hourly salary (USD) |
| `job_posted_date` | Date the job was posted |
| `job_work_from_home` | Whether the role is remote |
| `job_no_degree_mention` | Whether a degree is mentioned as required |
| `job_health_insurance` | Whether health insurance is offered |
| `job_country` | Country where the job is located |
| `job_via` | Platform/source of the job posting |
| `job_schedule_type` | Employment type (full-time, part-time, contract, etc.) |
| `Salary Star Rating` | Custom calculated column/measure for salary rating |

---

## 🚀 Getting Started

### Prerequisites
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free) — required to open `.pbix` files.

### Steps
1. Clone or download this repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   ```
2. Open **Power BI Desktop**.
3. Go to **File → Open report → Browse** and select `Data_Jobs_Dashboard.pbix`.
4. The dashboard will load with all visuals and data embedded.

> **Note:** The data is embedded directly in the `.pbix` file — no external database connection is needed.

---

## 💡 How to Use

- Use the **Job Title slicer** on Page 1 to filter all visuals by role.
- **Right-click any job title** in the bar chart or pivot table and select **Drill Through → Job Title Drill Through** to open the detail page for that role.
- Use the **back button** (top-left of Page 2) to return to the main dashboard.

---

## 📁 File Structure

```
📦 repository-root
 ┣ 📊 Data_Jobs_Dashboard.pbix   # Power BI report file
 ┗ 📄 README.md                  # Project documentation
```

---

## 🛠️ Built With

- [Microsoft Power BI Desktop](https://powerbi.microsoft.com/) — data visualization
- DAX — calculated measures and columns
- Power Query (M) — data transformation

---

## 📌 Notes

- Salary figures are in **USD**.
- Job posting data covers multiple years with quarterly/monthly drill-down available.
- The global map visual requires an internet connection in Power BI to render Bing Maps tiles.


