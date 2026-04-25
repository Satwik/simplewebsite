INDIA ETF EXPLORER — DEPLOYMENT GUIDE
======================================

FOLDER CONTENTS
---------------
  index.html    → Landing page (this is the homepage users see first)
  explorer.html → The ETF data explorer (linked from the landing page)
  etf.csv       → Today's ETF data (replace this daily)
  README.txt    → This file

HOW TO UPLOAD TO GODADDY
-------------------------
1. Log in to GoDaddy → go to your Hosting Control Panel (cPanel)
2. Open "File Manager"
3. Navigate to the "public_html" folder
4. Upload ALL THREE files: index.html, explorer.html, and etf.csv into public_html
5. Your site is live at: https://yourdomain.com

HOW TO UPDATE DATA DAILY
-------------------------
1. Download fresh ETF CSV from NSE MarketWatch
2. Rename the file to exactly:  etf.csv (all lowercase)
3. In GoDaddy File Manager → public_html → upload etf.csv
4. Click "Overwrite" when prompted
5. Done — the explorer shows fresh data immediately

USER FLOW
---------
  User visits yourdomain.com  →  Sees landing page (index.html)
  Clicks "Explore All ETFs"   →  Goes to explorer.html (the data page)

TROUBLESHOOTING
---------------
- Explorer shows error?  Make sure etf.csv is in public_html alongside the HTML files
- Old data showing?       Hard-refresh: Ctrl+Shift+R (Windows) / Cmd+Shift+R (Mac)
- AI analysis not working? The AI needs an internet connection (calls Anthropic API)

NOTES
-----
- No database, no backend, no server-side code needed
- Works on any standard web hosting (GoDaddy, Hostinger, Namecheap, etc.)
