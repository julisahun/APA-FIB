# Study of ETH wallets using ia models

## Getting Started

### Prerequisites

The only prerequisite is to have python3 installed. 
You can download and install python from the python [website](https://www.python.org/downloads/)


### Installation

1. Open a terminal and go to the root of this project
2. Install all the modules needed using the requirements.txt file
   ```sh
   pip3 install -r requirements.txt
   ```
If this command failed for whatever reason, you can install the packages manually. The packages needed are:
* [Pandas](https://pypi.org/project/pandas/) (1.5.1)
* [Numpy](https://pypi.org/project/numpy/) (1.23.4)
* [Scikit-learn](https://pypi.org/project/scikit-learn/) (1.2.0)
* [Yellowbrick](https://pypi.org/project/yellowbrick/) (1.5)
* [Scikit-optimize](https://pypi.org/project/scikit-optimize/) (0.9.0)
* [Matplotlib](https://pypi.org/project/matplotlib/) (3.6.0)
* [Lime](https://pypi.org/project/lime/) (0.2.0.1)






## Usage

The first two cells of the notebook are used to import all modules and check the version to ensure everything is correct

The third cell is used to adjust the global parameters of the code. For now, there's only 3:
```python
    #If set to True will train all the models, otherwise, will get the data from /store
    train_models = False 

    #If set to True will store the data and models in /store to be used in future executions
    save_models = False 

    #Number of crossValidations made in Grid and Bayes search
    cv = 5
```





## Models

In this project we will be seen 6 different models, 3 of them bases on linear algorisms and 3 based on non linear algorisms.

Here is the list of the models used:

* Linear:
    * [LinearDiscriminantAnalysis](https://scikit-learn.org/stable/modules/generated/sklearn.discriminant_analysis.LinearDiscriminantAnalysis.html)
    * [LinearSVC](https://scikit-learn.org/stable/modules/generated/sklearn.svm.LinearSVC.html)
    * [KNeighborsClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)
* Non Linear
    * [SVC](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)
    * [MLPClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html)
    * [RandomForestClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
