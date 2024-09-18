# Portfolio-Optimization

This project focuses on constructing an optimal stock portfolio that balances the trade-off between risk and return, while comparing different investment strategies. The approach leverages tools like Pandas, NumPy, Seaborn for data manipulation and visualization, and Pyomo with the IPOPT solver for optimization. Historical stock price data was collected for 30 tickers from three sectors, covering January 1, 2017, to December 31, 2021. The 'adjclose' prices were used to build a dataframe 'prep_data' for analysis. After cleaning the data, an Exploratory Data Analysis (EDA) was conducted to visualize time series stock values by sector. Momentum Trading was employed to identify the top 3 performing stocks from each sector based on moving average crossovers.

The goal was to allocate funds into these selected stocks to maximize expected return, factoring in risk tolerance and constraints. Momentum Trading helped identify the most suitable strategy for each stock. A final evaluation was performed on a $100K investment using different strategies.

Sectors and Selected Stocks:
Energy Sector: TRGP (Targa Resources Corp), FANG (Diamondback Energy, Inc), MRO (Marathon Oil Corporation)
Finance Sector: BX (The Blackstone Group Inc.), HIG (The Hartford Financial Services Group, Inc.), MET (MetLife, Inc.)
Materials Sector: NUE (Nucor Corporation), STLD (Steel Dynamics, Inc.), SHW (Sherwin-Williams Company)
Portfolio Allocation Across Risk Levels:

![image](https://github.com/user-attachments/assets/999df213-872e-41e5-b9a4-4f921d823bd5)

The "Optimal Stock Allocation for Different Risk Levels" graph shows how portfolio allocation shifts across nine different stocks as risk increases. Notably, 'BX' (red line) sees a significant rise in its share at higher risk levels, indicating its potential as a high-risk, high-reward option. On the other hand, 'SHW' (yellow line) decreases in allocation with higher risk, making it a safer option for low-risk portfolios. Other stocks exhibit steadier allocations, suggesting a balanced role regardless of risk levels. This visualization is essential for aligning portfolio allocations with investor risk preferences.

Efficient Frontier:

![image](https://github.com/user-attachments/assets/15bf3370-2d20-4459-87ba-a43e3c6673af)

The efficient frontier graph visualizes the trade-off between risk and return for various portfolio allocations. The x-axis represents risk (measured as standard deviation), ranging from approximately 0.00025 to above 0.00045, while the y-axis represents the expected return, spanning from just above 0.0012 to around 0.0016. This curve highlights the maximum expected return for each level of risk, guiding investors toward an optimal balance.
