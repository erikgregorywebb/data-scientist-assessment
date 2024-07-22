### Background

At Clair, we are on a mission to create financial freedom for America's workers by giving them access to free wage advances so they can be paid as soon as they clock out of work. Clair partners with Time & Attendance and Payroll providers to receive data on employees, including shifts they work or salaries they earn. Using this data, Clair underwrites the employees for loans (wage advances) to provide liquidity between their paychecks. When payday comes, Clair recoups the funds advanced by debiting the employee’s bank account. In order to facilitate that repayment, Clair must know what day in the future to expect a paycheck to land in the employee’s bank account.

### Part I

Prepare a model that predicts the next paycheck date for an employee given a history of previous paycheck deposits. The deliverable is a Jupyter notebook with your model, complete with prediction generation and accuracy measurement. 

Leverage the `paychecks` table hosted on a cloud-hosted PostgreSQL database:

```
Host: pg-285c4482-getclair-7a3a.a.aivencloud.com
Port: 10594
Database: assessment
```

_Username and password credentials will be shared by email._

### Part II

Clair needs to determine eligibility for incoming users using Plaid transaction data from linked bank accounts. In other words, who should be allowed to take an advance based on our confidence that their bank account will have sufficient funds at the time of repayment? The deliverable is a written plan for how you would approach the determination of eligibility, factors you would consider, and ways you would monitor and iterate over time. Consider the questions below in your write-up:

1. What approaches or methodologies would you take to determine eligibility?
2. What insights or features would you look to develop from the transaction data?
3. How would you measure the efficacy of the determined eligibility criteria?
4. What are some considerations or pitfalls to be aware of when analyzing results?

A `plaid_transactions_sample` table is available for reference, also hosted on a cloud-hosted PostgreSQL database from Part I.

_Note: We aren’t expecting you to develop features or write any code for this. We want you to take us through the process you would undertake to make a determination of eligibility._
