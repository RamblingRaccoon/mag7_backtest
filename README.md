# Magnificent 7 Backtesting

This repository contains the code for a backtesting software to evaluate the performance of the Magnificent 7 (Mag-7).

## Project Structure

The project is organized into the following directories and files:

- `src/`: Contains Python scripts for analysis and implementation.
- `README.md`: Provides an overview of the project.
- `requirements.txt`: Includes necessary packages and imports to run the scripts in this project.

## Files

- `back_test.ipynb`, `strat_backtest.py`: Jupyter Notebook / Python scripts with back tests for our Liquidity Provider (LP) strategy on Uniswap V3.
- `model_selection.py`, `model_forecast.py`: Python scripts for specific functionalities or modules.

## Usage

To run the project or execute scripts, follow these steps:

1. Clone this repository:

   ```bash
   git clone https://github.com/DarrellNgKK/truuuu.git
   cd truuuu
   ```

2. Install the required dependencies:

   - Ensure Python is installed.
   - Use `pip` to install necessary packages listed in `requirements.txt`.

3. Explore the files:

   - `back_test.ipynb` and `strat_backtest.py`: Details back tests for our Liquidity Provider (LP) strategy implementation on Uniswap V3.
   - `model_selection.py` and `model_forecast.py`: Contain specific functionalities or modules used in our project.

## Dependencies

Ensure required Python packages are installed using:

```bash
pip install -r requirements.txt
```

The `requirements.txt` file lists all necessary dependencies.

## Data

The `/data` directory stores datasets used in our project:

- `DeriBit_volatility_OHLC_ETH.csv`: Contains prices for DeriBit's ETH Implied Volatility Index (similar to VIX calculations).
- `ETHUSDC_clean.csv`: Contains spot prices for ETH/USDC from Binance. Missing data is imputed using ETH/USDT from Binance.
- `poolDayDatas.json`: Contains on-chain data for the Uniswap V3 0.05% USDC/ETH liquidity pool. The data was obtained by querying The Graph, a decentralized indexing and querying protocol for blockchain data.

## Techniques Used

Our project utilizes various techniques:

- Time series forecasting
- Statistical modeling

### GARCH Model for Volatility Forecasting

We utilized the Generalized Autoregressive Conditional Heteroskedasticity (GARCH) model to forecast volatility. This method is particularly effective in capturing volatility clustering and modeling time-varying volatility in financial data analysis.

### Delta Calculation for LP Pair Hedging

We implemented a delta calculation methodology to hedge our Liquidity Provider (LP) pair position. This technique calculates the delta, which represents the sensitivity of the LP pair's value to price changes. By quantifying this sensitivity, we can effectively manage risk and optimize our LP strategy by adjusting our exposure to the market's movements.

For detailed implementations and code related to these techniques, refer to scripts or notebooks available in the `/src` directory.

## Contributors

- Max (@Maaxxxxxxx)
- Ernest (@inistminist)
- Darrell (@DarrellNgKK)

Feel free to reach out to us if you have any questions or suggestions!
