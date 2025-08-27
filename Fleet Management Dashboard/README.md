# Fleet Management Dashboard

Monitor and analyze fleet performance in Tableau. The dashboard surfaces real-time insights on **utilization**, **availability**, and **operational status** with filters for **Branch ID**, **Target Date**, and **Hour**.

---

## 📊 KPI Definitions & Formulas

**1) Utilized Count**  
Number of vehicles currently in use (actively assigned/operated).

**2) Available Count**  
Number of vehicles in working condition and ready for use but not currently assigned.

**3) Out of Service**  
Number of vehicles unavailable due to maintenance, breakdown, or other issues.

**4) Total Operational**  
Vehicles in working condition (sum of utilized and available).  
`Total Operational = Utilized Count + Available Count`

**5) Total Fleet**  
All vehicles tracked by the branch (operational + out of service).  
`Total Fleet = Utilized Count + Available Count + Out of Service`

**6) Availability Rate (%)**  
Share of the fleet that is available for use.  
`Availability Rate (%) = (Available Count / Total Fleet) * 100`

**7) Utilization Rate (%)**  
Share of the fleet currently in use.  
`Utilization Rate (%) = (Utilized Count / Total Fleet) * 100`

**8) Out of Service Rate (%)**  
Share of the fleet not available due to issues.  
`Out of Service Rate (%) = (Out of Service / Total Fleet) * 100`

> **Note:** If `Total Fleet = 0`, display rates as `0%` (avoid divide-by-zero).

**9) Utilization Trend (24 Hours)**  
Line plot showing hourly utilization over a 24-hour window to reveal peak/off-peak usage.

---