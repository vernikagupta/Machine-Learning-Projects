## Reboot: Box-Plots for Education
Competition on DrivenData
#### Current Rank in competition - 55

### Summary

Budgets for schools and school districts are huge, complex, and unwieldy. It's no easy task to digest where and how schools are using their resources. Education Resource Strategies is a non-profit that tackles just this task with the goal of letting districts be smarter, more strategic, and more effective in their spending.

Your task is a multi-class-multi-label classification problem with the goal of attaching canonical labels to the freeform text in budget line items. These labels let ERS understand how schools are spending money and tailor their strategy recommendations to improve outcomes for students, teachers, and administrators.

### Approach taken by me

* I first signed up for the competition on DrivenData site. After downloading the data from website, I loaded jupyter notebook and started   working on the project.
* By inspecting the dataset I came to know that two types of data types are present. One is object that is generic string in python and     secong is numerical(float). 
* I first made a simple model taking only numerical features.
* The next challenge was to make labels in numerical data types.
* I converted labels from string data type to categorical and from categorical to numerical using get_dummies function of pandas.
* After separating features and labels, I imported simple logistic regression and fit this model with training data and checked             accuracy on cross validated test data.
* Then, I considered Textual data and used Natural Language processing tokenization process, specifically bag of words approach to process   textual data.
* After that I used pipeline to encapsulate all the processes from raw to model in pipeline and fit model first with logistic regression.
* Checked accuracy with logistic regression.
* Imported error metric log loss from multilabel multiclass.
* Checked log loss error.
* Then, I fitted random forest model and tried different hyperparameters.

#### Result: Model with log loss error 1.0

