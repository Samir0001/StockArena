# StockArena V1

A clean demonstration/starter implementation for the StockArena concept: social trading + thematic baskets + Solana execution adapters.

## Important
This package contains **no fake live market feed**. The chart component currently uses illustrative UI data until a live provider is configured. The quote endpoint returns `null` when no provider key is present.

## Run
1. Install Node.js 20+.
2. `npm install`
3. Copy `.env.example` to `.env`.
4. Add a market-data API key if available.
5. `npm run dev`
6. Open the Vite URL shown in the terminal.

## Production modules to add
- `@solana/web3.js`
- `@solana/wallet-adapter-react`
- `@solana/wallet-adapter-wallets`
- Anchor program for StockArena-owned state
- Jupiter quote/swap integration after selecting supported tokenized-stock liquidity
- WebSocket market-data adapter
- PostgreSQL/Supabase
- Authentication/signature verification
- Server-side transaction verification

## Data integrity
Never display an illustrative value as live market data. The UI explicitly labels the demo chart and the backend reports when a live provider is unavailable.

## License
This starter is newly authored for the StockArena concept. It does not include or remove third-party copyright notices.
