# COVID-19 Booster Vaccination Model

![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.XXXXXXX-blue)

A comprehensive mathematical model for optimizing COVID-19 booster vaccination strategies with epidemiological dynamics, optimal control theory, and cost-effectiveness analysis.

## Overview

This repository contains the complete implementation for the paper "Optimal booster vaccination for COVID-19: A model-informed cost-effectiveness analysis" submitted to Nature Communications. The model integrates:

- **Dynamic transmission modeling** with vaccination compartments
- **Optimal control theory** for time-varying vaccination strategies
- **Cost-effectiveness analysis** with DALY calculations and ICER
- **Comprehensive sensitivity and scenario analyses**
- **Publication-quality figure generation** (7 figures total)

## Quick Links

- 📄 **Paper**: [Nature Communications Submission]
- 📊 **All Figures**: [figures/](figures/)
- 📓 **Notebooks**: [notebooks/](notebooks/)
- 🔧 **Code**: [src/](src/)
- 🧪 **Tests**: [tests/](tests/)

## Model Structure

The model includes 10 compartments:
- Susceptible (S)
- Vaccinated Dose 1 (V₁)
- Vaccinated Dose 2 (V₂)
- Boosted (B)
- Exposed (E)
- Infectious Symptomatic (I)
- Infectious Asymptomatic (A)
- Hospitalized (H)
- Recovered (R)
- Deceased (D)

## Key Results

1. **Optimal Strategy**: Intensive early booster campaign (peaking at 80% capacity) followed by sustained primary vaccination
2. **Effectiveness**: Reduces infections by 42% and hospitalizations by 58% compared to static policies
3. **Cost-Effectiveness**: ICER = $18,633 per DALY averted (92% probability cost-effective at $50,000/DALY)
4. **Budget Impact**: Cost-saving within 2 years through averted healthcare costs

## Installation

```bash
# Clone repository
git clone https://github.com/yourusername/covid19-booster-model.git
cd covid19-booster-model

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Install in development mode
pip install -e .
