# Heimweg

Live board for the way home: U2 from Theresienstraße to Feldmoching, then the S1 towards Lohhof.

- For each upcoming S1 north (Freising / Flughafen) it shows the **two latest U2** that still catch it, using the S1's **live** departure and at least **1 minute** to change at Feldmoching.
- Data: MVV timetable server (EFA), via the Cloudflare relay `zug-relay` (MVV doesn't allow websites to load its data directly).
- U2 arrival times come from MVV's journey planner; if it has none, the app adds a typical ride time (marked with ≈).

Settings are constants at the top of the script in `index.html` (`MIN_CHANGE`, `PER_S1`, `MAX_S1`).
