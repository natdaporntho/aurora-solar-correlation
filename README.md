# Aurora–Solar Correlation Analysis

## Correlation between Auroral Indices, Solar Indices, and Neutron Monitor Count Rates

This project investigates the correlation between **auroral activity indices** (AE, Dst, Kp), **solar activity indices** (SSN, F10.7), and **neutron monitor count rates** from multiple stations worldwide.

**Data period**: 1964–2020  
**Analysis methods**: Pearson correlation, lagged cross-correlation, hysteresis analysis across solar cycles

---

## 📁 Project Structure

```
├── data/                          # All raw data files
│   ├── OULU_*.csv                 # OULU neutron monitor (Finland)
│   ├── WWW_dstae*.dat.txt         # AE & Dst geomagnetic indices
│   ├── kpdata.txt, kpdata1964.txt # Kp, SSN, F10.7 solar indices
│   ├── WSO_polarfield.txt         # Polar magnetic field data
│   ├── apty.html, Apatity cosmic ray station2.html
│   ├── huan-nm.html               # Huancayo NM (Peru)
│   ├── jung1.html                 # Jungfraujoch NM (Switzerland)
│   ├── thulefull.html, thuleadd.html  # Thule NM (Greenland)
│   ├── psnm.csv                   # PSNM McMurdo NM (Antarctica) – processed
│   └── 03Jan01_...txt             # PSNM McMurdo NM – raw
├── notebooks/
│   └── aurora_solar_correlation.ipynb   # Main analysis notebook
├── results/                       # Generated plots & figures (PNG, SVG)
├── references/                    # Research papers (PDF)
├── .gitignore
└── README.md
```

## 📊 Data Sources

| Parameter   | Description                     | Source              |
|-------------|---------------------------------|---------------------|
| **AE**      | Auroral Electrojet Index        | WDC Kyoto           |
| **Dst**     | Disturbance Storm Time Index    | WDC Kyoto           |
| **Kp**      | Planetary K-index (3-hourly)    | GFZ Potsdam         |
| **SSN**     | Sunspot Number                  | SILSO / WDC-SILSO   |
| **F10.7**   | Solar Radio Flux (10.7 cm)      | NRC Canada          |
| **OULU**    | Neutron Monitor                 | Oulu, Finland       |
| **THUL**    | Neutron Monitor                 | Thule, Greenland    |
| **APTY**    | Neutron Monitor                 | Apatity, Russia     |
| **PSNM**    | Neutron Monitor                 | McMurdo, Antarctica |
| **JUNG1**   | Neutron Monitor                 | Jungfraujoch, Switzerland |
| **HUAN**    | Neutron Monitor                 | Huancayo, Peru      |

## 🛠️ Dependencies

- Python ≥ 3.9
- pandas, numpy, scikit-learn
- plotly, matplotlib
- beautifulsoup4

Install with:
```bash
pip install pandas numpy plotly matplotlib scikit-learn beautifulsoup4
```

## 🚀 Usage

1. Open `notebooks/aurora_solar_correlation.ipynb` in Jupyter Notebook / JupyterLab / VS Code
2. Run cells sequentially from top to bottom
3. Generated plots are saved to `results/` folder

## 📝 Notebook Sections

| Section | Description |
|---------|-------------|
| 1. Setup & Imports | Library imports and configuration |
| 2. Utility Functions | Data parsing, IQR filtering, time conversion |
| 3. Data Processing | Functions to clean each data source |
| 4. Polar Field & Cycles | Solar cycle and polar hemisphere definitions |
| 5. Data Loading | Load all datasets and merge into hourly DataFrame |
| 6. Data Validation | Sanity checks and statistics |
| 7. Correlation Functions | Pearson correlation, lagged correlation, block averaging |
| 8. Visualization | Plotting functions for time series |
| 9. Correlation Matrix | Heatmap of cross-correlations |
| 10. Lagged Correlation | Correlation vs time lag analysis |
| 11. Hysteresis Analysis | Solar cycle hysteresis loops |
| 12. Results | Pre-configured analysis cells |

---

**Author**: Natdaporn Thongphan (Natdaporn T.)  
**Institution**: Mahidol Wittayanusorn School, Nakhon Pathom, Thailand  
**Project Code**: 33E-PH03-01  
**Repo**: [natdaporntho/aurora-solar-correlation](https://github.com/natdaporntho/aurora-solar-correlation)
