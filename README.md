# King County Housing Analysis

Author: Adam Pell

# Overview
This project will use regression analysis to analyze home prices in King County, Washington based on key attributes.

Iterative linear regression analysis of multiple attributes create a clearer picture of the factors that add value to (or detract value from) a home. My firm, Pell & Associates Realty, can use the information from this analysis to deliver effective and accurate insights to prospective home buyers and sellers.

# Business Problem
While buying or selling a home is a tremendously important transaction for many Americans, the process of finding the right price can be quite opaque, with large fluctuations in home values being attributed simply to market factors or location. At Pell & Associates Realty, our goal is to demystify King County housing prices through statistical analysis.

This project will examine comprehensive data from over 30,000 homes, discovering trends and building predictive models to forecast what your home will be worth when it's time for a move!

# Data Understanding
The available data comes from a record of home sales in King County. The records span from 1900 to 2022. In this analysis, I selected several key features to predict a home's price. They include:

- Livable square footage
- No. of bedrooms
- No. of bathrooms
- Year built
- View
- Condition (relating to overall maintenance)
- Grade (relating to construction and design quality)

# Methods
This analysis uses linear regression analysis starting with livable square footage and progressively adding other variables. This yields an iterative model that evolves and improves over the course of the project, generating valuable insights along the way.

# Results
Our final model has a predictive value (R-squared) of .462, meaning that about 46.2% of the variance in the data is captured by the model. The p-values for our F-statistic and for our coefficients are all statistically significant.

Our coefficients show that every square foot of livable space adds about 373 dollars to a home's value. Each bathroom adds about 9600 dollars to a home's value, and each bedroom still, to the model, diminishes a home's value. However, both of our negative influences (bedrooms and year built) are far outweighed by some of the encoded categorical features.

Each increase in grade adds, on average, around 250,000 dollars to the price of a home. The view feature that we encoded suggests that better views do correlate with higher prices, to the tune of about 130,000 dollars per increase in view quality. Our encoded condition value matters less than the other values, only accounting for about 1200 dollars per unit increase. This probably makes sense, since "condition" has more to do with maintenance of the house while "grade" has to do with more fundamental aspects such as construction and design quality.

All of the coefficient p-values are zero except for condition, which still manages to be significant at 0.034.

![Image of Square Footage Projections](/images/Screenshot%202024-01-17%20at%2010.57.52%20AM.png)


# Conclusions
Our final regression model paints a more complete picture of the factors to ignore and the factors to prioritize, whether you're buying or selling.

### Buyers

Buyers have a lot to pay attention to when looking for a prospective home. Not only should the design and layout speak to them, but they really need the home to preserve its value over time. Therefore, according to the Pell & Associates Realty analysis, buyers should pay a lot of attention to a home's grade. As evidenced in the dataset, King County assigns these grades to every home in the record. When touring, prospective buyers should demand to see the grade, as it not only provides vital information on the quality of the home, but also is a key factor in increasing or decreasing that home's value in the event of an purchase offer or future sale. Of course, having a nice view would help as well, but that is secondary in significance and can also be harder to come by.

**Prospective buyers should primarily be asking about the quality of a home's base attributes and finishes.**

### Sellers

Sellers have more control over how their home looks and presents on the market. In light of that, they can look beyond the grade and prioritize physical and cosmetic improvements. This includes things like "condition", livable square feet, and bathrooms. The King County Assessor defines condition as a function of a home's maintenance: Have faulty appliances been repaired? Has the home been touched up and renovated? These are the types of question an assessor would ask. These are also questions you are likely to get from interested buyers. As a seller, you want to make sure your home is in tip-top shape when it hits the market. That doesn't just mean repainting-- sellers should ensure all appliances are up-to-date and working well. Our analysis indicates that the value a good condition grade adds to a home is quite significant, potentially far outstripping the cost of renovations.

**Sellers should prioritize livable space and keep on top of maintenance and renovations.**

These recommendations should allow both buyers and sellers to maximize the value of a residential transaction. While there are other factors at play, this analysis allows our clients to see exactly how the physical attributes of a home can impact value

### Next Steps
Further analyses could yield additional insights for our clients. These include:

- Close analysis of ZIP codes/location
- Addition of noise pollution metrics to the model
- Different modeling techniques

## Repository Structure

- data
    - column_names.md
    - kc_housing_data.csv
- phase-2-project.ipynb
- Phase_2_Presentation.pdf (Direct link [here](https://docs.google.com/presentation/d/1no-E4kg61mOoCi9CrSUzbmcNo_mKAYO8nDhqT7nlh9w/edit#slide=id.g2ae3e555e6d_0_303))
- .gitignore
- CONTRIBUTING.md
- LICENSE.md
- README.md

## Contact Information
Adam Pell
apell7591@gmail.com
917-434-6615