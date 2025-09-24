## Options Simulator

A comprehensive options trading simulator with both API backend and GUI frontend for analyzing options strategies and market behavior.

## Overview

This project provides a complete options trading simulation environment that allows users to:
- Simulate options trading strategies
- Analyze market behavior and pricing models
- Interact through both programmatic API and graphical interface
- Test different scenarios and market conditions

## Architecture

The simulator consists of two main components:
- **Backend API** (`app.py`) - Core simulation engine and data processing
- **Frontend GUI** (`main.py`) - User interface for interactive simulation

## Installation

### Prerequisites
- Python 3.7+
- pip package manager

### Setup

1. Clone the repository:
```bash
git clone https://github.com/lj334g/Options-Simulator.git
cd Options-Simulator
```

2. Install required dependencies:
```bash
pip3 install -r requirements.txt
```

## Usage

The simulator requires running both the backend API and frontend GUI simultaneously.

### Starting the Backend API

In your first terminal, start the API server:
```bash
python3 app.py
```

This launches the backend simulation engine that handles:
- Options pricing calculations
- Market data processing
- Strategy analysis
- Real-time computations

### Starting the GUI Frontend

In a second terminal, launch the graphical interface:
```bash
python3 main.py
```

This opens the user interface for:
- Strategy configuration
- Market parameter adjustment
- Results visualization
- Interactive simulation controls

## Features

### Options Modeling
- Black-Scholes pricing model implementation
- Greeks calculation (Delta, Gamma, Theta, Vega, Rho)
- Multiple option strategies support
- Real-time price updates

### Market Simulation
- Customizable market parameters
- Volatility modeling
- Interest rate scenarios
- Time decay simulation

### Analysis Tools
- Profit/Loss visualization
- Risk metrics calculation
- Strategy comparison
- Performance analytics

## Project Structure

```
Options-Simulator/
├── app.py              # Backend API server
├── main.py             # Frontend GUI application
├── requirements.txt    # Python dependencies
├── README.md          # This file
└── [other modules]     # Additional simulation components
```

## API Endpoints

The backend API provides endpoints for:
- `/calculate` - Options pricing calculations
- `/strategy` - Strategy analysis
- `/market` - Market data simulation
- `/analyze` - Performance analysis

## GUI Features

The graphical interface includes:
- Strategy builder with drag-and-drop
- Real-time price charts
- Parameter adjustment sliders
- Results dashboard
- Export capabilities

## Dependencies

Key Python packages used:
- `numpy` - Numerical computations
- `scipy` - Statistical functions
- `pandas` - Data manipulation
- `matplotlib` - Visualization
- `tkinter` - GUI framework
- `flask` - API framework
- Additional packages listed in `requirements.txt`

## Usage Examples

### Basic Strategy Simulation
1. Start both backend and frontend
2. Select an options strategy (e.g., covered call)
3. Configure market parameters
4. Run simulation and analyze results

### Custom Scenario Testing
1. Adjust volatility, interest rates, and time parameters
2. Compare multiple strategies side-by-side
3. Export results for further analysis


## Development

### Running in Development Mode
- Backend: `python3 app.py --debug`
- Frontend: `python3 main.py --dev`

### Testing
```bash
python3 -m pytest tests/
```

## Technical Details

### Options Pricing Models
- Black-Scholes-Merton model
- Binomial tree pricing
- Monte Carlo simulation

### Risk Management
- Value at Risk (VaR) calculations
- Maximum drawdown analysis
- Scenario stress testing
