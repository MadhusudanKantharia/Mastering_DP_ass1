# Mastering_DP_ass1


## Question 1
In the first question I created 3 of my own data_types for the question which are pretty straight forward.<br>
struct product{} is for the details of a product.<br>
struct log{} is for storing transactions.<br>
account{} is just to keep track of the stores balance of money and its loan.<br>
I also used unordered_map to connect the product IDs to their stock and details about sale price and cost price.<br>
I solved the question by first taking the enquiries of each customer seperately and then for the optimal payoff for the customer in the given budget i applied the generic knapsack problem approach and to get the bill i went back through my purchases and made a bill out of them.<br>
Then I made an update function to update the stock and take the loan, update the money accordingly, also I stored all the transactions.<br>
Then I printed out all the transactions made today + the repayment of the loan and in the end the net profit made today.<br>

The input should be given in the form:-<br>
The first line contains the number of type of products P.<br>
The second line contains the number of customers N<br>
The next P lines contain the product_ID, quantity K, cost price C, sale price S of the products<br>
The first line for each customer contains the number of queries of the customer m<br>
The second line contains the budget B of the customer
The next m lines contain each query consisting of product_ID and payoff value<br>
INPUT EXAMPLE:-<br>
3<br>
1<br>
a 0 2 3<br>
b 2 3 4<br>
c 2 5 6<br>
12<br>
3<br>
a 6<br>
b 4<br>
c 9<br>


## Question 2
I did it similar to the way I did the previous problem, i mapped the upper bounds to a certain element of the DP grid<br>
Still I was unable  to convert it into time complexity O(n)


## Question 3
I mean I can't really directly think od one, but there was a sort i studied named Radix sort in which the time complexity weny to O(nd) well when you fix the d i.e the number of digits of the input vector we can sort it in bascially O(n), in that sort it basically said to first sort it in units digit then tens digit and so on individually until d and then you get your priority order so you basically have the answer.
