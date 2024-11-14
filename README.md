# Medical-DNA-Analyzer👨‍⚕️🧬🩺❤
A Python-based tool for simplified DNA analysis focused on medical applications, making it practical for doctors and healthcare providers to analyze genetic data in the context of various medical conditions..

## Overview

This tool allows the analysis of DNA sequences to detect common disease-associated mutations, genetic risk factors, and drug metabolism profiles. It generates clinical reports and visual summaries to aid in healthcare decision-making. The tool is designed to provide healthcare professionals with actionable insights derived from DNA sequences.

## Features

**Mutation Detection:** Identifies common mutations associated with diseases like Breast Cancer, Cystic Fibrosis, and Lynch Syndrome.

**Risk Factor Analysis:** Assesses genetic risk for cardiovascular diseases, Type 2 diabetes, Alzheimer's, and more.

**Drug Metabolism Profiling:** Analyzes genes related to drug metabolism, including CYP2D6, CYP2C19, and TPMT.

**Clinical Report Generation:** Automatically compiles a clinical report with findings and recommendations.

**Visualization:** Generates plots to visualize detected mutations, risk levels, and drug metabolism profiles.

## Installation

**Prerequisites**

Ensure Python 3.x is installed on your machine. The tool relies on the following Python packages:

**pandas

numpy

matplotlib

seaborn

biopython**

Install the dependencies by running the following command:

```bash
pip install -r requirements.txt
 ```
## Steps to Set Up
Clone the repository:

```bash
git clone https://github.com/yourusername/Medical-DNA-Analyzer.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Usage
**Initialize the Analyzer**

Create an instance of the `MedicalDNAAnalyzer` class by providing a DNA sequence string:
```python
from MedicalDNAAnalyzer import MedicalDNAAnalyzer

# Example DNA sequence
sequence = "ATGCGTGTAGCTAGCGTAAAGTCGGTAGCTAGCTGCTGTTACG"

analyzer = MedicalDNAAnalyzer(sequence)
```

**Analyze the Sequence**

Check for mutations:
```python
mutations = analyzer.check_mutations()
print(mutations)
```

Analyze genetic risk factors:
```python
risk_factors = analyzer.analyze_risk_factors()
print(risk_factors)
```

Analyze drug metabolism:
```python
drug_metabolism = analyzer.check_drug_metabolism()
print(drug_metabolism)
```

Generate a clinical report:
```python
report = analyzer.generate_clinical_report()
print(report)
```

Visualize the findings:
```python
analyzer.visualize_findings()
```

Print clinical summary:
```python
analyzer.print_clinical_summary()
```
## Example
```python
# DNA sequence example
sequence = "ATGCGTGTAGCTAGCGTAAAGTCGGTAGCTAGCTGCTGTTACG"

# Initialize the analyzer
analyzer = MedicalDNAAnalyzer(sequence)

# Generate and print a clinical summary
analyzer.print_clinical_summary()

# Visualize the findings
analyzer.visualize_findings()
```

## Output
**Clinical Report:** A detailed report summarizing mutations, risk factors, and drug metabolism findings with actionable recommendations.

**Visualizations:** Graphical representations of detected mutations, risk levels, and metabolism profiles using Seaborn and Matplotlib.
