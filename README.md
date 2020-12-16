# Airbnb Price Recommender
#### Javier Rando Ramírez

This repository contains the code to build a Airbnb price recommender for new listings. The idea is building a tool that based on historical information, is able to help new users choose a price for their property. On top of that, it uses [SHAP Values](https://github.com/slundberg/shap) to explain the prediction to the users. This way, we ensure user trust.

### Predictions
Our recommender will predict two different prices: `minimum price` and `total_price`. The first one accounts for the minimum occupancy of the property while the second, accounts for the price considering full occupancy.

![Sample Prediction](https://github.com/javirandor/airbnb-barcelona-price-predict/blob/main/others/Pipeline_Sample.png)

### Execution
If you want to test the system, you can directly execute the predictor with `Execute_Recommender.ipynb`. The models and scaler were included in the repository in pickled version.

Otherwise, you may want to:
1. Collect the data from Inside Airbnb: `Scrapper.ipynb`.
2. Build and fine-tune your own model: `Training_Models.ipynb`.
3. Execute your own recommender: `Execute_Recommender.ipynb`.

### Models
The best performing models that were chosen are Random Forests. More details about the hyperparameter selection can be found in `Report.pdf`.
