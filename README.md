# MEXC Futures Trading Bot

This repository provides basic information about **MEXC Futures Trading Bot**, a private project for automating trading on MEXC Futures.

Full access to the project includes source code, detailed documentation, setup and usage instructions, and a complete list of supported features. The repository also contains a demo code file provided by MEXC support, adapted for working with the unavailable official API.

## How to Get Access?

To gain full access to the private repository, contact us via Telegram: [@young_vykqq](https://t.me/young_vykqq).  
Access is available on a paid basis.

---

## Features

The private project includes the following features:
- Retrieve account balances and open positions.
- Create market and limit orders with extensive customization.
- Manage stop-loss and take-profit orders.
- REST API integration for external applications.
- Built-in FastAPI server to manage the bot via endpoints.
- Adaptation to the unavailability of the official API through alternative methods.

---

## Server API (Endpoints)

The private project provides the following REST API endpoints for management:

1. **Retrieve Balance**
   - `GET /api/balance`
   - Example response:
     ```json
     { "result": 51990.97 }
     ```

2. **Retrieve Open Positions**
   - `GET /api/positions/open`
   - Example response:
     ```json
     { "result": [{ "symbol": "BTC_USDT", "leverage": 10 }] }
     ```

3. **Create a Order With Take-Profits And StopLoss**
   - `POST /api/orders/advanced/create`
   - Example request body:
     ```json
     { "pair": "BTC_USDT", "side": "buy", "leverage": 10, "price": "30000", "stopLoss": "29000", "takeProfits": ["31000", "32000", "33000"] }
     ```

4. **Set Stop-Loss**
   - `POST /api/orders/stoploss/set`
   - Example request body:
     ```json
     { "orderId": "12345", "stopLossPrice": "29000" }
     ```

A complete list of endpoints and usage examples is available in the private repository.

---

## Workaround Explanation

The official MEXC Futures API has been unavailable since 2022. This project implements a workaround that uses "secret" data to communicate with the platform successfully.  
The private repository also includes a demo code file provided by MEXC support, which facilitates adapting the project to the current limitations.

---

## Instructions and Setup

The private repository includes:
- Detailed instructions for configuring API keys.
- Description of all features and their parameters.
- Step-by-step guide for launching the server and using the API.
- Code examples for integrating with the project.
- Demo code provided by MEXC for API usage.

---

## Disclaimer

This project is intended for educational purposes only.  
Use it at your own risk. The author is not responsible for any financial losses caused by using this software. Ensure compliance with MEXC's API policies and terms of use.
