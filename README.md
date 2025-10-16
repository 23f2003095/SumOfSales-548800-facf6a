# Sales Summary 659

## Overview / Purpose
This is a simple, minimal web application that loads sales data from a CSV file, calculates the total sales for categories less than or equal to 29, and displays the result on the page.

## Setup and Usage
1. Save the `index.html` file in your local directory.
2. Place the `sales.csv` file inside a folder named `attachments` in the same directory as `index.html`.
3. Open `index.html` in a web browser.
4. The total sales for categories &le; 29 will be displayed automatically.

## How it works
- The app uses JavaScript's `fetch()` to load the CSV file asynchronously.
- It parses the CSV data, assuming the first row contains headers.
- It iterates through each data row, summing the `sales` values where `category` is less than or equal to 29.
- The total sum is rounded to two decimal places and displayed in the element with `id="total-sales"`.

## Files
- `index.html`: The main webpage containing HTML, CSS, and JavaScript.
- `attachments/sales.csv`: The CSV data file (must be provided separately).

## Notes
- Ensure that the CSV file has headers named `category` and `sales`.
- This setup works locally with a simple file server or by opening the HTML file directly in a browser.