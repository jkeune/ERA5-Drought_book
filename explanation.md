# Background: Understanding Drought Indices

Drought is a complex phenomenon — it develops slowly, varies across regions, and affects different parts of the water cycle in different ways.  
Before diving deeper into ERA5-Drought, it helps to understand the **indices** we use to quantify drought and why they matter.

This page gives a short overview of two of the most widely used climate-based drought indicators: **SPI** and **SPEI**, as well as broader drought types (meteorological, agricultural, hydrological).  
For deeper reading, we link to authoritative sources such as the **World Meteorological Organization (WMO)**, the **European Drought Observatory (EDO)**, and the **Global Drought Observatory (GDO)**.

---

## Why drought indices?

Raw precipitation values alone don’t tell us whether a region is experiencing drought — is 50 mm of rainfall in a month “normal,” “too little,” or “a lot”?  
To answer such questions, drought indices compare current conditions to typical long-term patterns and express **how unusual** they are.

Drought indices help us:
- Compare regions with very different climates  
- Detect emerging drought early  
- Monitor severity and persistence  
- Support decision-making in agriculture, water management, and risk assessment  

ERA5-Drought focuses on climate-based indices that rely on long records of reanalysis data.

---

## The Standardized Precipitation Index (SPI)

The **Standardized Precipitation Index (SPI)** (McKee et al., 1993) is one of the simplest and most widely used drought indicators.

**What it measures:**  
SPI quantifies precipitation anomalies over a chosen accumulation period relative to a long-term climatology.

Common accumulation periods:
- **SPI-1** → short-term meteorological dryness  
- **SPI-3** → seasonal impacts  
- **SPI-12** → long-term hydrological stress  

**Interpretation (WMO, 2012):**

| SPI value      | Interpretation        |
|----------------|------------------------|
| > 2.0          | Extremely wet          |
| 1.5–1.99       | Very wet               |
| 1.0–1.49       | Moderately wet         |
| -0.99–0.99     | Near normal            |
| -1.0–-1.49     | Moderately dry         |
| -1.5–-1.99     | Severely dry           |
| < -2.0         | Extremely dry          |

**Strengths**
- Simple, robust  
- Requires only precipitation  
- Comparable across climates  

**Limitations**
- Does **not** consider temperature or evaporative demand  

---

## The Standardized Precipitation–Evapotranspiration Index (SPEI)

The **SPEI** (Vicente-Serrano et al., 2010) extends SPI by including temperature-driven **evaporative demand**, which is especially relevant under climate warming.

**What it measures:**  
It uses a simple climatic water balance:

> **Water balance = Precipitation – Potential Evapotranspiration (PET)**

Hotter conditions increase PET, lowering the water balance even when rainfall is unchanged — SPEI captures this effect.

**Advantages**
- Accounts for temperature effects  
- Sensitive to heat-driven drought intensification  
- Flexible timescales (1–48 months)

**Limitations**
- Requires PET estimation (method-dependent)  
- Slightly more complex than SPI  

---

## How ERA5-Drought uses these indices

ERA5-Drought provides **monthly global SPI and SPEI** derived from ERA5 and ERA5T reanalysis.  
All indices use a reference climatology (typically 1991–2020), ensuring spatial consistency.

This makes ERA5-Drought suitable for:
- Global drought monitoring  
- Sectoral applications  
- Early-warning systems  
- Research and education  

---

## Types of drought: meteorological, agricultural, and hydrological

Drought is not a single concept—it evolves across different parts of the water cycle.  
Understanding the major drought types helps interpret what SPI and SPEI can (and cannot) capture.

---

### Meteorological drought

**Definition:**  
A period of significantly below-normal precipitation (Gibbs & Maher, 1967).

**Where it occurs:**  
In the **atmosphere** — expressed in rainfall anomalies.

**Indicators:**  
- SPI  
- SPEI  
- Percentiles  

**Timescale:** Weeks to months  
**Significance:** First stage of drought development.

---

### Agricultural (soil moisture) drought

**Definition:**  
Insufficient soil moisture to meet vegetation or crop needs (FAO, 2013).

**Where it occurs:**  
**Root zone and surface soils**

**Indicators:**  
- Soil moisture anomalies  
- Evaporative Stress Index (ESI)  
- NDVI/vegetation indices  
- SPEI (via temperature sensitivity)

**Timescale:** Weeks to months  
**Impacts:** Crop failures, vegetation stress, fire risk.

---

### Hydrological drought

**Definition:**  
Long-term deficits in **streamflow, groundwater, lakes, or reservoirs** (Van Loon, 2015).

**Where it occurs:**  
The **deep water cycle**

**Indicators:**  
- River discharge  
- Groundwater levels  
- Reservoir storage  

**Timescale:** Months to years  
**Impacts:** Water supply, navigation, hydropower, ecosystems.

---

### How drought types relate

Meteorological drought can trigger agricultural drought, which can eventually trigger hydrological drought — but the pathway is not guaranteed:

- Heatwaves can cause agricultural drought without a rainfall deficit  
- Irrigation may prevent agricultural drought  
- Hydrological drought often persists long after rain returns  

**SPI** → Best for meteorological drought  
**SPEI** → Connects meteorological ↔ agricultural drought  
**Long timescales (SPI-12, SPEI-12)** → Early signals of hydrological drought  

---

## Further reading and authoritative sources

### Scientific and methodological references
- WMO (2012). *Standardized Precipitation Index User Guide.*  
- McKee, T. B., Doesken, N. J., & Kleist, J. (1993). *The relationship of drought frequency and duration to time scales.*  
- Vicente-Serrano, S. M., Beguería, S., & López-Moreno, J. I. (2010). *A multiscalar drought index sensitive to global warming.*  

### Operational drought monitoring
- **Global Drought Observatory (GDO)**: https://edo.jrc.ec.europa.eu/gdo  
- **European Drought Observatory (EDO)**: https://edo.jrc.ec.europa.eu/  

These platforms provide real-time maps, long-term records, and multiple drought indicators.

---

## Summary

SPI and SPEI are core indices for understanding climate-based drought.  
Knowing the difference between meteorological, agricultural, and hydrological drought provides essential context for interpreting the ERA5-Drought dataset.

---

## References

- FAO (2013). *Agricultural Drought.*  
- Gibbs, W. J., & Maher, J. V. (1967). *Rainfall deciles as drought indicators.*  
- McKee, T. B., Doesken, N. J., & Kleist, J. (1993). *The relationship of drought frequency and duration to time scales.*  
- Van Loon, A. F. (2015). *Hydrological drought explained.*  
- Vicente-Serrano, S. M., Beguería, S., & López-Moreno, J. I. (2010). *SPEI: A new global drought index.*  
- WMO (2012). *Standardized Precipitation Index User Guide.*  

