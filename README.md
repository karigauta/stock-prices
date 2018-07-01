# stock-prices

[![Build Status](https://travis-ci.org/modern-fortran/listings.svg?branch=master)](https://travis-ci.org/modern-fortran/stock-prices)
[![GitHub issues](https://img.shields.io/github/issues/modern-fortran/stock-prices.svg)](https://github.com/modern-fortran/stock-prices/issues)

Processing stock prices with Fortran arrays.

![](https://github.com/modern-fortran/stock-prices/blob/master/plotting/adjclose_multipanel.svg)

## Getting started

### Getting the code and data

```
git clone https://github.com/modern-fortran/stock-prices
cd stock-prices
make
```

This will build three small apps: `stock_gain`, `stock_volatility`, and `stock_crossover`.

### Running the programs

```
./stock_gain
./stock_volatility
./stock_crossover
```

### Making figures

Python plotting scripts are provided to read and plot the data
produced by the Fortran apps.

Make sure to first set up a fresh Python virtual environment:

```
python -m venv venv
source venv/bin/activate
pip install -U pip
pip install -r plotting/requirements.txt
```

Then type:

```
make figures
```
