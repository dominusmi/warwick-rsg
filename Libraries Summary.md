### Linear Regression & Classification

A generic notebook describing the methods can be found [here](Scouting/Linear%20Models%20%20for%20Regression%20%26%20Classification.ipynb).

|        | [SparseRegression.jl](Scouting/Sparse%20%Regression.ipynb) |  [MultivariateStats.jl](Scouting/MultivariateStats.ipynb) | [OnlineStats.jl](Scouting/OnlineStats.ipynb) |
| ------------- |:-------------:|:-------------:|:-:|
| Package works | yes | yes | yes |
| Deprecations warnings      | No | No | No |
| Compatible with JuliaDB | If transformed into matrix | If transformed into matrix | If transformed into matrix |
| Documentation | lacking | very good | very good |
| Simplicity | good | good | High |

### SVM

Theory on support vector machines is found [here](Scouting/SupportVectorMachinesTheory.ipynb)

|        | [KSVM.jl](Scouting/KSVM.jl.ipynb) |  [LIBSVM.jl](Scouting/LIBSVM.jl.ipynb) | [SVM.jl](Scouting/SVM.jl.ipynb) |
| ------------- |:-------------:|:-------------:|:-:|
| Package works | no | yes | no |
| Deprecations warnings      | yes | No | yes |
| - | If transformed into matrix | yes | - |
| Documentation | none | yes, as inline documentation. Type ?Functionname | none |
| Simplicity | good | medium | good |


### Gradient Boosting

A notebook detailing boosting and gradient boosting is available [here](Scouting/Boosting.ipynb).
  
- LightGMB.jl a Julia interface for Microsoft's LightGBM
- XGBoost.jl an interface fo XGBoost (written in C)
- A Julia implementation of gradient boosting


|   | [LightGBM.jl](Scouting/LightGBM.jl.ipynb) |  [XGBoost.jl](Scouting/XGBoost.jl.ipynb) | [GradientBoost.jl](Scouting/GradientBoost.jl.ipynb) |
| :-: | :-: | :-: | :-: |
| Packages works            | no                               | Yes | No
| Deprecation warnings      | None                              | None | Several
| Compatible with JuliaDB   | Yes (transformation of tables to arrays required) | - |
| Documetation              | None            | Points to XGBoost docs | few examples |


### Decision Trees

A generic notebook discussing decision tree models is available [here](Scouting/Decision%20Tree%20Models.ipynb). Note:

- DecisionTrees.jl was found to be about one order of magnitude slower than the python version
- OnlineStats only has an implementation for a type of tree called FastTree (and its ensemble, the FastForest)

|   | [DecisionTrees.jl](Scouting/DecisionTree.ipynb) |  [ScikitLearn.jl](Scouting/ScikitLearn.jl.ipynb) | [OnlineStats.jl](Scouting/OnlineStats.ipynb) |
| :-: | :-: | :-: | :-: |
| Packages works            | yes                               | Yes | Yes
| Deprecation warnings      | None                              | Some | None
| Compatible with JuliaDB   | Yes (transformation of tables to arrays required) | Yes (transformation of tables to arrays required) | Yes (transformation of tables to arrays required) |
| Documetation              | None, but many examples             | very good | None |
| Simplicity                | Good, like sklearn                | good | quite low |

### Utilities

- _MLPreprocessing_ is used to do simple scaling/normalising
- _MLLabelUtils_ provides functions to modify the labels to be compatible with whatever the algorithm requires. For instance transform into categorical, booleans, from text to number etc
- MLBase provides function for label encoding, classification from model scores, performance evaluation (ROC, F1 etc),
  cross-validation (Kfold, stratified Kfold, subsmapling), and grid search hyperparameter tuning.
- MLMetrics provides model evaluation functions for regression, classification, multilabel ranking, and clustering designed
to follow python's sklearn.metrics closely.




|                       | [MLPreprocessing.jl](Scouting/MLPreprocessing.ipynb) | [MLLabelUtils.jl](Scouting/MLLabelUtils.ipynb) | [MLBase.jl](Scouting/MLBase.jl.ipynb)| [MLMetrics.jl](Scouting/MLMetrics.ipynb)|
| :- | :- | :- | :- | :- |
| Packages works            | yes | yes | yes|yes|
| Deprecation warnings      | None | No |No|yes|
| Compatible with JuliaDB   | If tables are converted to arrays or dataframes | If tables transformed into arrays |If tables transformed into arrays|yes|
| Documetation              | None, but sufficient examples | good | good | none |
| Simplicity                | Fair | good |good|good|


