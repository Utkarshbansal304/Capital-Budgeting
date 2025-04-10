# Capital Budgeting Model

## File Access
The model can be accessed here: [Capital Budgeting Model](https://docs.google.com/spreadsheets/d/1Vr_A171dOKhwBLp0srefiScDduR4uGoY/edit?usp=sharing&ouid=104526269926966601048&rtpof=true&sd=true)

⚠️ Important Note: Please download the file first rather than viewing in the web browser. For optimal functionality, open the spreadsheet directly in Microsoft Excel app. The file contains complex formulas that may display errors when viewed in browser.

## Overview
This repository contains a comprehensive capital budgeting model designed to evaluate energy projects' financial feasibility. The model calculates Net Present Value (NPV), Internal Rate of Return (IRR), and conducts sensitivity analysis under different scenarios (best case, base case, worst case).

## Model Structure
The Excel-based model consists of the following key components:

### Input Sheets
- **Input -->**: Entry point for model navigation
- **Drivers**: Core parameters including installed capacity, capacity factor, prices, and scenario selection

### Calculation Sheets
- **Workings**: Intermediate calculations supporting the model
- **Revenue**: Energy output and revenue projections based on installed capacity and price
- **Opex**: Operating expense calculations as a percentage of revenue
- **Fixed Asset roll-forward**: Asset depreciation and capital expenditure tracking
- **Financing**: Debt structure, repayments, and interest calculations
- **P&L**: Profit and loss statement with revenue, expenses, and taxation
- **Cash Flow**: Comprehensive cash flow projections including initial investment, operations, and financing
- **WACC**: Weighted Average Cost of Capital calculations using comparable companies

### Output Sheets
- **Output**: Summary results and key metrics
- **Discounted Cash Flows**: NPV, IRR, and time series of discounted cash flows

## Key Model Parameters

### Project Specifications
- **Installed Capacity**: 
  - Best case: 220 MW
  - Base case: 200 MW
  - Worst case: 180 MW
- **Capacity Factor**: 25%
- **Annual Operation**: 365 days, 24 hours per day
- **Energy Output Formula**: Installed capacity (MW) × Capacity factor × Days in year × Hours per day

### Financial Parameters
- **Initial Investment**: 
  - Best case: €50,000,000
  - Base case: €51,000,000
  - Worst case: €52,000,000
- **Project Lifetime**: 10 years
- **CAPEX after Year 1**: 3% of initial investment
- **Debt Financing**: €30,000,000 senior facility at 4% interest rate
- **Repayment Schedule**: Structured over 10 years with varying percentages
- **Tax Rate**: 30%
- **Residual Value**: €10,000,000

### Revenue & Expenses
- **Price per MWh**: 
  - Best case: €220
  - Base case: €210
  - Worst case: €200
- **OPEX (% of Revenue)**: 
  - Best case: -15%
  - Base case: -16%
  - Worst case: 17%
- **Inflation Rate**: 1% (for long-term projections)

### Market Parameters
- **Market Risk Premium**: 5.5%
- **Risk-free Rate**: 2.0%
- **Comparable Companies**: Analyzed for industry benchmarks and beta calculations

## How to Use the Model

1. **Setup**:
   - Download or clone this repository
   - Open the `Capital Budgeting.xlsx` file in Microsoft Excel

2. **Scenario Selection**:
   - Navigate to the "Drivers" sheet
   - Select your desired scenario (1=Best case, 2=Base case, 3=Worst case) in cell C5

3. **Parameter Adjustment** (optional):
   - Modify input parameters in the "Drivers" sheet to fit your specific project
   - Update comparable companies in the "WACC" sheet if necessary

4. **Results Interpretation**:
   - Review the "Output" sheet for summary financial metrics
   - Analyze "Discounted Cash Flows" sheet for NPV and IRR results
   - Examine cash flow projections over the project lifetime

## Model Features

- **Scenario Analysis**: Compare outcomes across best, base, and worst-case scenarios
- **Sensitivity Analysis**: Assess how changes in key parameters affect NPV and IRR
- **Financial Metrics**: Calculate NPV, IRR, payback period, and debt service coverage ratios
- **Dynamic Projections**: Automatically updates all calculations when inputs are changed
- **WACC Calculation**: Industry-standard approach to determine discount rate using market data

## Requirements
- Microsoft Excel 2016 or newer
- Basic understanding of capital budgeting concepts and financial modeling

## Contributing
Contributions to improve the model are welcome. Please feel free to submit a pull request or open an issue to discuss potential enhancements.

## Acknowledgements
This capital budgeting model was developed using industry-standard financial modeling practices and methodologies.
