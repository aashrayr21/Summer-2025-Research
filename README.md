Imported stock indicator data from Yahoo Finance. Originally did testing on a large cap stock (SOFI), medium cap stock (NOA), and a small cap stock (BRTX). Testing was done on stock data over the course of 10 days, with all three initial stocks going through the process.
Started with a 70/20/10 split of the data and then put it through three different machine learning algorithms which were GD Boost, Random Forest, and LSTM. 
Initial models were the data showed GD Boost to have the best model so I proceeded with that algorithm and applied RSI to it before putting it through paper trades.
Then the data was denoised using moving averages and put through the same process and once again paper traded.
The paper trades were done with a value of $1,000,000. 
These were just initial tests and now it was time to apply the same code to 4 new stocks that were top daily gainers for their respective days.
The algorithm would only run on a few hours of code from 9:30 am to whenever the stock peaked in price which was usually around noon. 
First stock was NEGG, which had an opening price of 08/04/2025 of $60.25 and hit a peak of $68.40, which was a gain of 13.53 %. I applied my algorithm (noisy and denoised) and then did paper trades I got -8.12% gain for noisy and -9.04 % gain for denoised.
Second stock was SEAT, which had an opening price on 08/06/2025 of $20.95 and hit a peak of $35.00, which was a gain of around 67.06 %. I applied my algorithm (noisy and denoised) and then did paper trades I got -0.81% gain for noisy and 4.20 % gain for denoised.
Third stock was BROS, which had an opening price on 08/07/2025 of $69.65 and hit a peak of $71.80, which was a gain of around 3.09 %. I applied my algorithm (noisy and denoised) and then did paper trades I got 0% gain for noisy and 0 % gain for denoised.
Fourth stock was IBP, which had an opening price on 08/07/2025 of $230.93 and hit a peak of $263.20 which was gain of around 13.98%. I applied my algorithm (noisy and denoised) and then did paper trades I got 0% gain for noisy and 1.07 % gain for denoised.
These four stocks were all picked on the same day in the morning which is why some don't have gains as much as others. I wanted to simulate a trader would pick a stock for the machine based off of initial stock momentuem in the morning. 
Overall I found that denoised data was better to use but regardless it can still not beat a human simply trading using his or her eyes.
