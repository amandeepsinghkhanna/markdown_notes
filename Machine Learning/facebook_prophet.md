# Facebook Prophet Algorithm

- Prophet is an open-source algorithm designed for time-series forecasting by Facebook's core data science team [1]. It breaks down the time-series in three main components:
    
    1. Trend: Captures the long term increasing or decreasing trajectory of data, filtering out seasonal variations [2].

    2. Seasonality: Captures predictable cyclic patterns in the data at varied levels of granularity [2].

    3. Holidays: It allows to incorporate the effect of holidays on the data [2].

These components are combined with the error term to account for any unexpected fluctuation in the data [2].

The functioning of the algorithm is similar to that of Generalized Additive Models (GAMs).

$$y(t) = g(t) + s(t) + h(t) + e(t)$$

here,
    - $$g(t)$$ refers to trend (changes over a long period of time)
    - $$s(t)$$ refers to seasonality (periodic or short-term changes)
    - $$h(t)$$ refers to effects of holidays to the forecast
    - $$e(t)$$ refers to the unconditional changes that is specific to a
    business or a person or a circumstance. It is also called the error term.
    - $$y(t)$$ is the forecast.

*TODO: Read up on GAMs.*

Prophet provides us with two models:
1. Logistic growth model
2. Piece-Wise linear model

- By default it uses the piece-wise linear model.


## Resources to go through

1. Official Documentation: https://github.com/facebook/prophet
2. Official GitHub Repository: https://github.com/facebook/prophet
3. Javapoint Tutorial: https://www.javatpoint.com/time-series-forecasting-with-prophet-in-python
4. Time series forecasting using Facebook prophet by Krish Naik: https://youtu.be/VtItg-J6-CI?si=p0Ie9qnDsiVjEKtH
5. Time series forecasting with Facebook Prophet and Python in 20 minutes: https://youtu.be/KvLG1uTC-KU?si=pLHgz5BXNEP07taB
 

## References


1. https://facebook.github.io/prophet/
2. [GeeksforGeeks](https://www.geeksforgeeks.org/time-series-analysis-using-facebook-prophet/)