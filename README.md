# Stock Prediction App

This is a simple stock prediction web application built with React. The application allows users to input various financial metrics and get predictions about whether a stock is overvalued or undervalued. The app calculates various financial ratios and returns the results in a formatted table.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Environment Variables](#environment-variables)
- [Components](#components)
  - [App](#app)
  - [FinancialForm](#financialform)
  - [Result](#result)
- [API Integration](#api-integration)
- [Styling](#styling)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/stock-prediction-app.git
    ```
2. Change directory to the project folder:
    ```bash
    cd stock-prediction-app
    ```
3. Install the dependencies:
    ```bash
    npm install
    ```

## Usage

1. Start the development server:
    ```bash
    npm start
    ```
2. Open your browser and go to `http://localhost:3000`.

## Environment Variables

To run this project, you will need to add the following environment variable to your `.env` file:

```
REACT_APP_GEMINI_API=your_gemini_api_key_here
```

## Components

### App

The main component that renders the application. It includes the header, `FinancialForm` for input, and `Result` for displaying the result.

### FinancialForm

This component renders a form for users to input financial metrics. It includes fields for market price, EPS, book value, sales, annual dividends, previous EPS, current EPS, total debt, total equity, and net income. It also handles the form submission and API call to get the prediction result.


## API Integration

The app integrates with the Gemini API to get stock predictions. The `handleSubmit` function in the `FinancialForm` component sends the input data to the API and processes the response.

## Styling

The app uses CSS for styling. The styles are organized into separate CSS files for each component:
- `App.css`
- `FinancialForm.css`
- `index.css`

### Result

This component displays the prediction result returned from the API.
