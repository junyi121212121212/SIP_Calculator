# SIP Calculator 📈

A modern, user-friendly SIP (Systematic Investment Plan) and Lump Sum investment calculator built with Python and CustomTkinter. This application helps investors calculate returns, visualize growth patterns, and make informed investment decisions.

## ✨ Features

- **Dual Investment Modes**: Calculate returns for both SIP and Lump Sum investments
- **Interactive Visualizations**:
  - Pie charts showing invested amount vs maturity value
  - Growth charts displaying month-by-month portfolio progression
- **Modern UI**: Clean, green-themed interface using CustomTkinter
- **Input Validation**: Comprehensive error handling and input validation
- **Flexible Tenure Options**: Pre-defined tenure options (5-35 years) with custom input support
- **Real-time Calculations**: Instant results with detailed breakdowns

## 🚀 Quick Start

### Prerequisites

Make sure you have Python 3.7+ installed on your system.

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/junyi121212121212/SIP_Calculator.git
   cd SIP_Calculator
   ```

2. **Install required dependencies**:
   ```bash
   pip install customtkinter matplotlib numpy
   ```

3. **Run the application**:
   ```bash
   python SIP_calculator.py
   ```

   Or use the pre-built executable:
   ```bash
   ./SIP_calculator.exe  # Windows
   ```

## 📊 How to Use

### SIP Calculator
1. Enter your **monthly SIP amount** (e.g., 5000)
2. Select **investment tenure** from dropdown (5-35 years)
3. Input **expected rate of return** (e.g., 12 for 12% annual return)
4. Click **Calculate** to see results

### Lump Sum Calculator
1. Enter your **lump sum investment amount**
2. Select **investment tenure** from dropdown
3. Input **expected rate of return**
4. Click **Calculate** to see results

### Visualization Features
- **Pie Chart**: Visual breakdown of total invested amount vs maturity value
- **Growth Chart**: Month-by-month progression showing portfolio value vs invested amount

## 🛠️ Technical Details

### Built With
- **Python 3.x**: Core programming language
- **CustomTkinter**: Modern UI framework for enhanced appearance
- **Matplotlib**: Data visualization and charting
- **NumPy**: Numerical computations
- **Tkinter**: Base GUI framework

### Project Structure
```
SIP_Calculator/
├── SIP_calculator.py      # Main application file
├── SIP_calculator.ipynb   # Jupyter notebook version
├── SIP_calculator.exe     # Pre-built Windows executable
└── README.md             # Project documentation
```

### Key Calculations

**SIP Formula**:
```
M = P × [((1 + i)^n - 1) / i] × (1 + i)
```
Where:
- M = Maturity Amount
- P = Monthly Investment
- i = Monthly Interest Rate (Annual Rate / 12)
- n = Total number of months

**Lump Sum Formula**:
```
M = P × (1 + r)^t
```
Where:
- M = Maturity Amount
- P = Principal Amount
- r = Annual Interest Rate
- t = Time in years

## 🎯 Features in Detail

### Input Validation
- Prevents fractional values for amounts and tenure
- Validates numerical inputs only
- Ensures ROI doesn't exceed 100%
- Prevents zero values for critical fields
- Mutual exclusivity between SIP and Lump Sum modes

### Visualization Components
- **Pie Chart**: Shows proportion of invested capital vs returns
- **Growth Chart**: Displays portfolio growth trajectory over time
- **Color Coding**: Green theme for positive growth visualization

### User Interface
- **Clean Design**: Modern green-accented interface
- **Responsive Layout**: Organized input and output sections
- **Error Handling**: User-friendly error messages
- **Reset Functionality**: Easy form clearing

## 🔧 Development

### Creating Executable
To create a standalone executable:

```bash
pip install pyinstaller
pyinstaller -F -w SIP_calculator.py
```

### Jupyter Notebook
The project includes a Jupyter notebook version (`SIP_calculator.ipynb`) for:
- Matplotlib Version
- Plotly Version
- To provide alternative if you do not want to download the .exe file

## 📈 Example Calculations

### SIP Example
- **Monthly Investment**: $10,000
- **Tenure**: 10 years
- **Expected Return**: 12% per annum
- **Result**:
  - Total Invested: $12,00,000
  - Maturity Value: $23,23,391
  - Wealth Gained: $11,23,391

### Lump Sum Example
- **Investment Amount**: $1,00,000
- **Tenure**: 10 years
- **Expected Return**: 12% per annum
- **Result**:
  - Maturity Value: $3,10,585
  - Wealth Gained: $2,10,585

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🙏 Acknowledgments

- CustomTkinter for the modern UI framework
- Matplotlib for excellent charting capabilities
- The Python community for continuous support

## 📞 Support

If you encounter any issues or have questions:
1. Check the existing issues on GitHub
2. Create a new issue with detailed description
3. Include screenshots if applicable

---

**Happy Investing! 💰**

*Disclaimer: This calculator provides estimates based on the inputs provided. Actual investment returns may vary due to market conditions and other factors. Please consult with a financial advisor for investment decisions.*