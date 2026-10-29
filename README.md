
# agricultural-residue-bioenergy-bangladesh

# Assessment of Agricultural Residue Availability, Bioenergy, and Electricity Potential in Bangladesh (2017–2024)

This repository contains a comprehensive data-driven assessment framework for quantifying crop production trends, gross agricultural residues, recoverable dry biomass, and thermal bioenergy/electricity generation potential in Bangladesh from 2017 to 2024 using official [FAOSTAT data portal](https://www.fao.org/faostat/?utm_source=chatgpt.com) metrics.


## 🌾 1. Research Overview & Scope
- **Study Period:** 2017–2024
- **Target Crops & Residues:**
  1. **Rice** $\rightarrow$ Rice straw & Rice husk
  2. **Maize (corn)** $\rightarrow$ Maize stover
  3. **Sugarcane** $\rightarrow$ Sugarcane bagasse
- **Key Parameters:** Residue-to-Product Ratios (RPR), Recovery Fractions, Moisture Content, and Lower Heating Values (LHV) gathered from peer-reviewed literature (*Yevich & Logan, 2003*).

---

## 📊 2. Data Tables & Findings

### Table 1: Annual Crop Production in Bangladesh (2017–2024)
| Year | Maize (tonnes) | Rice (tonnes) | Sugar cane (tonnes) |
| :--- | :--- | :--- | :--- |
| **2017** | 3,025,392.00 | 52,079,606.96 | 3,862,775.00 |
| **2018** | 3,288,102.00 | 54,614,714.97 | 3,638,731.00 |
| **2019** | 3,569,321.00 | 54,784,186.92 | 3,141,923.00 |
| **2020** | 4,015,306.00 | 56,056,815.18 | 3,682,951.00 |
| **2021** | 4,116,438.00 | 56,772,472.25 | 3,332,546.00 |
| **2022** | 4,261,845.00 | 57,776,021.60 | 3,087,428.00 |
| **2023** | 4,592,507.00 | 60,601,180.62 | 2,982,546.00 |
| **2024** | 4,592,508.00 | 60,570,453.05 | 2,933,694.00 |

---

### Table 2: Crop Production Growth & Change Summary (2017 vs 2024)
| Crop | First Year | Production in First Year (t) | Last Year | Production in Last Year (t) | Absolute Change (t) | Percentage Change (%) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Maize** | 2017 | 3,025,392.00 | 2024 | 4,592,508.00 | +1,567,116.00 | +51.80% |
| **Rice** | 2017 | 52,079,606.96 | 2024 | 60,570,453.05 | +8,490,846.09 | +16.30% |
| **Sugar cane** | 2017 | 3,862,775.00 | 2024 | 2,933,694.00 | -929,081.00 | -24.05% |

---

### Table 3: Literature-Based Gross Residue Scenario Estimates (2024)
| Residue | Gross Residue Low (t) | Gross Residue Central (t) | Gross Residue High (t) |
| :--- | :--- | :--- | :--- |
| **Rice straw** | 48,456,362.00 | 90,855,680.00 | 151,426,133.00 |
| **Rice husk** | 10,296,977.00 | 12,114,091.00 | 13,325,500.00 |
| **Maize stover** | 4,133,257.00 | 9,185,016.00 | 18,370,032.00 |
| **Sugarcane bagasse** | 146,685.00 | 440,054.00 | 586,739.00 |

---

### Table 4: Master Summary Table (2024 Baseline Results)
| Agricultural Residue | Crop Production (t) | Gross Residue (t) | Recoverable Dry Mass (t) | Energy Potential (PJ) | Electricity Potential (GWh) | Avg. Capacity (MW) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Rice straw** | 60,570,453.05 | 90,855,679.57 | 30,890,931.06 | 463,363.97 | 25,742,648.49 | 2,938,658.50 |
| **Rice husk** | 60,570,453.05 | 12,114,090.61 | 9,812,413.39 | 142,279.99 | 7,904,507.36 | 902,341.02 |
| **Maize stover** | 4,592,508.00 | 9,185,016.00 | 2,732,542.26 | 46,453.22 | 2,580,755.00 | 294,606.74 |
| **Sugarcane bagasse** | 2,933,694.00 | 440,054.10 | 187,022.99 | 3,272.90 | 181,829.36 | 20,756.78 |

*(Note: Electricity potential is modeled based on a 20% thermal-to-electric conversion efficiency via direct thermal combustion).*

---

## 📈 3. Visual Graphs & Trends
*(Download your generated plots from Colab, place them in an `outputs/figures/` folder, and link them below)*

### A. Annual Crop Production Trends
```markdown
<img width="889" height="490" alt="download (30)" src="https://github.com/user-attachments/assets/7f4b48ef-5ed7-49bb-b198-66aebb7be8d4" />

```

### B. Gross Residue Scenarios (Low, Central, High)

```markdown
![Gross Residue Scenarios](outputs/figures/gross_residue_scenarios.png)

```

### C. Potential Annual Electricity Generation

```markdown
![Electricity Generation Potential](outputs/figures/electricity_generation_potential.png)


## 🛠️ 4. Methodology Flow Chart


[FAOSTAT Raw Data (2017–2024)]
              │
              ▼
    [Data Cleaning & Filtering] 
      (Bangladesh | Production)
              │
              ▼
   [Crop Production Analysis]
     (Trends & % Growth)
              │
              ▼
   [Literature-Based RPR & Scenarios]
     (Low / Central / High RPR)
              │
              ▼
[Gross & Recoverable Biomass Calculation]
     (Moisture & Recovery Factors)
              │
              ▼
  [Energy & Electricity Estimation]
    (LHV & 20% Conversion Efficiency)
              │
              ▼
     [Exported Master CSVs & Graphs]


## 📁 5. Repository Contents & Exported Datasets

* **`notebooks/`**: Contains the complete Google Colab python code notebook (`Assessment of Agricultural Residue.ipynb`).
* **`outputs/figures/`**: Contains generated trend and scenario graphs.
* **`data/`**: Cleaned CSV outputs and master summary reports:
* `bangladesh_crop_production_clean.csv`
* `annual_crop_production_table.csv`
* `crop_production_change_summary.csv`
* `gross_biomass_scenario_estimates.csv`
* `recoverable_biomass_energy_potential_2024.csv`
* `electricity_generation_potential_2024.csv`
* `master_biomass_energy_summary_2024.csv`




## 👤 Author

**Md. Abdul Malek**

Department of Agricultural and Industrial Engineering

Hajee Mohammad Danesh Science and Technology University (HSTU)

```

```
