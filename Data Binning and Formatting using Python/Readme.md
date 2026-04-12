# Experiment 13: Data Binning and Formatting using Python

Data binning is the process of grouping a large set of continuous numerical values into smaller "bins" or intervals to reduce the effects of minor observation errors and simplify data analysis.

Data formatting is the practice of converting raw data into a standardized, readable structure to ensure consistency and compatibility across different systems

### Aim:

To perform data binning and formatting using Python and the Pandas library in order to trasform raw continuous data into structured, interpretable and analysis - ready formats.

### Tools Used:

Google Colab, Jupyter Notebook

### Theory:

#### Introduction:

Raw datasets often contain continuous values and inconsistent formats, making them difficult to interpret directly. In real-world scenarios, such unprocessed data can lead to incorrect analysis or poor decision-making.

Data binning is a preprocessing technique that groups continuous values into discrete intervals, reducing noise and simplifying data interpretation. For instance, instead of analyzing exact marks, grouping them into ranges (e.g., Low, Average, High) makes trends easier to observe.

Data formatting, on the other hand, ensures that data is presented in a consistent and readable manner. This includes operations such as rounding numbers, converting data types, and standardizing text.

Using Python’s powerful Pandas library, both binning and formatting can be efficiently implemented, making it a fundamental step in data preprocessing pipelines used in analytics, machine learning, and reporting systems.

#### Data Binning:
Data binning converts continuous data into categorical data by dividing it into intervals. It helps in: Reducing complexity Minimizing noise Improving interpretability

#### Types of Binning:
a) Equal-Width Binning:
Divides the entire data range into intervals of equal size Simple and easy to implement May result in uneven data distribution

Implemented using: pd.cut()

b) Equal-Frequency Binning:
Each bin contains approximately the same number of observations Produces balanced groups More useful for skewed datasets

Implemented using: pd.qcut()

#### Labelling Bins:
Instead of numerical intervals, descriptive labels improve clarity.

Example:

0–50 → Low

50–75 → Medium

75–100 → High

This improves human readability and reporting quality.

#### Data Formatting:

Data formatting is the practice of converting raw data into a standardized, readable structure to ensure consistency and compatibility across different systems

It includes:
  * Rounding numerical values

  * Converting data types

  * Standardizing text (uppercase/lowercase)

  * Cleaning and structuring data

#### Type Conversion:

Common conversions:

  * int → float

  * float → int

  * object → category

Done using: astype()

#### Rounding and Precision:

Excess decimal precision can the clutter data.

Example:

Financial values rounded to 2 decimal places

Done using: round()

### Example of Code and syntax:

* Equal Width Binning:

            df['Marks_Bin'] = pd.cut(df['Marks'], bins=3)
            print(df)

* Equal Frequency Binning:

            df['Marks_Bin'] = pd.qcut(df['Marks'], q=3)
            print(df)

* Labelling Bins:

            labels = ['Low', 'Medium', 'High']
            df['Marks_Bin'] = pd.cut(df['Marks'], bins=3, labels=labels)

* Data Formatting:

            df['Marks'] = df['Marks'].astype(float)
            df['Marks'] = df['Marks'].round(2)

* String Formatting:

            df['Name'] = df['Name'].str.upper()


### Applications:

* Data preprocessing in machine learning
  
* Business analytics and reporting

* Academic grading systems

* Survey data categorization

* Dashboard and visualization preparation

### Advantages of Data Binning ad Formatting:

* Reduces complexity of large datasets

* Improves clarity and presentation

* Helps identify trends and patterns

* Enables better decision-making

* Integrates well with visualization tools

### Learning Outcomes:

* Equal-width binning created uniform ranges

* Equal-frequency binning balanced data distribution

* Labeling improved interpretability Formatting enhanced readability and consistency

### Conclusion:

Data binning and formatting were successfully implemented using Python and the Pandas library. Continuous data was categorized into meaningful intervals, and formatting techniques improved data clarity, consistency, and usability. The processed dataset is now suitable for further analysis and visualization.
