# London Building Stock Model Dataset

## Overview
The **London Building Stock Model** dataset provides detailed information on the characteristics, energy performance, and sustainability of buildings across Greater London. The dataset is part of the **Greater London Authority’s (GLA) initiative** to improve energy efficiency, support decarbonisation efforts, and guide policy decisions related to the built environment.

- **Data Source:** Greater London Authority (GLA) – London DataStore  
- **Coverage:** All buildings across Greater London  
- **Primary Purpose:**
  - Assess energy efficiency and carbon footprint of London’s buildings  
  - Identify trends in building stock characteristics  
  - Provide insights for energy conservation, retrofitting, and urban planning  
- **Update Frequency:** Periodically updated based on new data collection efforts.

---

## Key Features of the Dataset
The dataset contains multiple fields describing each building's characteristics, energy performance, and location.

### **A. Geographical Identifiers**
| **Column Name** | **Description** |
|---------------|----------------|
| **MSOA** | Middle Layer Super Output Area – a geographical region used for statistical purposes. |
| **OAC** | Output Area Classification – categorisation of areas based on demographic and socio-economic features. |
| **WARD_CODE** | Unique identifier for each ward in London. |
| **WARD** | Name of the London ward. |
| **ADMINISTRATIVE_AREA** | The administrative region covering the building (e.g., borough or district). |

### **B. Building Characteristics**
| **Column Name** | **Description** |
|----------------|---------------|
| **ESTIMATED_FLOOR_COUNT** | Estimated number of floors in the building. |
| **ESTIMATE_TOTAL_FLOOR_AREA_ALL** | Total estimated floor area of the building (m²). |
| **SCU_FOOTPRINT** | Site coverage footprint – an estimate of the building's ground-level area. |
| **MEAN_OBJECT_HEIGHT_M** | Mean height of the building (meters). |
| **BASEMENT_FLOOR** | Indicates whether the building has a basement (Yes/No or Count). |

### **C. Building Usage and Activity**
| **Column Name** | **Description** |
|----------------|---------------|
| **COUNT_D_UPRNS** | Count of Domestic Unique Property Reference Numbers (UPRNs). |
| **COUNT_ND_UPRNS** | Count of Non-Domestic UPRNs. |
| **MIX_CLASS** | Indicates if the building is mixed-use (residential + commercial). |
| **DOMINANT_ND_ACTIVITY_BY_C2_FS** | Primary non-domestic activity type based on C2 functional sector classification. |
| **DOMINANT_ND_ACTIVITY_BY_C2_COUNT** | Count of non-domestic properties by dominant C2 classification. |

### **D. Energy Performance Data (DEC & EPC Ratings)**
| **Column Name** | **Description** |
|----------------|---------------|
| **DEC_COUNT** | Number of Display Energy Certificates (DECs) associated with the building. |
| **AGG_DEC_CURRENT_OPERATIONAL_RATING_BY_COUNT** | Aggregated operational energy rating based on count of DEC certificates. |
| **AGG_DEC_CURRENT_OPERATIONAL_RATING_BAND_BY_COUNT** | Operational energy efficiency rating band (A-G). |
| **AGG_DEC_CURRENT_OPERATIONAL_RATING_BY_FLOORAREA** | Operational rating adjusted by floor area. |
| **AGG_DEC_CURRENT_OPERATIONAL_RATING_BAND_BY_FLOORAREA** | Operational energy band considering total floor area. |

### **E. Energy Performance Certificates (EPC Ratings)**
| **Column Name** | **Description** |
|----------------|---------------|
| **EPC_RATING_COUNT_DOM** | Count of EPC ratings for domestic buildings. |
| **EPC_RATING_COUNT_NONDOM** | Count of EPC ratings for non-domestic buildings. |
| **AGG_EPC_CURRENT_ENERGY_EFFICIENCY_BY_COUNT** | Aggregated energy efficiency score from EPCs (current state). |
| **AGG_EPC_CURRENT_ENERGY_RATING_BY_COUNT** | Aggregated EPC rating (A-G) for all properties in the dataset. |
| **AGG_EPC_CURRENT_ENERGY_EFFICIENCY_BY_FLOORAREA** | EPC energy efficiency score adjusted by floor area. |
| **AGG_EPC_CURRENT_ENERGY_RATING_BY_FLOORAREA** | EPC rating (A-G) weighted by total floor area. |
| **AGG_EPC_POTENTIAL_ENERGY_EFFICIENCY_BY_COUNT** | Potential EPC energy efficiency rating if retrofits are applied. |
| **AGG_EPC_POTENTIAL_ENERGY_RATING_BY_COUNT** | Potential EPC rating (A-G) for all properties. |
| **AGG_EPC_POTENTIAL_ENERGY_EFFICIENCY_BY_FLOORAREA** | Potential EPC efficiency score considering floor area. |
| **AGG_EPC_POTENTIAL_ENERGY_RATING_BY_FLOORAREA** | Potential EPC rating (A-G) weighted by total floor area. |

### **F. Renewable Energy & Retrofitting Potential**
| **Column Name** | **Description** |
|----------------|---------------|
| **AGG_RVEPC_CURRENT_ENERGY_EFFICIENCY_BY_COUNT** | Current renewable energy efficiency rating (aggregated). |
| **AGG_RVEPC_CURRENT_ENERGY_RATING_BY_COUNT** | Aggregated renewable energy efficiency band (A-G). |
| **AGG_RVEPC_CURRENT_ENERGY_EFFICIENCY_BY_FLOORAREA** | Renewable energy efficiency metric adjusted for floor area. |
| **AGG_RVEPC_CURRENT_ENERGY_RATING_BY_FLOORAREA** | Renewable energy rating (A-G) adjusted for floor area. |

---

## Key Insights & Analysis Opportunities
### **1. Energy Efficiency & Carbon Footprint**
- How do EPC and DEC ratings vary across different London boroughs?
- What is the relationship between building height, size, and energy performance?
- Which boroughs have the highest concentration of inefficient buildings?

### **2. Retrofitting & Sustainability**
- Which buildings have the greatest potential for energy efficiency improvements?
- What is the estimated cost vs. savings potential for retrofitting?
- How do EPC ratings compare between domestic and non-domestic properties?

### **3. Spatial Analysis & Urban Planning**
- How does energy efficiency vary across different administrative areas?
- Can we identify clusters of energy-inefficient buildings that need priority intervention?
- How do EPC and renewable energy indicators correlate with socio-economic conditions in London?

---

## Next Steps
1. **Load the Dataset** – Start by opening the dataset in Pandas and exploring column values.
2. **Data Cleaning** – Handle missing values, inconsistencies, and data formatting issues.
3. **Exploratory Data Analysis (EDA)** – Generate summary statistics and initial visualisations.
4. **Feature Engineering** – Create new features like `Building Age`, `EPC Improvement Potential`, etc.
5. **Geospatial Analysis** – Use mapping techniques to visualise energy efficiency across boroughs.
6. **Predictive Modelling** (Optional) – Build models to forecast energy performance improvements.

---

## Conclusion
The **London Building Stock Model** dataset provides a wealth of information for analysing the energy efficiency and carbon footprint of London’s buildings. By understanding the dataset’s structure and potential applications, we can derive insights that support decarbonisation policies, promote sustainable building practices, and guide targeted retrofitting initiatives.
