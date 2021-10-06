
# Future Capital Coding Interview

To solve this challenge, feel free to use any and all resources available to you. You can also choose to solve the problem in whichever language you're most comfortable with. This challenge will consist of three parts and a bonus question. 

##  Part  1  -  Calculate  the  total  value  of  a  stock  portfolio

A sample stock portfolio is passed in as an argument to a console application. Your application should parse this input, lookup the stock price at close from the sample [stocks.json](https://raw.githubusercontent.com/pronvest/interview/master/backend/stocks.json) file, and then return the total value of the portfolio.

### Input
`-part1 [<TICKER>:<QUANTITY>]`

### Output
`<TOTAL>`

###  Examples

1) `./app -part1 "FB:12,PLTR:5000"  =>  119887.4`

2) `./app -part1 "BABA:1,TSLA:5,WISH:1200"  =>  9891.9`

##  Part  2  -  Return  the  allocations  for  each  investment

Add an additional function that returns the portfolio percentage or allocation for each investment. Essentially, we want to know how much of a portfolio is allocated towards each investment.

### Input
`-part2 [<TICKER>:<QUANTITY>]`

### Output
`[<TICKER>:<ALLOCATION>]`

### Examples

1) `./app -part2 "FB:12,PLTR:5000"  =>  FB:0.03242543,PLTR:0.96757457`

##  Part  3  -  New  investment

A client wants to make a new investment of $10,000 into facebook. They want to be assured that their portfolio is at least 10% allocated to facebook. Write an additional function that returns true or false if a new investment of $10,000 is enough for them to reach a 10% holding of fb for their portfolio.

### Input
`-part3 [<TICKER>:<QUANTITY>]`

### Output
`<SUCCESS>`

####  Examples

1) `./app -part3 "BABA:1,TSLA:5,WISH:1200"  =>  true`

## Bonus - Maximize profits

An analyst has developed an equation for predicting future stock prices. A client wants to use this algorithm to place a buy order at the optimum time and one sell order at the optimum time. You are provided a list of `prices` where `prices[i]` is the price of a given stock on the `ith` day. You want to maximize your profit by choosing a single day to buy one stock and choosing one different day to sell in the future. Due to trade restrictions, you may only place one buy order and one sell order. Return the maximum profit that the client can achieve from this transaction. If the client cannot achieve any profit, then return 0.

### Input
`-bonus [<PRICE>]`

### Output
`<PROFIT>`

#### Examples

1) `./app -bonus "7,1,5,3,6,4"  =>  5` 
* In this example, you would buy on day 2 (price = 1) and sell on day 5 (price = 6).

2) `./app -bonus "7,6,4,3,1"  =>  0`
* In this example, no buy or sells are performed.

## Submission

Please upload your sample application, along with execution instructions, to github and then send us the link to your repository.
