# Cally — final submission

Live website: https://cally-v1-2.vercel.app/

This is the final website snapshot. The existing Vercel production project stays connected to aarush-hitgub/cally-v1.2; this repository is a separate submission snapshot and changes here do not redeploy the submitted URL. Cally Showcase is a separate copy for a protected real call to the owner's approved test phone.

## Judge walkthrough
1. Open the live website in Chrome or Safari. Allow microphone access if using speech, or use Type instead.
2. Choose a location by typing, current location or map pin. Adjust the 1–20 km radius.
3. Describe a repair request and confirm the details.
4. Watch roughly one minute of SIMULATED conversations against real local business listings. No businesses are called. Prices, availability and dialogue are illustrative, not those shops' actual quotes.
5. Compare results, inspect a simulated transcript, or open a real shop listing.
6. Use the credit button to preview 1/5/10/custom credit packs, U-topia's 5% merchant-funded demo discount, debit-card preview and alternating PromptPay reference images. No real payment verification exists; do not transfer money during the demo.
7. Settings support dark mode and English/Thai/Cantonese UI and call voice preferences. Defaults are English UI and Thai voice.

No payment or registration is required for judging. Three demo credits are supplied and search reservations are returned. The site runs on Vercel with the laptop switched off. Anthropic and Google Places credentials, balances, quotas and uptime remain required for understanding requests and live listing discovery.

## Run locally
Node.js 24.x is required. Run npm.cmd ci, then npm.cmd run dev -- --hostname 127.0.0.1 --port 3200. Production check: npm.cmd run build. Credentials are not committed. Copy the owner's existing .env.local privately. Final hosted mode needs ANTHROPIC_API_KEY, GOOGLE_MAPS_API_KEY, CALLY_DEMO_COOKIE_SECRET and CALL_LANGUAGE=th; keep LIVE_SHOP_NUMBERS empty. No template env files were substituted.

The final demo does not include official U-bot integration or real payments. Do not describe simulated data as verified savings or genuine shop quotes. Local credit state is SQLite; Vercel uses signed demo-session cookies, not a real money ledger. API keys remain server-only.

## Before judging
Test from a private browser/second device, keep provider quotas and billing available, avoid last-minute pushes to the deployed source repository, and keep a short backup recording. Monitor the Vercel project for deployment errors. Keep secrets outside Git; the original repository and caller configurations remain unchanged.

Upstream history and LICENSE files are preserved. Current source was production-built and radius filtering, location listings, payment-demo state and UI were verified before this snapshot. See the other handoff documents for implementation limitations.
