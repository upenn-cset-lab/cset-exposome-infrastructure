# Modeling Framework – C-SET Exposome Infrastructure

## 1. Purpose

This document defines the statistical and computational modeling framework used within the C-SET exposome infrastructure.

The modeling system is designed to support:

- Spatiotemporal exposure-response analysis
- Longitudinal transplant outcome modeling
- Causal inference for time-varying exposures
- High-dimensional and machine learning integration
- Scalable high-performance computing implementation

The framework is explicitly aligned with the multi-granularity data architecture and supports modeling across transplant-level, person-time, and area-level datasets.

## 2. Modeling Domains

The C-SET modeling framework is organized into four major domains:

### 2.1 Longitudinal Outcome Modeling

Models designed to evaluate associations between environmental exposures and transplant outcomes over follow-up time.

Common applications include:
- Mortality
- Graft failure
- Infection
- Cardiovascular events

---

### 2.2 Spatiotemporal Exposure-Response Modeling

Models that explicitly incorporate spatial and temporal structure of environmental exposures.

Common approaches include:
- Generalized Additive Models (GAMs)
- Spatial random effects models
- Hierarchical and multi-level models

---

### 2.3 Time-Varying and Distributed Lag Modeling

Frameworks designed to capture delayed and cumulative exposure effects.

Common approaches include:
- Distributed Lag Models (DLM)
- Distributed Lag Non-Linear Models (DLNM)
- Moving average exposure windows

---

### 2.4 Causal and Counterfactual Modeling

Approaches designed to estimate causal effects under time-varying exposures.

Common approaches include:
- Inverse Probability Weighting (IPW)
- Marginal Structural Models (MSMs)
- G-methods and counterfactual frameworks

### 2.5 Machine Learning and High-Dimensional Integration

Models designed to integrate multi-source exposures and high-dimensional biological data.

Common approaches include:
- Gradient boosting methods
- Penalized regression frameworks
- Tree-based ensemble models
- Neural network architectures (when applicable)

These models are used for:
- Risk prediction
- Exposure pattern discovery
- Feature selection in high-dimensional settings

Interpretability tools (e.g., SHAP or feature importance analysis) are incorporated to maintain clinical relevance.

## 3. Alignment with Analytical Grain

The modeling framework is explicitly aligned with supported analytical grains.

### 3.1 Transplant-Level Models
- Survival models
- Baseline covariate risk modeling
- Long-term outcome prediction

### 3.2 Person-Day / Person-Time Models
- Time-varying exposure models
- Distributed lag models
- Conditional Poisson or case-crossover designs
- Mixed-effects longitudinal models

### 3.3 ZCTA-Day / Area-Level Models
- Spatial random effects models
- Area-level exposure-response modeling
- Ecologic or multilevel frameworks

This alignment ensures that modeling strategies are selected based on the structural grain of the Standard Analysis File (SAF).

## 4. Computational Implementation

All models are implemented using modular, reproducible workflows optimized for secure high-performance computing environments.

### 4.1 Software Environment

Common tools include:
- R (primary statistical modeling environment)
- Python (machine learning and data engineering)
- Secure HPC batch systems

### 4.2 Scalable Computation

Large-scale modeling workflows are executed using:

- Parallelized model fitting
- Job-array submission strategies
- Controlled memory allocation
- Structured logging and failure handling

### 4.3 Reproducibility Controls

- All model specifications are parameterized
- Hyperparameters are explicitly documented
- Model outputs are version-linked to SAF builds
- Scripts are designed to regenerate results from source data

## 5. Model Validation and Sensitivity Analysis

Model robustness is evaluated through structured validation and sensitivity procedures.

### 5.1 Internal Validation
- Cross-validation where applicable
- Out-of-sample prediction testing
- Stability of effect estimates across specifications

### 5.2 Sensitivity Analyses
- Alternative exposure windows
- Alternative spatial aggregations
- Alternative lag structures
- Subgroup analyses

### 5.3 Diagnostic Evaluation
- Residual diagnostics
- Convergence checks
- Assessment of random effects variance components
- Evaluation of overdispersion or model misspecification

All validation procedures are documented and reproducible within the pipeline structure.
