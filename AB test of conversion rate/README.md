# A/B Testing

## Task

Plan an A/B test, run, and analyze the results for an online store.

## Data

Table orders

- transactionId - order identifier;
- visitorId - ID of the user who made the order;
- date - the date when the order was made;
- revenue — order revenue;
- group — the A/B test group the order belongs to.

Table visitors

- date — date;
- group — A/B test group;
- visitors - the number of users on the specified date in the specified A/B test group

## Libraries used

- pandas
- scipy
- numpy
- seaborn
- matplotlib
- statsmodels
