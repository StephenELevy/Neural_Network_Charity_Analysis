# Neural_Network_Charity_Analysis

## Use Binary Classification through application of Neural Networks to determine if applicants will be successful if they are funded by the AlphabetSoup Charity.

## 4 Deliverables:

 ##  Deliverable 1: Preprocessing of Neural Network Data.
        * Working with AlphabetSoupCharity.ipynb file in Jupyter Notebook.
        * Load "charity_data.csv" into notebook and build "application_df" DataFrame.
        * "IS_SUCCESSFUL" column is the target (dependent variable).
        * All columns except "IS_SUCCESSFUL, EIN, AND NAME" are features (independent variables).
        * Drop "EIN" and "NAME" columns. 
        * Determine the number of unique values for each categorical variable in DataFrame.
        * Apply bucketing to "APPLICATION_TYPE" and "CLASSIFICATION" columns.
        * Encode the columns corresponding to the categorical variable.
        * Create our features (X) and target (y) arrays.
        * Split X and y into training and testing datasets.
        * Apply StandardScaler() to X_train and X_test.

 ##  Deliverable 2: Compute, Train, and Evaluate a Neural Network Model.
        * Define neural net sequential model - # input features, # nodes for each hidden layer, and output layer.
        * Compile Model
        * Create written output for hidden layer weights.
        * Create callback function for hidden layer weights.
        * Fit/train model.
        * Output accuracy/loss for model.
        * save model to "AlphabetSoupCharity.h5"


 ##  Deliverable 3: Optimize the Neural Network Model.
        * Create 3 modified nn models & 1 Random Forest Classifier in effort to optimize accuracy results.
        * Mod1 - 1st hidden layer has 128 nodes and 2nd hidden layer has 64 nodes. "relu" activation for both.
        * Mod2 - 1st hidden layer has 128 nodes and 2nd hidden layer has 64 nodes. "tanh" activation for both.
        * Mod3 - 1st hidden layer 128 nodes, 2nd hidden layer 64 nodes, and 3rd hidden layer 32 nodes. "tanh, tanh, and relu" activation functions, respectively.
        * Saved weights and made callbacks for each of the 3 NN models. 
        * Saved each of the 3 NN models in .h5 files - "AlphabetSoupCharity_Optimization_del3-1.h5", "AlphabetSoupCharity_Optimization_del3-2.h5", and "AlphabetSoupCharity_Optimization_del3-3.h5"
        * Random Forest Classifier with 128 estimators.
        * Created confusion matrix and classification chart for Random Forest Output.
        * see "AlphabetSoupCharity_Optimization.ipynb" file to see setups for NN & Random Forest models.

 ##  Deliverable 4: Written report on Neural Network Modeling.
        * The NN Models for Deliverables 2 & 3 had accuracy values around 73%.
        * The 3 NN Models in Deliverable 3 did not improve accuracy compared to Deliverable 2.
        * The accuracy from the Random Forest output was about 71%.
        * Used a .loc function to exclude rows with high values in "ASK_AMT" column, but made accuracy worse (not shown).
        * Also tried to scale down "ASK_AMT" values by 1000 before StandardScaler() but provided no accuracy improvement (not shown).
        * I suspect some of the feature variables contain outliers but no time to clean further.



