# AutoTrade Pro Mobile Web v1.1

This version adds a real read-only Deriv market-data connection and a deterministic BOS + Order Block + FVG + OTE + confirmation scanner.

## What it does
- Connects to public Deriv market data over WebSocket (no account token required for market data).
- Loads historical candles for supported Deriv symbols.
- Calculates swing highs/lows, BOS, Order Block, FVG, OTE (61.8–79%), confirmation and RR.
- Calculates the cash amount at risk from the configured account balance and risk %.
- Enforces the configured maximum trades/day and daily loss limit in the local demo journal.
- Keeps trade execution LOCKED. No real orders are placed.

## Install
1. Replace the files in your GitHub Pages repository with these files.
2. Open the GitHub Pages site over HTTPS.
3. Use Chrome > Add to Home screen.

## Important
This is a signal/scanner build, not a live MT5 executor. The public market-data connection is read-only. Real-money execution requires authenticated account access and a secure backend/bridge; do not put trading credentials in GitHub Pages frontend code.

## Source
Deriv public market-data documentation:
https://developers.deriv.com/docs/data/
