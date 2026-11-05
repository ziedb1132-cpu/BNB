# BNB AI Paper Research Engine

Independent BNB-USDT spot research engine.

- OKX market data for **BNB-USDT**
- Paper signals only; no real orders
- 1,205-dimensional feature schema (1,200 engineered features + 5 context features)
- 8 explainable strategy families with fee-aware evaluation
- 30-layer AI signal and TP/SL exit-policy models
- AI training gate opens after 10 compatible closed TP/SL signals and continues incrementally
- AI-selected entry method and learned TP/SL policy
- 5-minute signal lifecycle; no time-exit
- State persistence after every cycle; 100 cycles per GitHub Actions run, then workflow restarts
- Files larger than 90 MiB are split into verified chunks and restored on the next run

Start manually from **Actions → BNB AI 100-cycle runner → Run workflow**. The workflow also runs on its scheduled cadence.

All signals are simulated research records. No exchange orders are submitted.
