# Week 1 - Order Brushing

## Result



## Overview 

### Order brushing detection
Abnormal user behaviors on e-commerce platforms can be detected in various ways. For example, if an item in a shop is a best seller but many of its orders come from the same buyer, we have reason to suspect that the seller is conducting order brushing. Order brushing is technique that may be employed by sellers to create fake orders in order to inflate the sellers or a particular items rating, which may likely push that sellers items up the search results on Shopee. To maintain the integrity of shopee online shopping experience, shopee consistently monitor and flag any possible cases of order brushing on Shopee.

### Task

**1. Identify all shops that are deemed to have conducted order brushing.**

**2. For each shop that is identified to have conducted order brushing, identify the buyers suspected to have conducted order brushing for that shop**

For the purpose of this question, shops are deemed to have conducted order brushing if their concentrate rate is greater that or equal to 3 at any instance
```
ConcentrateRate = Number of orders within 1 hour / Number of unique buyes within 1 hour
```
For the purpose of this question, suspicious buyers are deemed as the buyer that contributed the highest proportion of orders to a shop that is deemed to have conducted order brushing. For calculation of the highest porportion of orders to a shop, only include the orders that occured in instances when order brushing has been deemed to have teaken place. In the case where mutiple users share the same highest proportion of orders for a specific shop, all those users are deemed to be suspicious buyers.
