# Denmark Electricity Production Analysis (2005–2024)

This repository contains an SQLite-based analysis of Denmark’s electricity production and consumption from **2005 to 2024**.  
The dataset (`dk_annual_energy.csv`) includes annual values for gross production, net production, central/public power stations, industrial autoproducers, wind (onshore & offshore), hydro, and solar photovoltaic.

The goal of this project is to demonstrate **SQL data analysis skills** while uncovering insights into Denmark’s energy transition, especially the growth of renewable sources.

---

## 📂 Repository Structure

- `dk_annual_energy.csv` → Clean dataset (semicolon-separated)
- `analysis.sql` → SQL queries for analysis
- `README.md` → Documentation and insights

---

## 📊 Dataset Columns

- `year`
- `gross_production`
- `use_of_electricity_in_electricity_generation`
- `net_prod_total`
- `central_power_stations`
- `public_power_stations`
- `industrial_autoproducers`
- `total_wind_turbines`
- `thereof_offshore_wind_turbines`
- `hydro_power`
- `solar_photovoltaic`

---

## 🔎 Analyses Performed

### 1. Net Production Trend Over Time
```sql
SELECT year, net_prod_total
FROM dk_annual_energy
ORDER BY year;
