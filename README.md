## Step 1: Pre modelling  Data Prep

### Data Prep steps include:

##### Row Granularity: 
Use some python functions; groupby(), to combine all records with the sane ID columns in a single row.

Use .pivot() function to transform data from a long format to a wide format based on the requirement

##### Column Preparation

After setting the row granularity, you need to prepare the columns for modelling.

-All values must be non-null by identifying, removing or imputing the missing values, using .info(), isna()

All values must be numeric data type by converting the fields from text data types to numeric datatype. Turn filed into numerical fields by using conditional logic with np.where() function,
and turn categorical fields into numerical fields using dummy variable

#### Feature Engineering
some of techiques are applying calculations, binning values, identifying proxy variables and so on

#### Feature selection and feature scaling
In feature selection, we exclude unique identifiers such as names, IDs. Use your intuition based on the the goal of the analysis to select the right features.

Feature scaling has two major techniques, Normalisation and standardization.

With Normalisation, it transforms all columns to be between o and 1  or -1 to 1, while with standardization, it transforms all columns to have mean 0 and standard deviation to be 1
