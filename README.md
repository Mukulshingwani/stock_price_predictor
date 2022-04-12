# stock_price_predictor
<img src='https://schaeffers-cdn.s3.amazonaws.com/images/default-source/schaeffers-cdn-images/default-images/charts/bigstock-concept-of-stock-market-and-fi-410303575.jpg?sfvrsn=dd3ad806_4' width = '100%' height='450px'>
<h2> Project Overview</h2>
Investment firms, hedge funds and even individuals have been using financial models to understand market behaviour better and make profitable investments and trades. A wealth of information is available in the form of historical stock prices and company performance data, suitable for machine learning algorithms to process.
<br>
<br>
This Program uses an Artificial Recurrent Neural Network (RNN) called Long Short Term Meomery(LSTM) to predict the stock price of listed companies
<br>
<br>
RNN remembers its input, due to an internal memory, which makes it perfectly suited for machine learning problems that involve sequential data, prediction problems ,voice recognition etc. When it makes a decision, it considers the current input and also what it has learned from the inputs it received previously.

But An RNN tends to forget some things since it only has hidden state but a LSTM remembers all those things which are crucial for the program since it has a cell state as well as hidden states, cell state has the ability to remove or add info to the cell regulated by gates.

<h2>preprocessing</h2>
The required data was extracted using the pandas_datareader and the closing price of the stock was visualized
<br>
<br>
<img src = 'https://user-images.githubusercontent.com/73459839/162897179-251444df-d5d0-4fab-aed1-9bf51b222f82.png'>
<br>
out of all the retrieved data only closing price was considered
<br>
MinMax scaler was applied to scale the data in range 0 to 1
<br>
It was then splitted into training and testing datasets
<br>
<h2> Building and compiling the model</h2>
Sequential model was used to add the LSTM layers
<br>
<br>
optimizer used : Adam
<br>
loss function : Mean Squared Error
<br>
metric : Accuracy
<br>
<h2> Prediction graph </h2>
<img src = 'https://user-images.githubusercontent.com/73459839/162899199-e7f3c253-f831-4b57-abf1-e6e0a67d8b30.png'>

 
