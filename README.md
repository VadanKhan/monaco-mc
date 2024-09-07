# Monte Carlo Integration Example

This script demonstrates a Monte Carlo integration example using the `monaco` library. It estimates the value of π by calculating the area of a unit circle.

## Requirements

- Python 3.7+
- Poetry

## Installation

1. **Clone the repository** (if applicable):

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Install Poetry** (if not already installed):

   ```bash
   curl -sSL https://install.python-poetry.org | python3 -
   ```

3. **Install dependencies and create a virtual environment** in the same directory:

   ```bash
   poetry config virtualenvs.in-project true
   poetry install
   ```

## Usage

1. **Activate the virtual environment**:

   ```bash
   source .venv/bin/activate
   ```

2. **Run the script**:

   ```bash
   python mc_package.py
   ```

## Script Overview

The script performs the following steps:

1. **Preprocess**: Extracts input values.
2. **Run**: Checks if the points are under the curve (inside the unit circle).
3. **Postprocess**: Adds the result to the output values.

## Functions

- `integration_example_preprocess(case)`: Preprocesses the input values.
- `integration_example_run(x, y)`: Determines if the points are under the curve.
- `integration_example_postprocess(case, isUnderCurve)`: Postprocesses the results.

## Simulation Parameters

- `xrange`: Range for x values.
- `yrange`: Range for y values.
- `totalArea`: Total area for integration.
- `dimension`: Dimension of the integration.
- `savecasedata`: Whether to save case data.
- `samplemethod`: Sampling method (e.g., 'sobol').
- `firstcaseismedian`: Whether the first case is the median.
- `error`: Maximum error bound.
- `conf`: Confidence level.
- `stdev`: Standard deviation.

## Example Output

The script prints the estimated value of π and the number of samples needed for the specified error and confidence level.
