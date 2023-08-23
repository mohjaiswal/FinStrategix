# Financial Planning Report

## Introduction

This report outlines the work undertaken in a financial planning project aimed at assisting members of a credit union in enhancing their financial health. The project involves the development of two financial analysis tools to help users assess their personal finances and forecast retirement plans. The report provides an overview of the project's background, objectives, methodologies, and outcomes.

![Financial Planner](Images/financial-planner.png)

## Project Background

The project is centered around a FinTech consultancy firm's initiative to create impactful solutions for local communities. The first client is a major credit union, which seeks to empower its members with tools for evaluating monthly personal finances and projecting retirement plans. The consultancy is tasked with developing prototype applications to showcase during the upcoming credit union assembly.

## Objectives

The primary objectives of this project are as follows:

1. **Personal Finance Planner:** Create an application allowing users to visualize their savings in shares and cryptocurrencies to assess if they have an adequate emergency fund.

2. **Retirement Planning Tool:** Develop a tool that employs historical data to project the performance of a retirement portfolio composed of stocks and bonds over a 30-year period.

## Methodology

### Personal Finance Planner

The first part of the project focuses on the creation of a personal finance planner application. Assumptions for this segment include:

- Average household income per member: $12,000.
- Crypto assets: `1.2` BTC and `5.3` ETH.
- Shares in stocks and bonds: `50` SPY (stocks) and `200` AGG (bonds).

The `requests` library is used to fetch the current prices of bitcoin (`BTC`) and ethereum (`ETH`) in Canadian dollars (`CAD`) through the **Alternative Free Crypto API**. The obtained crypto prices are used to calculate the portfolio value of cryptocurrencies.

### Retirement Planning Tool

The second part of the project involves a retirement planning tool. The steps taken are as follows:

1. Historical closing prices for `SPY` (stocks) and `AGG` (bonds) are fetched using the **Alpaca Markets API** to create a 40/60 portfolio.
2. A Monte Carlo Simulation with 500 runs and 30 years is executed to project portfolio performance.
3. The simulation results, including probability distributions and confidence intervals, are visualized.

## Findings

### Personal Finance Planner

- The computed portfolio value of cryptocurrencies allows users to assess their savings.
- If the total savings exceed the emergency fund requirement (three times monthly income), users are congratulated.
- Users reaching the emergency fund goal or falling short by a certain amount are provided appropriate messages.

### Retirement Planning Tool

- The Monte Carlo simulation provides insights into the potential performance of a retirement portfolio.
- Simulated outcomes are used to calculate expected portfolio returns at different confidence intervals.
- The visualization of simulation results aids in understanding the range of potential outcomes.

## Conclusion

The financial planning project successfully achieved its objectives of creating user-friendly tools for assessing personal finances and projecting retirement plans. By utilizing APIs, historical data, and simulation techniques, the consultancy firm has demonstrated its capabilities in offering valuable financial solutions. The tools empower credit union members to make informed decisions about their financial health and retirement goals.

---
**Author:** Moh Jaiswal  
**Date:** 23/08/23
