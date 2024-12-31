#CS50 - Project 9 - Finance Project
#EDX => mh_rabiyan
#Country => Pakistan
Repository that contains the code for the solution for the ninth project of the CS50 course. The application consists of a share purchase and sales company. The main objective of the project is to allow users to see the current quote, buy shares, sell shares and view their transaction history. The application was built with the Flask framework.

[![Page Wiki Project](https://i.postimg.cc/JnfrdSf6/Dja.png)](https://vvpasson.pythonanywhere.com/login)

## Project Page

The project was made available for interaction through [Python Any Where](https://vvpasson.pythonanywhere.com/login).
Note: Because the application is using a free trial API key from IEX Cloud, it may not work when you try to search for stocks - it will return that it is invalid - this is because the free key has a duration. After the free trial period, I only pay to continue carrying out consultations on the IEX Cloud platform, which is not in my interest.

## Youtube Video

A brief video demonstrating the result of the project was made and hosted on [YouTube](https://youtu.be/PnCtjh5K7-M).

## Project specifications

1. **Registration**: complete the implementation of *register* so that a user can register through a *form*.
    * The user must provide a *username* input via a *text field*, where the *name* is *username*. If the field is left blank or the user already exists, a message must be returned;
    * It must also have a password as *input*, implement this with a *text field* with *name* of *password* and then make an equal field for confirmation, whose *name* will be *confirmation*. Return a message if the field is left blank or the passwords do not match;
    * Submit user input via *POST* to */register*;
    * Insert the new user into the *users* database, but do not store the user's password itself, but a *hash* of the password.

    After implementing *register* correctly, you should be able to register an account and log in.
2. **Quote**: Complete the *quote* implementation so that it allows a user to check the current price of a share.
    * The user must provide the stock symbol and the current stock price will be returned;

3. **Purchase**: Complete the implementation of *buy* in a way that allows a user to buy a share.
    * The user must provide the stock symbol and quantity;
    * Make sure that the symbol exists and the quantity is not negative, if either of these occurs, return a message to the user;
    * In addition, you must make sure that the user has the funds to do so, if he does not have enough money to purchase the quantity of shares at a certain price, he must not complete the purchase and a message must be returned to the user.

    After implementing *buy* correctly, it should be possible to see what the user's wallet is like.
4. **Sell**: Complete the *sell* implementation so that it allows a user to sell a share.
    * User must provide stock symbol and quantity. However, it should only be possible to sell shares that are in your portfolio;
    * Return a message to the user if the quantity is negative, zero or does not have that quantity in the portfolio to sell.

5. **History**: complete the implementation of *history* in a way that allows a user to see a summary of their transactions, that is, what they sold and what they bought.
    * In each line, make it clear whether a share was bought or sold, including the symbol, price, quantity and date when the transaction occurred.

6. **Personal touch**: give the application a personal touch.
