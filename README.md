# Zerodha Trading MCP

A Model Context Protocol (MCP) server that enables AI models to interact with the Zerodha trading platform. This project provides a set of tools for executing trades, viewing portfolio, and managing positions on Zerodha through a standardized interface.

## Features

- 🔐 Secure authentication with Zerodha API
- 📊 View portfolio holdings
- 📈 Check open positions
- 💹 Place buy/sell orders
- 👤 Access user profile information

## Prerequisites

- Node.js (v14 or higher)
- Zerodha Trading Account
- API credentials from Zerodha

## Installation

1. Clone the repository:
```bash
git clone https://github.com/shubhamprajapati7748/zerodha-trade-mcp.git
cd zerodha-trade-mcp
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file in the root directory with your Zerodha credentials:
```env
KITE_API_KEY=your_api_key
KITE_SECRET_KEY=your_secret_key
REQUEST_TOKEN=your_request_token
ACCESS_TOKEN=your_access_token
```

## Usage

The MCP server provides the following tools:

### Get Profile
```typescript
get-profile
```
Retrieves the user's profile information from Zerodha.

### Buy Stock
```typescript
buy-stock {stock: string, quantity: number}
```
Places a buy order for the specified stock and quantity.

### Sell Stock
```typescript
sell-stock {stock: string, quantity: number}
```
Places a sell order for the specified stock and quantity.

### Show Portfolio
```typescript
show-portfolio
```
Displays the user's complete portfolio holdings.

### Show Positions
```typescript
show-positions
```
Shows the user's open positions.

## Development

The project is built using:
- TypeScript
- KiteConnect API
- Model Context Protocol (MCP) SDK
- Zod for schema validation

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Disclaimer

This project is for educational purposes only. Trading in financial markets carries significant risk. Always do your own research and trade responsibly.