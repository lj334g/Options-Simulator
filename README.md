# Options Simulator
A desktop application for simulating and visualizing options trading strategies in real time. It lets you build complex strategies, fetch live option quotes, and analyze risk and P&L interactively.

Link to project: https://github.com/lj334g/Options-Simulator


# How It's Made
Tech used: Python, Flask, Tkinter (or PyQt), NumPy, pandas

The backend API is built with Flask exposing endpoints for pricing and simulation. The frontend GUI uses Tkinter (or PyQt) to provide an interactive interface. Data fetching, option pricing models (Black-Scholes, binomial), and Monte Carlo simulations are implemented in modular Python packages.

# Optimizations

Optional performance improvements include:
- Caching API responses to reduce latency when fetching quotes
- Vectorized NumPy operations in Monte Carlo to achieve 3× speedup over naive loops
- Asynchronous request handling in Flask to improve throughput under load

# Requirements

Use pip to install the packages in `requirements.txt`
pip3 install -r requirements.txt

# Run backend

In one terminal, run `python3 app.py`.
You can see the backend operations running from the API.

# Run frontend

In another terminal, run `python3 main.py`. This one is for the GUI.
python3 main.py
