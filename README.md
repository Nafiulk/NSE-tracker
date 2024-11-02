# NSE-tracker
This project analyse NSE market data using google sheet.
## Step 1: Set Up the Google Sheet

1. Open Google Sheets:
Go to Google Sheets and open a new spreadsheet.
2. Create Column Headers:

In Row 1, create the following headers:
- A1: Ticker
- B1: Company
- C1: Price
- D1: Open
- E1: High
- F1: Low
- G1: Change %
## 📊 Step 2: Enter Stock Tickers and Company Names
Enter Ticker Symbols:

In column A, enter stock ticker symbols. For example:
A2: GOOG
A3: AAPL
A4: MSFT
Add Company Names:

In column B, enter the company names:
B2: Alphabet Inc.
B3: Apple Inc.
B4: Microsoft Corp.
## 📈 Step 3: Use the GOOGLEFINANCE Formula for Real-Time Data
In the following columns, we’ll add formulas to pull real-time data.

3.1 Current Price
C2:
excel
Copy code
=GOOGLEFINANCE(A2, "price")
Drag this formula down the column to apply it to other tickers.
3.2 Opening Price
D2:
excel
Copy code
=GOOGLEFINANCE(A2, "open")
Drag down to copy the formula.
3.3 High Price
E2:
excel
Copy code
=GOOGLEFINANCE(A2, "high")
3.4 Low Price
F2:
excel
Copy code
=GOOGLEFINANCE(A2, "low")
3.5 Change Percentage
G2:
excel
Copy code
=GOOGLEFINANCE(A2, "changepct")
