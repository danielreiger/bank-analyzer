# 🏦 Bank Health Analyzer

Python-Tool zur automatisierten Analyse von Banken auf Basis regulatorischer Kennzahlen — orientiert am FINMA / Basel III Framework.

## Was das Tool macht

1. **Ticker eingeben** — beliebige börsennotierte Bank (z.B. DBK.DE, UBSG.SW, CBK.DE)
2. **Kennzahlen berechnen** — ROE, ROA, Equity Ratio, Net Income Margin über 4 Jahre
3. **Bank Health Score** — automatisierter 0-100 Score auf Basis regulatorischer Benchmarks
4. **Excel-Export** — formatierter Report inkl. Regulatory Context

## Beispiel-Output: Deutsche Bank AG
```
Equity Ratio:      5.5%   (FINMA Minimum: 4.5%)
ROE:               8.8%   (Zielwert: >10%)
ROA:               0.48%  (Zielwert: >1.0%)

Bank Health Score:  68/100
Rating:  MODERATE ⚠️ — Some weaknesses, monitoring required
```

## Regulatorische Benchmarks

| Kennzahl | Grenzwert | Bedeutung |
|---|---|---|
| Equity Ratio | > 4.5% | Basel III Mindestanforderung |
| Equity Ratio | > 7.0% | Starker Kapitalpuffer |
| ROE | > 10% | Starke Eigenkapitalrendite |
| ROA | > 1.0% | Effizienter Vermögenseinsatz |

## Installation
```bash
pip install yfinance pandas numpy openpyxl
python bank_analyzer.py
```

## Tech-Stack
- Python 3.9+
- yfinance, pandas, numpy, openpyxl

---
*Erstellt von Daniel Reiger | Lernprojekt Assurance Advisory & Regulatory Analysis*
