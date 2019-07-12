
# Module 3 -  Final Project - Northwind Database


## Introduction

For this project, I was handed the Northwind Database and directed to formulate four questions that, when answered, will provide actionable information and recommendations to the company.

Before asking any questions, it was necessary to conduct an EDA to familiarize myself with the data.

* [Initial exploratory data analysis (EDA) notebook](initial_data_exploration.ipynb): A preliminary glance at the Northwind dataset to generate ideas for d.s. questions and to identify any potentially problematic nuances within the data.

## Questions

* **[Question 1 notebook](question_01.ipynb):** Does discount amount have a statistically significant effect on the quantity of a product in an order? If so, at what level(s) of discount?
    * *Null Hypothesis:* The presence of a discount has no effect on the quantity ordered.
    * *Alternate Hypothesis:* The presence of a discount has a statistically significant effect on the quantity ordered. 

* **[Question 2 notebook](question_02.ipynb):** Does the salesperson impact number and/or value of a sale? If so, can this be correlated to the reporting structure within the company?
    * *Null Hypothesis:* It makes no difference which employee took the order.
    * *Alternate Hypothesis:* Certain employees generate more (or higher value) sales than others.

* **[Question 3 notebook](question_03.ipynb):** Is there a correlation between product category and customer region? (i.e. do certain categories of product sell better/worse depending on the region?)
    * *Null Hypothesis:* There is no correlation between product category and customer region.
    * *Alternate Hypothesis:* There is a statistically significant correlation between product category and customer region.

* **[Question 4 notebook](question_04.ipynb):** Does time of year (month or season) affect the amount of each category that is ordered?
    * *Null Hypothesis:* The time of year has no impact on product sales.
    * *Alternate Hypothesis:* The time of year has a statistically significant impact on product sales.


## Analysis & Recommendations

Fortuitously, after testing, I was able to confidently reject all null hypotheses. The variables *discount*, *salesperson*, *employee reporting structure*, *customer region*, and *time of year* all had statistically significant effects on Northwind revenue. 

### Recommendations

#### Question 1:

Since the mere existence of a discount (even as low as 5%) tends to increase the number of units ordered by around 6-7 units, ***I  recommend applying a small discount to all products offered for sale***. Furthermore, large discounts should be avoided (unless there is a limited-time special sales event to drive interest) because they do not substantially increase units sold above the lower discount levels. The reasoning behind this phenomenon is the supposition that the presence of even a 5% discount has a psychological effect that encourages customers to buy more than they would otherwise.

#### Question 2:

Despite the testing results concluding that the sales manager's team regularly generates higher-priced sales than the VP's team, it seems that the VP's strategy is ultimately more beneficial. Rather than focus on increasing the price of each individual order, it appears that the VP's strategy of ***focusing on generating the highest number of sales ultimately produces more revenue*** for the company. 

This may simply be a result of the best salespeople being assigned to the VP's team while the Sales Manager is stuck with less-effective salespeople. 

Regardless, moving forward this company should encourage all of its salespeople to focus on producing as many distinct sales as possible and to pay less attention to making the total price of each sale as high as possible; the theory here being that the extra time spent trying to increase the value of a single sale would be better spent generating a second sale to another customer. 

#### Question 3:

I would recommend that salespersons readjust their sales efforts according to the table below. 

| Region | Product Categories to Market more Aggressively | Product Categories to Market Less Aggressively |
|:----- |:-----:|:-----:|
| British Isles | Condiments, Meat/Poultry, Produce | Beverages, Dairy Products, Grains/Cereals |
| Latin America | Condiments, Dairy Products, Produce, Seafood | Confections, Grains/Cereals, Meat/Poultry |
| North America | Beverages, Confections, Grains/Cereals, Meat/Poultry | Produce |
| Northeastern Europe | Beverages, Seafood | Confections, Dairy Products, Grains/Cereals, Meat/Poultry |
| Southern Europe | Condiments, Grains/Cereals, Meat/Poultry | Beverages, Confections, Dairy Products, Seafood |
| Western Europe | Condiments, Confections, Grains/Cereals | Meat/Poultry, Seafood |

These lists detail which regions spend proportionately more on certain categories as compared to the population ratios (e.g. Britain spends a higher percentage of its total wallet on condiments than the sample population does). This means that the listed product categories are in higher demand in the listed regions than one could normally expect, implying that it should be easier to sell more of those products (and possibly at a higher price) in those regions than others, especially when acquiring new customers.

However, this does not mean that existing sales of low-demand product-region combinations should be neglected to the point where they decrease. This study merely suggests that no additional effort be spent increasing those combinations.

#### Question 4:

Given the information in the table below, I recommend that salespersons focus on selling each product category during its respective highest demand season and spend less attention attempting to sell them during their lowest demand seasons. When demand is highest, sales of that product should be easiest to accomplish; conversely, when demand is lowest, sales will be hard fought, thus one should prioritize items which are more likely to sell.

| Product Category | Highest Demand | Lowest Demand |
|------|:------:|:-------:|
| Beverages | Autumn | Spring |
| Condiments | Spring | Summer |
| Confections | Winter | Summer |
| Dairy | Autumn | Summer |
| Grains | Winter | Summer |
| Meat | Autumn | Summer |
| Produce | Spring | Winter |
| Seafood | Autumn | Winter |


## Conclusions




## Future Investigation

Though the above recommendations should result in greater revenue for the company, there are many avenues for further potential insights. Looking at the product-by-product sales rates is likely to produce actionable information.

Additionally, the most advantageous think that could be done for future study is to include more diverse data in the database. The first variables that come to mind are `ProductWeight`, `ProductDimensions`, and `UnitCost` (assuming that `UnitPrice` refers to the sales price


### PowerPoint Presentation

Here is a link to the [slideshow itself]().

