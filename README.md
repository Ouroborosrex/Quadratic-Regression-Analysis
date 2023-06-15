## Quadratic Regression Analysis
### Author: OuroborosRex
This script performs quadratic regression analysis on financial data using the Statsmodels library in Python. It fits a quadratic curve to the data and predicts future values based on the curve.

### Prerequisites

- Python 3.x
- pandas
- statsmodels
- matplotlib
- scipy

### Installation

1. Clone the repository or download the script file.
2. Install the required libraries by running the following command:
   ```
   pip install pandas statsmodels matplotlib scipy
   ```

### Usage

1. Prepare the data:
   - Ensure the financial data is in a CSV file.
   - Update the file path in the `data = pd.read_csv(...)` line to point to your CSV file.

2. Customize the regression analysis:
   - Modify the `quadratic_func` function if you want to fit a different quadratic equation.
   - Adjust the window size in the `calculate_rolling_average` function for calculating the rolling average.
   - Uncomment the necessary plotting code if you want to visualize the data and regression curves.

3. Run the script:
   ```
   python script.py
   ```
   or
   - Run the Jupyter code blocks.

4. Interpret the results:
   - The script performs quadratic regression on the financial data and calculates the directional accuracy and directional short accuracy.
   - The directional accuracy represents the percentage of successful directional predictions based on the regression curves.
   - The directional short accuracy represents the percentage of successful short-term directional predictions based on the regression curves and rolling averages. The short term is half of the window of the normal directional accuracy (e.g. 40 -> 20).

### Notes

- This script assumes that the financial data is organized in a specific format and requires customization based on your data structure.
- Adjustments and modifications may be necessary to fit the script to your specific use case.

Please make sure to customize the script according to your data and requirements before running it.
