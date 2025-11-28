# Explanations

# Background: Understanding Drought Indices

Drought is a complex phenomenon — it develops slowly, varies across regions, and affects different parts of the water cycle in different ways.  
Before diving deeper into ERA5-Drought, it helps to understand the **indices** we use to quantify drought and why they matter.

This page gives a short overview of two of the most widely used climate-based drought indicators: **SPI** and **SPEI**.  
At the end, you’ll find links to authoritative resources such as the **European Drought Observatory (EDO)** and the **Global Drought Observatory (GDO)** for further reading.

---

## Why drought indices?

Raw precipitation values alone don’t tell us whether a region is experiencing drought — is 50 mm of rainfall in a month “normal,” “too little,” or “a lot”?  
To answer such questions, drought indices compare current conditions to typical long-term patterns and express **how unusual** they are.

Drought indices help us:
- Compare regions with very different climates  
- Detect emerging drought early  
- Monitor severity and persistence  
- Support decision-making in agriculture, water management, and risk assessment  

ERA5-Drought focuses on climate-based indices that rely on long meteorological records.

---

## The Standardized Precipitation Index (SPI)

The **Standardized Precipitation Index (SPI)** is one of the simplest and most widely used drought indicators.

**What it measures:**  
SPI quantifies precipitation anomalies (deficits and surpluses) over a given accumulation period relative to a long-term historical baseline.

**Examples of common accumulation periods:**
- **SPI-1** → last 1 month (short-term meteorological dryness)
- **SPI-3** → last 3 months (seasonal drought)
- **SPI-12** → last 12 months (longer-term hydrological impacts)

**How SPI is interpreted:**  
Values are standardized, meaning they express *how many standard deviations* the current precipitation level deviates from normal conditions.

| SPI value      | Interpretation        |
|----------------|------------------------|
| > 2.0          | Extremely wet          |
| 1.5–1.99       | Very wet               |
| 1.0–1.49       | Moderately wet         |
| -0.99–0.99     | Near normal            |
| -1.0–-1.49     | Moderately dry         |
| -1.5–-1.99     | Severely dry           |
| < -2.0         | Extremely dry          |

**Strengths of SPI**
- Simple and robust  
- Requires only precipitation  
- Flexible across timescales  

**Limitations**
- Does **not** consider temperature or evaporative demand  

---

## The Standardized Precipitation–Evapotranspiration Index (SPEI)

The **SPEI** extends SPI by including **temperature-driven evaporative demand**, which is crucial in a warming climate.

**What it measures:**  
SPEI is based on the climatic water balance:

> **Water balance = Precipitation – Potential Evapotranspiration (PET)**

Hotter conditions increase PET, meaning land dries faster even if rainfall stays the same. SPEI captures this mechanism, making it useful for understanding drought in warm or rapidly warming regions.

**Advantages of SPEI**
- Accounts for temperature effects  
- More sensitive to heat-driven drought intensification  
- Also available at multiple accumulation periods (SPEI-1, SPEI-3, SPEI-12, …)

**Limitations**
- Requires estimating PET, which introduces methodological choices  
- Slightly more complex to compute than SPI  

---

## How ERA5-Drought uses these indices

ERA5-Drought provides **globally consistent, monthly SPI and SPEI estimates** derived from ERA5 and ERA5T data.  
All indices are computed relative to a reference climatology (typically 1991–2020), ensuring global comparability.

This makes ERA5-Drought suitable for:
- Global monitoring  
- Regional risk assessment  
- Early warning systems  
- Research and teaching  

---

## Further reading and authoritative resources

### Drought indices
- **SPI (WMO guidelines):**  
  https://library.wmo.int/idurl/4/51520  
- **SPEI (original methodology papers):**  
  https://spei.csic.es/

### Operational drought monitoring
- **Global Drought Observatory (GDO):**  
  https://edo.jrc.ec.europa.eu/gdo  
- **European Drought Observatory (EDO):**  
  https://edo.jrc.ec.europa.eu/  

These platforms offer real-time maps, historical context, and additional drought indicators.  
They are excellent reference points for understanding how climate-based drought monitoring is used operationally around the world.

---

## Summary

SPI and SPEI are foundational tools for drought monitoring.  
- **SPI** assesses precipitation anomalies.  
- **SPEI** extends this with temperature-driven evapotranspiration.  
Together, they give us a powerful lens to understand changing drought conditions — especially when combined with global, high-resolution datasets such as **ERA5-Drought**.

