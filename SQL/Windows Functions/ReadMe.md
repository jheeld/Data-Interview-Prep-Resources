## Windows Functions are important

### Examples of Questions it answers

* What is the increase in sales today from yesterday?
* What is average salary by department ? (which is essentially a groupby aggregate but windows functions adds the group by in table for each row- which is helpful to pull into queries)
* What is rank of person in each class by marks ?
* If a person visited a electronics ecommerce website to get their phone fixed then we'd want to be able to rank their interactions with service center by latest to oldest if they happen to visit more than once
* Moving Averages (Thirty Day Aveages, monthly churn rate ,etc)


```
Windows_function (<Column you want to aggregate or perform function on>)
  OVER (
    [ PARTITION BY <Column you want to group by>  ]
    [ ORDER BY <Column you want to order by> [{ ASC | DESC }] ]
    [ <Windows Frame> ]
  )

```
Windows Frame first parameter : UNBOUNDED PRECEDING  or CURRENT ROW  
Windows Frame second parameter : UNBOUNDED FOLLOWING  or CURRENT ROW  


### Resources


* [PostGres Documentation](https://www.postgresql.org/docs/9.1/tutorial-window.html/)
* [Mode Analytics Windows Function Tutorial](https://mode.com/resources/sql-tutorial/sql-window-functions/)
* [N rolling day average](https://stackoverflow.com/questions/25922379/sql-query-for-7-day-rolling-average-in-sql-server/)
* [Added Calculations over N rolling day average](https://www.essentialsql.com/sql-puzzle-calculate-moving-averages/)
* [Periscope Blog Day over Day Changes](https://www.periscopedata.com/blog/computing-day-over-day-changes-with-window-functions/)
* [Difference between RowNum() , Rank() & DenseRank()](https://codingsight.com/methods-to-rank-rows-in-sql-server-rownumber-rank-denserank-and-ntile/)
* [Running Total Tutorial](https://codingsight.com/calculating-running-total-with-over-clause-and-partition-by-clause-in-sql-server/)
* [Google Cloud Analytical Functions Tutorial](https://cloud.google.com/bigquery/docs/reference/standard-sql/analytic-function-concepts)
* [Running Total Tutorials covering rows and range](https://sqlwithmanoj.com/tag/running-totals/)
* [Cumulative Sum](http://infocenter.sybase.com/help/index.jsp?topic=/com.sybase.infocenter.dc00800.1510/html/iqapgv2/iqapgv288.htm)
* [10 Day Moving Average](https://www.essentialsql.com/sql-puzzle-calculate-moving-averages/)
* [2 Months Moving Average](http://infocenter.sybase.com/help/index.jsp?topic=/com.sybase.infocenter.dc00800.1510/html/iqapgv2/iqapgv288.htm)
* [Lag / Lead](https://www.sqlshack.com/use-window-functions-sql-server/)
* [Rows Vs Range ](https://auntkathisql.com/2014/09/27/what-is-the-difference-between-rows-and-range/)
* [Rows Vs Range II](https://www.sqlpassion.at/archive/2015/01/22/sql-server-windowing-functions-rows-vs-range/)

