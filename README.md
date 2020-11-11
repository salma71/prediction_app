# Machine learning prediction application
![CircleCI](https://img.shields.io/circleci/build/github/salma71/prediction_app?style=for-the-badge&token=781e1233134910ffefc006ea82a7fe966b5277f2)

![GitHub repo size](https://img.shields.io/github/repo-size/salma71/prediction_app?style=for-the-badge)


[![GitHub forks](https://img.shields.io/github/forks/salma71/prediction_app?style=for-the-badge)](https://github.com/salma71/prediction_app/network)

[![GitHub forks](https://img.shields.io/github/stars/salma71/prediction_app?style=for-the-badge)](https://github.com/salma71/prediction_app/network)
------

## Steps of usage

1. Fork or clone this repo to your local machine.
2. Navigate to the project directory and activate the virtualenv `source dev/bin/activate`
3. Install requirements `pip install -rrequirements.txt` from the root directory. 
4. Navigate to the packages -> regression_model then run `tox` to make sure that everything is passing. 

---------
## Basic Analyses
The following kaggle notebooks includes the complete basic analyses and EDA 
- [Data Analysis](https://www.kaggle.com/salmaeng/data-exploration-medium-post-1)
- [Feature Engineering](https://www.kaggle.com/salmaeng/feature-engineering-medium-post-2)
- [Feature Selection](https://www.kaggle.com/salmaeng/feature-selection-medium-post-3)
- [Model Building](https://www.kaggle.com/salmaeng/model-building-medium-post-4)

[Medium post part_1](https://towardsdatascience.com/exclusive-how-to-deploy-your-first-machine-learning-models-bf0a2109e522)

[Medium post part_2](https://towardsdatascience.com/how-to-deploy-your-first-machine-learning-models-part-2-9e1d0fcfb68)

[Scaffold template - starter template](https://github.com/salma71/ML_app_scaffold)

---------
Notes to consider:
* If you intended to use this project as a reference to build your own, you need to define your environmental variables in the circleci.
* Tests are disabled for this project, would appreciate if anyone raise a pull request to include them. 


## Few things to consider

I structured the scaffold based on the OOP which seperate concerns of code. 
* `processing` folder conatains any scripts for data wrangeling, cleaning, or feature engineering. 
* `trained_model` folder contains any scripts dedicated to build model, tuning or any related scripts.
* `pipeline.py` file contains all the procedures that should be done using the `sklearn.pipeline` 
* `predict.py` file dedicated for getting out the predictions
* `train_pipeline.py` file dedicated to train the model, starting from downloading the dataset, split, apply pipeline...etc. 
 

## Output:

* The resulted model is saved as a `.pkl` file versioned with the same version of the package. 
* Only one API end point is already deployed to Heroku, pull requests are welcome

------

## Future work
- [X] Build extra API end points 
- [ ] Build frontend interface using streamlit
- [ ] Complete unit tests.
- [ ] Create a configuration file for travis

------
## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


## License
[MIT](https://choosealicense.com/licenses/mit/)