# SQL Query Practice

In this exercise we'll practice writing SQL queries. Please use the `Wedge.DB` database. 
My recommendation is that you write your code in a plain text editor. Your OS comes with
one, but it's often nice to have a "fancier" one. Some recommendations: 

* [Ultraedit](https://www.ultraedit.com/)
* [Notepad++](https://notepad-plus-plus.org/downloads/)
* [SublimeText](https://www.sublimetext.com/)

I've included a .SQL file in the repository for you to work in, but there's nothing special
about it. You could make one yourself by just making a plain text file and changing the file
extension. 

The typical flow for working on SQL could be something like this: 

1. Open `Wedge.db` via DB Browser.
1. Open your .sql file in DB Browser
1. Refine the query in the DB Browser. Save your work as you go. 
1. Submit the finished SQL file. 

## Questions

The file `Wedge.DB` has three summary tables of Wedge data in it: 

* `HourSales`: Sale information by hour of the day for the full range of our data. 
* `OwnerSales`: Sale information by owner (called CardNum), year, and month.
* `ProdSales`: Sale information by product, year, and month. 

The "Sale Information" has three columns in each case: spend, transactions, and 
items. The first is the dollar amount associated with the dimensions. The second,
called `transact` in the tables, is the number of transactions associated with the
dimensions. This is, basically, the number of receipts. So if card 12345 has 4 transactions
in January 2010, this means they generated 4 receipts. If "Organic Bananas" has 1000
transactions in the same month, this means organic bananas appeared on 1000 reciepts in the 
month. The final field, items, counts the number of individual items purchased, although
these can be unreliable for some produce and bulk purchases. 

Here are the questions I'd like you to answer in your queries: 

1. Sales by Hour of the Day across the full time period. This will have at most 24 rows.
1. Sales by Hour by Year: Same as the above but broken out by year as well. This will have at most 24 rows per year.
1. Sales by Hour for 2015: Same as above, but subset to just 2015. 
1. Owner spend by month: Spend or sales by owner by month.
1. Owner spend by month for owners who spent between $5K and $10K: Spend or sales by owner by month but only for owners who spent between $5K and $10K in total. 
1. The top 10 selling products at the Wedge
1. The top 10 selling products at the Wedge by Year for 2015 and 2016

