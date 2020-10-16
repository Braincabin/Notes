- [Supervised vs Unsupervised learning](#supervised-vs-unsupervised-learning)
- [Regression and Classification](#regression-and-classification)
  - [Regression](#regression)
  - [Classification](#classification)

### Supervised vs Unsupervised learning

| Basis                   | Supervised learning                                                                                         | Unsupervised learning                                                                                                    |
| ----------------------- | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Input data              | Labelled                                                                                                    | Not labelled                                                                                                             |
| Expected model behavior | Model learns from the given input and tries to minimize inaccuracy using a cost function                    | Model tries to find similarities or groups within the input and automatically analyze groups or similarities in the data |
| Example use case        | Training by looking at labelled dog and cat pictures and finding if an unseen picture contains a dog or cat | To group news articles into similar categories without any labels                                                        |

### Regression and Classification

#### Regression

Regression is used to predict the output when the input and label values are a continuous range of numbers

Example:

-   Predict the cost of a house of square feet `x` area, given a dataset with:
    -   area of houses sold (Function input)
    -   price at which they were sold (Expected output)
    Since the inputs and outputs are a continuous series of values, we can use a Regression model to solve this problem


#### Classification

Classification is used when the input has to be classified into either one of the **possible outputs**

Example:
-   Predict whether the given number is `even` or `odd`, given a dataset with:
    -   input numbers (Function input)
    -   whether the number is `even` or `odd` (Expected output)
    Since we're trying to **classify** the number as `even` or `odd`, we use a Classification model to solve this problem