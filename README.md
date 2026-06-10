# Stock-Portfolio-Tracker
# Hardcoded stock prices
stock_prices = {
    "AAPL": 180,
    "TSLA": 250,
    "GOOG": 140,
    "MSFT": 320
}
total_investment = 0
n = int(input("Enter number of stocks: "))
for i in range(n):
    stock = input("Enter stock name (AAPL/TSLA/GOOG/MSFT): ").upper()
    quantity = int(input("Enter quantity: "))
    if stock in stock_prices:
        investment = stock_prices[stock] * quantity
        total_investment += investment
    else:
        print("Stock not found!")
print("\nTotal Investment Value =", total_investment)
