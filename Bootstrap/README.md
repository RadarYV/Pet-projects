# Bootstrap in oil mining company

You work for the mining company BigOilCompany. We need to decide where to drill a new well.

You have been provided with oil samples in three regions: in each 10,000 fields, where the quality of oil and the volume of its reserves were measured. Build a machine learning model that will help determine the region where mining will bring the greatest profit. Analyze the possible profits and risks with the *Bootstrap technique.*

Steps to select a location:

- They are looking for deposits in the selected region, the values of the parameters are determined for each;
- Build a model and estimate the volume of reserves;
- Select the deposits with the highest value estimates. The number of deposits depends on the company's budget and the cost of developing one well;
- The profit is equal to the total profit of the selected fields.


## Task

Build a model to determine the region where mining will bring the greatest profit. Analyze the possible profits and risks with the *Bootstrap technique*.

- During the exploration of the region, 500 points are explored, from which 200 best ones are selected for development using machine learning.
- After assessing the risks, you need to leave only those regions in which the probability of losses is less than 2.5%. The region with the highest average profit is chosen among them.

## Data
The data of the three regions are in the files: geo_data_0.csv, geo_data_1.csv, geo_data_2.csv

- `id` — unique well ID;
- `f0, f1, f2` — three features of wells (it doesn't matter what they mean, but they themselves are significant);
- 'product' — the volume of reserves in the well (thousand barrels)

## Brief
- We loaded data, evaluate it.
- Calculate necessary level of product. It is significantly higher than the average values
- Create models
- Using bootstrap calculated 1000 profits (profit calculated over 200 best wells from 500 random points) in each region
- Selected site for mining


## Libraries used

- pandas
- seaborn
- matplotlib
- sklearn
