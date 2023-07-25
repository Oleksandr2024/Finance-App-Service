# Finance-App-Service

The original Finance-App was divided into client and server part for convenience of deployment process. This is just a server part of the entire App. To visit the entire App live example please visit [Finance-App](https://finance-app-client-4d0z.onrender.com/)

Server-side:
Server side "getQuotes" function in server.js generates ticker prices with four dimensions: open_price, high_price, low_price, and close_price. This was done to enable candlestick visualization in the chart, similar to real-world stock apps. Additionally, the function considers the close price of a certain ticker and generates new prices with a reasonable price difference to avoid dramatic changes. It also calculates the "change_percent" and "change" based on a comparison between previous and current prices.

Implemented the ability for users to change the original value of "FETCH_INTERVAL" variable. Users can now adjust the fetch interval within a range of 1 to 50 seconds through the user interface. The updated value is then passed to the server-side and applied to the fetch_interval variable.
