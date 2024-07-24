# M3_Challenge_MTF
Paper, code, and supplementary files submitted to the Math Modeling M3 Challenge.

**Keywords:** _Time Series Analysis, Regression Model, Ridge Regression, Facebook Prophet, Loss Models, Climate Change, Farming_

## Summary
This paper models financial impacts and losses in agriculture, particularly focusing on the rice industry in California and Louisiana, and proposes innovative solutions to prevent small farmers from going bankrupt.

[Prophet](https://facebook.github.io/prophet/) is a decomposable **time series model** designed for forecasting non-linear trends amongst seasonality and holiday effects. We used Prophet to project various NOAA weather variables such as average temperature, precipitation, and drought indices for Louisiana from 2000 to 2020. This model was chosen for its robustness and ability to handle irregularities in data, which are common in agricultural datasets. Our projections using Prophet achieved high accuracy, exemplified by an **R² score of 0.92** for average temperature projections.

After projecting weather variables, we used **Ridge linear regression** to predict the annual mean loss proportion for Louisiana’s rice industry. This model incorporated the weather parameters, transformed using a second-order polynomial feature generator to capture non-linear interactions. To improve our predictions, we developed a **custom formula** optimized using nonlinear least squares, which significantly enhanced our model's accuracy, achieving an **R² score of 0.83.**

The results of our models indicated a general trend of increasing loss proportions in the rice industry, primarily driven by rising temperatures and changing climatic conditions. Our findings suggest that while there may be more arable land available for rice cultivation in the short term, the long-term outlook is less optimistic, with higher loss proportions and reduced net output expected. To mitigate losses, we recommend that farmers integrate advanced technologies (such as modified seed varieties and precision farming techniques) and propose a rebate program and adjusted insurance policies to reflect technology adoption.
