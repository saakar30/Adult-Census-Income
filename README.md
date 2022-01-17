# Adult Census Income Prediction

## Appendix

* [Acknowledgements](#Acknowledgements)
* [About_Data](#About_Data)
* [Motivation](#Motivation)
* [Workflow](#Workflow)
* [Technologies Used](#Technologies Used)
* [Architecture](#Architecture)
* [API Interface](#API Interface)
* [Environment_Variables](#Environment_Variables)
* [Deployment_on_Heroku](#Deployment_on_Heroku)
* [FAQ](#FAQ)

## Acknowledgements

 - The prominent inequality of wealth and income is a huge concern especially in the World. The likelihood of diminishing poverty is one valid reason to reduce the world's surging level of economic inequality. The principle of universal moral equality ensures sustainable development and improve the economic stability of a nation. Governments in different countries have been trying their best to address this problem and provide an optimal solution. This study aims to show the usage of machine learning and data mining techniques in providing a solution to the income equality problem. The UCI Adult Dataset has been used for the purpose. Classification has been done to predict whether a person's yearly income in US falls in the income category of either greater than 50K Dollars or less equal to 50K Dollars category based on a certain set of attributes. 
  
## About_Data
#### Attribute Information:

Listing of attributes:

>50K, <=50K.

- age: continuous.
- workclass: Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, Local-gov, State-gov, Without-pay, Never-worked.
- fnlwgt: continuous.
- education: Bachelors, Some-college, 11th, HS-grad, Prof-school, Assoc-acdm, Assoc-voc, 9th, 7th-8th, 12th, Masters, 1st-4th, 10th, Doctorate, 5th-6th, Preschool.
- education-num: continuous.
- marital-status: Married-civ-spouse, Divorced, Never-married, Separated, Widowed, Married-spouse-absent, Married-AF-spouse.
- occupation: Tech-support, Craft-repair, Other-service, Sales, Exec-managerial, Prof-specialty, Handlers-cleaners, Machine-op-inspct, Adm-clerical, Farming-fishing, Transport-moving, Priv-house-serv, Protective-serv, Armed-Forces.
- relationship: Wife, Own-child, Husband, Not-in-family, Other-relative, Unmarried.
- race: White, Asian-Pac-Islander, Amer-Indian-Eskimo, Other, Black.
- sex: Female, Male.
- capital-gain: continuous.
- capital-loss: continuous.
- hours-per-week: continuous.
- native-country: United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands.

## Motivation

#### Product Perspective
The Adult Census Income Prediction, classified  the income category of either greater than 50K Dollars or less equal to 50K Dollars category of the person by using classification based Supervised Machine Learning algorithms.
#### Problem statement
The Goal is to predict whether a person has an income of more than 50K a year or not. This is basically a binary classification problem where a person is classified into the >50K group or <=50K group.
#### Proposed Solution
The solution here is a classification based Supervised Machine Learning model. It can be implemented by different classification algorithms (like Logistic Regression, Random Forest Classification, Decision Tree Classification, SVC, Xg-boost Classifier, Gausian NB and so on.).

Here first, we are performing Data preprocessing step, in which feature engineering, feature selection, feature scaling steps are performed and then we are going to build model.

## Benefits: 
- To discover one’s earning potential.
- To find the key areas which impact your salary.
- Salary insights for certain Job roles.

## Approach 
The classical machine learning tasks like Data Exploration, Data Cleaning, Feature Engineering, Model Building, Model Testing and Deployment. Trying out different machine learning algorithms that’s best fit for the above case.

## Technologies Used
###### Python: high-level computer programming language used to develop the project 
###### Py-Charm:	an integrated development IDE used in computer programming, for the Python language
###### Pandas: Open source data analysis and manipulation tool, for the Python programming language.
###### Numpy: Python library used for working with arrays
###### Matplotlib/Seaborn:	For data visualization and graphical plotting library for Python
###### Scikit-Learn:	Machine learning library used for the Python programming language. It features various classification, regression and clustering algorithms
###### Flask:	A web applications  framework, it's a Python module that lets you develop web applications easily
###### HTML/CSS: 	Are two of the core technologies used for building Web pages. HTML provides the structure of the page, CSS the layout for a variety of devices.
###### Heroku:	Is used as a platform as a service (PaaS) that build, run, and operate applications entirely in the cloud 
###### GitHub:	Web-based interface that used Git for the open source version control system 

## Architecture
<p align="center">
  <img src="https://github.com/xoikia/IncomePrediction/blob/main/readme%20images/architecture.jpeg" alt="architecture">
</p>

## API Interface
Our web API will be a single page. The user input and the model’s prediction will be displayed in the same page
<p align="center">
  <img src="https://github.com/xoikia/IncomePrediction/blob/main/readme%20images/interface.png" alt="API interface">
</p>
'## Environment_Variables

To run this project, you will need to add the following environment variables to your .env file :

The Code is written in Python 3.7. If you don't have Python installed you can find it here. If you are using a lower version of Python you can upgrade using the pip package, 
ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after cloning the repository:
 [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:

For pip installation:

```bash
pip install -r requirements.txt
```
For anaconda installation

```bash
conda env create -f environment.yml
```
For more refrence regarding Managing Anconda environment [click here](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-with-commands)

## Deployement_on_Heroku
Login or signup in order to create virtual app. You can either connect your github profile or download ctl to manually deploy this project.
[![](https://i.imgur.com/dKmlpqX.png)](https://heroku.com)
Our next step would be to follow the instruction given on [Heroku Documentation](https://devcenter.heroku.com/articles/getting-started-with-python) to deploy a web app.

Application Link


## FAQ

#### Q1) What’s the source of data?
##### The data for training is taken from the internship portal of ineuron.ai., but along with that data is also avialable on Kaggle.com

####  Q 2) What was the type of data?
##### The data was the combination of numerical and Categorical values.

#### Q 3) What’s the complete flow you followed in this Project?
##### Refer slide 4th for better Understanding

#### Q 4) How logs are managed?
##### We are using different logs as per the steps that we follow invalidation and  modeling like File validation log , Data 	Insertion Model Training log , prediction log  etc.

#### Q 6) What techniques were you using for data pre-processing?
- Removing unwanted attributes
- Visualizing relation of independent variables with each other and output variables
- Checking and changing Distribution of continuous values
- Removing outliers
- Cleaning data and imputing if null values are present.
- Converting categorical data into numeric values.
- Scaling the data
#### Q 7) what kind of coding statderds are used?
coding is done in modulara fasion as per python [Python Developer's Guide](https://www.python.org/dev/)


## Feedback
Hello reader if you find any bug please consider raising issue. I will try to fix it. If you like the project please give a ⭐
