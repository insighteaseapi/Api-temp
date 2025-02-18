# **Forex API Node.js by Insightease**

## **Overview**
This project integrates with the **[Insightease Forex API](https://insightease.com/docs/forex-api)** to fetch and process forex-related data. The API allows you to:  
-  Retrieve forex symbols  
-  Convert currencies  
-  Get real-time exchange rates  
-  Analyze historical price trends  

It's built with **JavaScript** and runs in a Node.js environment.

---

## **Project Structure**
The project consists of two main files:

- **`insightease_forex.js`** – Defines the `InsighteaseForex` class, which interacts with the API.
- **`main.js`** – Demonstrates how to use `InsighteaseForex` by fetching exchange rates and displaying results.

---

## **Getting Started**

### **Prerequisites**
Before running this project, make sure you have:

- **Node.js 14+** installed
- An **Insightease API key** (sign up on their website)

### **Installation**
1. Clone this repository:
   ```sh
   git clone https://github.com/your-username/forex-api-insightease.git
   cd forex-api-insightease
#### Necessary Library
**Fetch API**: Used for making HTTP requests to the Forex API.

## Application
To make API requests and retrieve forex data, run the main script:
sh
node main.js

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

###  Other Links
- **Real-Time Currency Conversion:** [Forex Real-Time Conversion](https://insightease.com/currency-converter)
- **Contact Us:** [Website](https://insightease.com)

## License
This project is intended for educational purposes. For usage restrictions, please refer to the terms provided by the API provider.
