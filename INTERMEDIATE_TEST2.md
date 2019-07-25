# Backend Intermediate Test

There is a law stating that all employees from all companies in a certain country are required to contribute to a shared fund managed by the government with 8% of their salary on a monthly basis. Every employee has its own account and balance that represents the sum of all his monthly contributions plus inflation adjustments.

The employee is able to withdraw a portion of the account balance only on the day of his anniversary. The eligible ammount is determined by some rules according to the total available balance on his account.

Create a micro-service that allows the employee to withdraw his money according to the following business rules.

## Business rules

* Withdrawals can only be made once on the employee's anniversary 
* Withdrawals are composed of a fixed money plus a gradual % limit of the account balance
* Withdrawals are limited to an ammount according to employee's account balance as per the following:

| Balance                     | % Limit | Fixed money |
|-----------------------------|---------|-------------|
| Up until $500.00            | 50%     | $0.00       |
| From $500.01 to $1000.00    | 40%     | $50.00      |
| From $1000.01 to $5000.00   | 30%     | $150.00     |
| From $5000.01 to $10000.00  | 20%     | $650.00     |
| From $10000.01 to $15000.00 | 15%     | $1150.00    |
| From $15000.01 to $20000.00 | 10%     | $1900.00    |
| From $20000.01              | 5%      | $2900.00    |
  

## Non functional requirements

Use whatever language, tools and frameworks you feel comfortable with, and briefly elaborate on your solution, architecture details, choice of patterns and frameworks.
