# Forex API JavaScript by Insightease

## Overview
This project integrates seamlessly with the **[Forex API JavaScript by Insightease](https://insightease.com/docs/forex-api)** to retrieve and process forex-related data. It offers a range of functionalities, including fetching forex symbols, converting currencies, retrieving real-time prices, and analyzing historical data—all powered by JavaScript.

### Components:
- `insightease_forex.js`: Implements the `insighteaseForex` class, which provides multiple API interaction methods.
- `main.js`: Demonstrates the usage of `insighteaseForex` by calling various functions and printing the results.

# Integration of the Insightease Forex API

## Summary
Insightease's Forex API provides features such as currency conversion, accessing the latest market values, fetching forex symbols, and leveraging JavaScript to analyze historical data.

### Elements:
- The `insighteaseForex` class, which offers a number of API interaction methods, is implemented by `insightease_forex.js`.
- `main.js`: Shows how to use `insighteaseForex` by executing different functions and displaying the output.

## Installation

### Prerequisites
Make sure Node.js is installed. It is recommended to use Node.js 14 or later. Install the necessary dependencies next.

#### Necessary Library
**Fetch API**: Used for making HTTP requests to the Forex API.

## Application
To make API requests and retrieve forex data, run the main script:
```sh
node main.js
```

## Use Case Example
An example request to retrieve the most recent GBP/USD pricing is as follows:
```javascript
const insighteaseForex = require('./insightease_forex');

async function main() {
    const forexApi = new insighteaseForex('YOUR_API_KEY');
    const latestPrice = await forexApi.getLatestPrice("GBP/USD");
    console.log("Latest Price of GBP/USD:", latestPrice);
}

main();
```

## Notes
- The **fetch API** is used to make HTTP requests.
- The API key should be securely stored instead of hardcoding it.
- Ensure that the API base URL is correct and up to date.
- Since the response format is JSON, proper parsing and handling must be done.

### 🔗 Other Links
- **Real-Time Currency Conversion:** [Forex Real-Time Conversion](https://insightease.com/currency-converter)
- **Contact Us:** [Contact Insightease](https://insightease.com/contact)

## License
This project is intended for educational purposes. For usage restrictions, please refer to the terms provided by the API provider.

