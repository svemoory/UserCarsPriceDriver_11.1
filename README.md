# What drives the price of a car?

### Overview:

This a a practical application assignment for PCMLAI program from Berkeley Haas to understand what factors make a car more or less expensive. The provided dataset contains information on 426K cars. As a result of the analysis, we need to provide clear recommendations to our client -- a used car dealership -- as to what consumers value in a used car. Here is the link to the [Jupyter Notebook](https://github.com/svemoory/UserCarsPriceDriver_11.1/blob/main/prompt_II.ipynb).

To frame the task, throughout our practical applications we will refer back to a standard process in industry for data projects called CRISP-DM.

### Business Understanding

The objective of the assignment is to determine the key features that determine the price of a used car and ultimately help the car dealerships to better manage their inventory. To achieve this, let's classify this business into the following data problem and try to answer them at the end.

* Identify the top features that determines the price of a used car.
* Does the year of manufacture of the used car contribute to the overall price?
* Give the green earth drive, are electric cars getting more popular and if so does the state where the car is sold drive the price of a used car?
* Are American made cars more popular than imported cars, if so which cars contribute to the price?
* Does the number of miles driven influence the price of a car?

### Data Understanding

Here is a list of the columns of the dataset:

![image](https://user-images.githubusercontent.com/28323151/205938877-71b1683b-6bcb-4347-980a-fe6238b36154.png)


After an EDA, we have identified various features to see which one qualifies to be numeric representation vs categorical. Some features show strong correlation with the price. We also need to eliminate nulls after encoding some of the categorical fields.

### Data Preparation

By splitting the data into 70:30 ratio, and creating training and test sets, five different models have been created using multiple regression alogorithms. Error and Score has been calculated to select the best model. GridSearch has been performed for cross validation.

### Evaluation

The permutation importance and the significant features driving the target (Used Car Price) extracted from the best model suggest that the newer used cars, followed by powerful engines and fewer mileage drives the price of used car. In granular level, diesel engined trucks seem to be hot sellers as well followed by American cars like gas driven ford seems to be very popular.

### Deployment (Final report)
The features in a used car that are most valued by the customers are

* Relatively newer cars with powerful engines and that have low mileage are the best sellers and can get you bang for the buck.
* For limited space dealerships, my study further indicates that Trucks/Picks up are great sellers.
* Diesel Engine cars seem to be very popular which could be a factor of higher gas prices followed by gas cars.
* American car models like Ford, Chevy preferably white(neutral color) are extremely common sell. Since people in America love to take road trips
* Family and durable cars like Toyota and Rover seems to be popular as well.
* Surprisingly Electric cars have not caught up yet, but something to look out for in the future, as it picks up.
* Luxury cars are a rare sell, so I would suggest stock it based on location.

### Next steps and recommendations
To further improve the model with better accuracy, I would recommend:

* Improve data quality, by collecting information like, number of previous owners, accident reports, safety features, service records
* Create new models using different split ratios
* Get economic data like pandemics, recession, war that can effect supply chain and potentially impact the sales.
* Also, forecast models can be build if we have sale data.
