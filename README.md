# 🐍 SnakeTrade — BTC Price Prediction Game

Real-time BTC price moves like a snake. Place targets where you think it'll go. Hit = points × multiplier.

## 🚀 Run Locally with Real BTC Data

### Option A: Just Double-Click (Easiest)
1. Save `index.html` to your computer
2. Double-click to open in Chrome
3. Binance WebSocket connects automatically — no API key needed
4. Green dot + "LIVE" = real data flowing

### Option B: Local Server (for mobile testing)
```bash
cd btc-snake-trader
python3 -m http.server 8080
```
Open `http://localhost:8080` on your phone (same WiFi).
Tap Share → "Add to Home Screen" to install as an app.

## 📡 Data Sources (auto-fallback)
1. **Binance WebSocket** — real-time trades (~10ms) 🟢 LIVE
2. **CoinDesk/CoinGecko/CryptoCompare REST** — polling (~3s) 🟡 POLL
3. **Built-in simulation** — offline fallback (50ms ticks) 🟠 SIM

No build step. No npm. No API keys. Just open and play.
