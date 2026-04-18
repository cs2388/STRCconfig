# STRC Tracker Support

STRC Tracker is an iOS app that tracks Strategy's STRC Bitcoin accumulation program in real time.

## Contact

For support, questions, or feedback, please email **cws2026@proton.me**. We'll respond as quickly as we can.

## Frequently Asked Questions

### How are ATM accumulation estimates calculated?

Estimates are derived from STRC trading volume above par ($100). When STRC trades heavily above par, Strategy issues new shares and uses the proceeds to buy Bitcoin. The app estimates the daily BTC accumulation using a volume-proxy methodology.

These estimates are not confirmed purchases. Official confirmation comes via SEC 8-K filings, which Strategy files weekly on Mondays covering the prior Monday–Sunday period.

### What do the confidence ratings mean?

- **HIGH** — STRC volume is strongly above the ATM threshold
- **MED** — Volume is moderately above the threshold
- **LOW** — Volume is near or below the threshold
- **NO ATM ACTIVITY** — STRC traded below par all day; no ATM issuance occurred
- **8-K CONFIRMED** — The purchase has been officially disclosed via SEC 8-K filing

### Where does the data come from?

- **Bitcoin price:** CoinGecko public API
- **STRC real-time trades:** Alpaca Markets
- **Confirmed purchases and STRC dividend rates:** SEC EDGAR
- **Strategy total BTC holdings:** SEC filings, periodically updated

### Why did the STRC dividend rate change?

STRC is a variable-rate perpetual preferred stock. Strategy adjusts the dividend rate each month. Rate changes are announced via SEC 8-K filings and reflected in the app once EDGAR publishes them.

### Why does the ATM status show "closed"?

ATM issuance only happens during US market hours. When the market is closed — weekends, before 9:30 AM ET, after 4:00 PM ET, or on market holidays — the app shows a closed or standby state. During pre-market (4:00–9:30 AM ET) and after-hours (4:00–8:00 PM ET) sessions, the app shows extended-hours labels.

### Why do BTC prices update every 60 seconds instead of continuously?

The BTC price comes from CoinGecko's public API, which has a 60-second polling limit to prevent rate limiting. Prices are as live as the free tier allows.

### Is this financial advice?

No. STRC Tracker is an informational tool only. Nothing in this app constitutes financial, investment, trading, or any other type of advice. Cryptocurrency and preferred stock investments carry significant risk including possible loss of principal. Always conduct your own research and consult a qualified financial advisor before making investment decisions.

### Is this app affiliated with Strategy Inc.?

No. STRC Tracker is an independent product and is not affiliated with, endorsed by, or sponsored by Strategy Inc. (formerly MicroStrategy), CoinGecko, Alpaca Markets, or the SEC.

## Privacy

STRC Tracker does not collect, store, or transmit any personal data. All user input — including share counts, cost basis, and start dates — is stored locally on your device via iOS UserDefaults and is never sent to any server. The app communicates only with public data APIs (CoinGecko, Alpaca Markets, SEC EDGAR) to fetch market information.

## Version History

Release notes for each version are available on the App Store listing.

## Reporting a Bug

If you encounter a bug or unexpected behavior, please email **cws2026@proton.me** and include:

- Your iOS version
- Your iPhone model
- The app version (shown in Settings → About)
- A description of what you expected vs. what actually happened
- Screenshots if applicable
