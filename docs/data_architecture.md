# Data Architecture – C-SET Exposome Infrastructure

## 1. Purpose
**(YOU FILL)** One paragraph describing the purpose of the data architecture (what problems it solves and for whom).

## 2. High-Level Data Flow
**(YOU FILL)** A 5–8 step bullet flow describing how data move from raw sources → linked exposures → analysis-ready SAFs → modeling outputs.

## 3. Data Layers
### 3.1 Clinical Layer
**(YOU FILL)** List the clinical sources used (e.g., USRDS components, claims, EHR) and the unit of analysis.

### 3.2 Environmental Exposure Layer
**(YOU FILL)** List exposure sources (e.g., USHAP, PRISM) and how they are aligned to time and geography.

### 3.3 Spatial Linkage Layer
**(YOU FILL)** List geographies and crosswalk resources (ZCTA, ZIP, county, shapefiles, crosswalks).

### 3.4 Contextual Indices Layer
**(YOU FILL)** List indices (e.g., CVI) and how they are joined (geography + time).

## 4. Linkage Keys and Grain
**(YOU FILL)** Specify the core linkage keys (e.g., patient_id, transplant_date, ZCTA, date) and the “grain” (person-day, ZCTA-day, person-week, etc.).

## 5. Standard Analysis Files (SAFs)
**(YOU FILL)** Define what SAFs exist (names) and what each SAF is used for.

## 6. Data Quality and Validation
**(YOU FILL)** List validation checks (e.g., missingness, range checks, join completeness, duplicate detection).

## 7. Security and Compliance
**(YOU FILL)** Short statement on secure storage and restricted data handling.

## 8. Versioning and Reproducibility
**(YOU FILL)** How data builds are versioned (dates/tags), and how pipelines ensure reproducibility.

