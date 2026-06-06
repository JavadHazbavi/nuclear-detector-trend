# Voltage vs Counts Analysis

This project analyzes the relationship between applied voltage and detector count rate using Python.

## Overview

The code performs the following tasks:

- Plots experimental count data as a function of voltage.
- Visualizes trends in detector response.
- Applies linear regression using NumPy's `polyfit`.
- Calculates the coefficient of determination (R²).
- Displays fitted trendlines together with experimental data.

## Requirements

Install the required packages:

```bash
pip install numpy matplotlib
```

## Project Structure

### 1. Basic Data Visualization

Plots the measured counts versus voltage.

### 2. Linear Trendline Fitting

Uses a first-order polynomial fit:

\[
y = mx + b
\]

where:

- \(y\) = counts
- \(x\) = voltage
- \(m\) = slope
- \(b\) = intercept

### 3. R² Calculation

The coefficient of determination is calculated as:

\[
R^2 = 1 - \frac{SS_{res}}{SS_{tot}}
\]

where:

- \(SS_{res}\) = residual sum of squares
- \(SS_{tot}\) = total sum of squares

## Example Dataset

| Voltage (V) | Counts |
|------------|---------|
| 420 | 27306 |
| 440 | 28239 |
| 460 | 29110 |
| 480 | 29384 |
| 500 | 30192 |
| 520 | 30636 |
| 540 | 31311 |
| 560 | 31589 |
| 580 | 32113 |
| 600 | 32433 |

## Output

The program generates:

- Count vs Voltage plots
- Linear regression trendline
- Regression equation
- R² value

Example output:

```text
Slope = 28.77
Intercept = 15340.50
R² = 0.99
```

## Technologies Used

- Python 3
- NumPy
- Matplotlib

## Applications

This project can be used for:

- Radiation detector characterization
- Geiger-Müller tube analysis
- Plateau region studies
- Experimental physics data analysis
- Detector calibration

## Author

- Shaqayeq Nezami
- Javad Hazbavi