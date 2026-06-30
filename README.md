# Aurora–Solar Correlation Analysis

## Correlation between Auroral Index, Solar Indices, and Neutron Monitor Count Rate

This project investigates the correlation between **auroral activity indices** (AE, Dst, Kp), **solar activity indices** (SSN, F10.7), and **neutron monitor count rates** from multiple stations worldwide.

---

## 📁 Project Structure

```
├── codes/
│   ├── aurora_solar_correlation.ipynb     # Main analysis notebook
│   ├── graphes/                            # Generated plots and figures
│   ├── WSO_polarfield.txt                  # Polar magnetic field data
│   ├── kpdata.txt, kpdata1964.txt          # Kp, SSN, F10.7 index data
│   ├── OULU_*.csv                          # OULU neutron monitor data
│   ├── WWW_dstae*.dat.txt                  # AE and Dst index data
│   ├── apty.html, Apatity cosmic ray station2.html
│   ├── huan-nm.html                        # Huancayo NM data
│   ├── jung1.html                          # Jungfraujoch NM data
│   ├── thulefull.html, thuleadd.html       # Thule NM data
│   └── psnm.csv                            # PSNM (McMurdo) NM data
├── references/                             # Research papers (PDF)
├── .gitignore
└── README.md
```

## 📊 Data Sources

| Parameter | Description | Station / Source |
|-----------|-------------|------------------|
| **AE** | Auroral Electrojet Index | WDC Kyoto |
| **Dst** | Disturbance Storm Time Index | WDC Kyoto |
| **Kp** | Planetary K-index | GFZ Potsdam |
| **SSN** | Sunspot Number | SILSO / WDC-SILSO |
| **F10.7** | Solar Radio Flux (10.7 cm) | NRC Canada |
| **OULU** | Neutron Monitor | Oulu, Finland |
| **THUL** | Neutron Monitor | Thule, Greenland |
| **APTY** | Neutron Monitor | Apatity, Russia |
| **PSNM** | Neutron Monitor | McMurdo, Antarctica |
| **JUNG1** | Neutron Monitor | Jungfraujoch, Switzerland |
| **HUAN** | Neutron Monitor | Huancayo, Peru |

## 🛠️ Dependencies

- Python 3.x
- pandas
- numpy
- plotly
- matplotlib
- scikit-learn
- beautifulsoup4

## 🚀 Usage

Open `codes/aurora_solar_correlation.ipynb` in Jupyter Notebook or VS Code and run cells sequentially.

## 📝 Analysis Methods

- Pearson correlation analysis
- Lagged cross-correlation
- Hysteresis analysis across solar cycles
- Block averaging for long-term trends
- IQR outlier filtering
- Polar magnetic field cycle segmentation

---

**Author**: Natdaporn Thongʻʻ  
**Project**: 33E-PH03-01
