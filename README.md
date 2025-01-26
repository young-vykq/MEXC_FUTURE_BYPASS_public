# MEXC Futures Trading Code

This project offers a Python and Node.js-based client for interacting with the MEXC Futures API. Despite the official API being unavailable since 2022, a custom workaround is implemented to maintain functionality. Examples and concepts are adapted from the `/official_demo/contract_rest.py` and `/official_demo/contract_ws.py` files, ensuring seamless integration.

## Features
- Retrieve account balances and open positions.
- Create market and limit orders with advanced customization.
- Manage stop-loss and take-profit orders.
- REST API support for external integrations.
- Workaround for the unavailable official API through alternative methods.

## Developers

@vkidik
- [GitHub](https://github.com/vkidik/)
- [Telegram](https://t.me/young_vykqq) 

## Repository Access
**Full access to this private repository is available on a paid basis. For inquiries, contact:**
- Telegram: [@young_vykqq](https://t.me/young_vykqq)

## Example Functions (Partial List)
The following table provides a glimpse into the available functions in this project. For the full list, refer to the private repository:

| Method Name              | Description                              | HTTP Method | Parameters                                      |
|--------------------------|------------------------------------------|-------------|------------------------------------------------|
| `getServerPing`          | Check server availability               | GET         | None                                           |
| `getContractInfo`        | Retrieve details of a specific contract | GET         | `symbol: str` (e.g., `BTC_USDT`)              |
| `getContractDepth`       | Fetch order book depth                  | GET         | `symbol: str`, `limit: int?`                  |
| `createOrder`            | Place an order                          | POST        | `symbol: str`, `price: float`, `side: int`    |
| `cancelAllOrders`        | Cancel all orders                       | POST        | `symbol: str?` (optional)                     |

**This is only a subset of the supported functions. The private repository includes detailed documentation, parameter explanations, and additional features.**

## Project Structure
The project is organized into the following structure:

```
├── official_demo/
│   ├── contract_rest.py
│   ├── contract_websocket.py
├── src/
│   ├── nodejs/
│   │   ├── func.js
│   │   ├── index.js
│   │   ├── constants.js
│   │   ├── package.json
│   │   └── package-lock.json
│   ├── python/
│   │   ├── func.py
│   │   ├── init.py
│   │   ├── constants.py
│   │   └── requirements.txt
├── .gitignore       
├── LICENSE       
└── README.md
```

### Key Directories:
- **`official_demo/`**: Contains example scripts provided by MEXC for REST and WebSocket interactions.
- **`src/nodejs/`**: Node.js implementation of the client, including helper functions and constants.
- **`src/python/`**: Python implementation of the client, along with required dependencies.

# Usage Overview
- Utilize the Python or Node.js client for features such as balance retrieval, order placement, and more.
- Full documentation, code examples, and configuration guides are provided.

## Disclaimer
This project is for educational purposes only. Use at your own risk, and ensure compliance with MEXC's terms of use.

