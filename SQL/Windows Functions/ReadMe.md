## Windows Functions are important

### Examples of Questions it answers

* What is the increase in sales today from yesterday?
* What is average salary by department ? (which is essentially a groupby aggregate but windows functions adds the group by in table for each row- which is helpful to pull into queries)
* What is rank of person in each class by marks ?
* If a person visited a electronics ecommerce website to get their phone fixed then we'd want to be able to rank their interactions with service center by latest to oldest if they happen to visit more than once
* Moving Averages (Thirty Day Aveages, monthly churn rate ,etc)




### Resources


* [PostGres Documentation](https://www.postgresql.org/docs/9.1/tutorial-window.html/)
* [Mode Analytics Windows Function Tutorial](https://mode.com/resources/sql-tutorial/sql-window-functions/)
* [N rolling day average](https://stackoverflow.com/questions/25922379/sql-query-for-7-day-rolling-average-in-sql-server/)
* [Added Calculations over N rolling day average](https://www.essentialsql.com/sql-puzzle-calculate-moving-averages/)
* [Periscope Blog Day over Day Changes](https://www.periscopedata.com/blog/computing-day-over-day-changes-with-window-functions/)
