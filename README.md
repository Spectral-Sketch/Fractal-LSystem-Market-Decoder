# Fractal Market Decoder: L-System Grammar & Reichardt Flow Analysis

## Project Overview
This repository contains a quantitative research framework designed to identify structural patterns (motifs) in financial time-series. By combining **Fractional Differentiation (FFD)** with **Adaptive L-System Grammar**, the model explores the lead-lag relationship between the S&P 500 (Equity) and Bitcoin (Crypto).

## Key Technical Features

### 1. Fractional Differentiation (FFD)
Traditional returns ($d=1$) often erase the market's memory. This engine implements **Fixed Width Window FracDiff ($d=0.2$ to $0.4$)** to achieve stationarity while preserving the fractal properties and long-term memory required for structural analysis.

### 2. Symbolic Aggregate Approximation (SAX)
Continuous price data is encoded into a discrete linguistic string (a, b, c, d) using **Adaptive Rolling Bins**. This allows the application of Natural Language Processing (NLP) logic to identify recurring market "sentences" or motifs.

### 3. Recursive L-System Parser
Inspired by the formal grammars developed by **Aristid Lindenmayer**, this engine extracts production rules from market "strings." 
* **Biological Parallel:** Just as L-Systems model the recursive growth of plants and fractals, this parser identifies self-similar growth patterns in market volatility.
* **Functionality:** It treats the S&P 500 as the "generator" of rules to predict the "growth" (next move) of Bitcoin.


### 4. Reichardt Flow Correlation
Implements a biological-inspired **Reichardt Correlator** to measure the direction of information flow. This confirms which market acts as the "Leading Indicator" (e.g., Bitcoin as the 'Canary in the Coal Mine').

## Model Validation & Bias Mitigation
A critical phase of this research involved identifying and eliminating **Look-ahead Bias**. 
* **Initial Observation:** Static quantiles yielded over-optimized hit-rates (>80%).
* **Correction:** Implemented a strictly adaptive walk-forward validation with rolling bins.
* **Result:** A statistically significant and realistic edge (~37% - 45%), proving the model's integrity for real-world regime detection.

## How to Use
1. Clone the repository.
2. Install requirements: `pip install pandas numpy yfinance matplotlib`.
3. Open `final_analysis.ipynb` to view the full research and Reichardt Flow visualizations.

---
*Developed by Spectral-Sketch | Quantitative Research*# Fractal-LSystem-Market-Decoder
