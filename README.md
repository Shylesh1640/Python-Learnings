# Python Learnings

This repository is a collection of Jupyter notebooks that serve as a practical guide to various fundamental and advanced concepts in Python, with a focus on data science libraries. Each notebook is a self-contained tutorial on a specific topic, from basic Python features to powerful data manipulation and visualization techniques.

---

## Table of Contents

1.  [Core Python Concepts](#core-python-concepts)
    *   [functions.ipynb](#functionipynb)
    *   [lambda.ipynb](#lambdaipynb)
    *   [list.ipynb](#listipynb)
    *   [iterators.ipynb](#iteratorsipynb)
    *   [string.ipynb](#stringipynb)
    *   [filter function.ipynb](#filter-functionipynb)
    *   [maping functions.ipynb](#maping-functionsipynb)
2.  [Data Science Libraries](#data-science-libraries)
    *   [numpy and its functions.ipynb](#numpy-and-its-functionsipynb)
    *   [pandas and its functions.ipynb](#pandas-and-its-functionsipynb)
    *   [matplotlib.ipynb](#matplotlibipynb)
    *   [seaborn.ipynb](#seabornipynb)
    *   [eda.ipynb](#edaipynb)
3.  [Utilities](#utilities)
    *   [pyforest.ipynb](#pyforestipynb)

---

## Core Python Concepts

### `function.ipynb`
This notebook provides a comprehensive introduction to functions in Python.
- **Key Concepts**:
  - **Basic Function Definition**: How to define and call simple functions.
  - **`print` vs. `return`**: A clear demonstration of the difference between functions that display output and those that return values.
  - **Arguments**: Covers positional, default, and keyword arguments.
  - **`*args` and `**kwargs`**: Explains how to create functions that can accept a variable number of positional and keyword arguments, a crucial concept for writing flexible code.
  - **Practical Example**: Includes a function to calculate the sum of even and odd numbers in a list.

### `lambda.ipynb`
A concise guide to lambda functions, also known as anonymous functions.
- **Key Concepts**:
  - **Syntax**: Compares a standard function definition with the equivalent lambda function to highlight its compact syntax.
  - **Use Cases**: Shows how to use lambda functions for simple operations like addition and conditional logic (e.g., checking for even numbers).
  - **Multiple Arguments**: Demonstrates that lambda functions can accept multiple arguments.

### `list.ipynb`
This notebook focuses on one of Python's most powerful features for working with lists: list comprehensions.
- **Key Concepts**:
  - **Traditional vs. Comprehension**: Contrasts the standard `for` loop method of creating a list with the more elegant and efficient list comprehension syntax (`[expression for item in iterable]`).
  - **Conditional Logic**: Shows how to embed `if` conditions within a list comprehension to filter items, with examples for squaring only even or odd numbers.

### `iterators.ipynb`
An explanation of the fundamental concepts of iterables and iterators in Python.
- **Key Concepts**:
  - **Iterable vs. Iterator**: Clarifies that an iterable is an object that can be looped over (like a list), while an iterator is an object that produces the next value in a sequence.
  - **`iter()` and `next()`**: Demonstrates how to get an iterator from an iterable using the `iter()` function and how to retrieve subsequent items using the `next()` function.
  - **Iterator Exhaustion**: Shows that an iterator can only be consumed once.

### `string.ipynb`
This notebook covers basic string manipulation and formatting in Python.
- **Key Concepts**:
  - **Basic Print**: A "hello world" example.
  - **`.format()` method**: Demonstrates how to use the `.format()` method to insert variables into a string, including controlling the order of insertion.

### `filter function.ipynb`
A short tutorial on the built-in `filter()` function.
- **Key Concepts**:
  - **Functionality**: Explains that `filter()` constructs an iterator from elements of an iterable for which a function returns true.
  - **Examples**: Shows how to use `filter()` with both a pre-defined function and a lambda function to extract even numbers from a list.
  - **Comparison with `map()`**: Includes a `map()` example to highlight the difference in their outputs.

### `maping functions.ipynb`
This notebook provides a clear and simple introduction to the `map()` function.
- **Key Concepts**:
  - **Functionality**: Explains that `map()` applies a given function to every item of an iterable and returns a map object (an iterator).
  - **Example**: Demonstrates how to apply a function that classifies numbers as "Even" or "Odd" to a list of integers.

---

## Data Science Libraries

### `numpy and its functions.ipynb`
An essential introduction to NumPy, the foundational package for numerical computing in Python.
- **Key Concepts**:
  - **Array Creation**: Creating 1D and 2D arrays from lists.
  - **Array Manipulation**: Using `.shape` to check dimensions and `.reshape()` to change them.
  - **Indexing and Slicing**: Accessing and subsetting data in 1D and 2D arrays.
  - **Array Creation Routines**: Using functions like `np.arange()`, `np.linspace()`, and `np.ones()`.
  - **Broadcasting and Copying**: Understanding how NumPy performs element-wise operations and the importance of using `.copy()` to avoid modifying original arrays.
  - **Conditional Selection**: Using boolean arrays to filter data.
  - **Random Number Generation**: An overview of `np.random.rand()`, `randn()`, and `randint()`.

### `pandas and its functions.ipynb`
A comprehensive tutorial on Pandas, the primary library for data manipulation and analysis in Python.
- **Key Concepts**:
  - **DataFrame and Series**: Creating a `DataFrame` from scratch and understanding its structure.
  - **I/O Operations**: Reading from and writing to CSV (`.read_csv()`, `.to_csv()`) and JSON (`.to_json()`). It also covers reading from in-memory strings (`StringIO`) and URLs.
  - **Data Access**: Detailed examples of using `.loc` (label-based) and `.iloc` (integer-based) for selecting and slicing data.
  - **Data Inspection**: Using `.head()`, `.describe()`, `.info()`, and `.value_counts()` to explore and understand a dataset.
  - **Handling Missing Data**: Using `.isnull().sum()` to identify missing values.
  - **Conditional Filtering**: Selecting rows based on data conditions (e.g., `df[df['y'] > 100]`).

### `matplotlib.ipynb`
A hands-on guide to Matplotlib, the most widely used plotting library in Python.
- **Key Concepts**:
  - **Plot Types**: Demonstrates how to create a variety of common plots:
    - **Scatter Plots** (`plt.scatter()`)
    - **Line Plots** (`plt.plot()`)
    - **Bar Plots** (`plt.bar()`)
    - **Histograms** (`plt.hist()`)
    - **Box Plots** (`plt.boxplot()`)
    - **Pie Charts** (`plt.pie()`)
  - **Customization**: Shows how to add titles, labels, colors, and line styles to make plots more informative.
  - **Subplots**: Explains how to arrange multiple plots in a single figure using `plt.subplot()`.
  - **Saving Plots**: How to save a figure to a file with `plt.savefig()`.

### `seaborn.ipynb`
An introduction to Seaborn, a high-level visualization library based on Matplotlib that provides a more attractive and informative statistical plotting interface.
- **Key Concepts**:
  - **Statistical Plots**:
    - **`heatmap()`**: Visualizing correlation matrices.
    - **`jointplot()`**: Combining bivariate and univariate views of data.
    - **`pairplot()`**: Creating a matrix of scatterplots to see relationships across an entire dataset. The `hue` parameter is used to add a categorical dimension.
    - **`distplot()`**: Visualizing the distribution of a single variable (now deprecated).
  - **Categorical Plots**: Visualizing relationships between numerical and categorical data.
    - **`countplot()`**: Counting occurrences of categories.
    - **`barplot()`**: Showing the central tendency of data.
    - **`boxplot()` and `violinplot()`**: Comparing distributions across categories.

### `eda.ipynb`
This notebook is a complete case study of Exploratory Data Analysis (EDA) on the Titanic dataset. It integrates many of the concepts from Pandas, Matplotlib, and Seaborn.
- **Workflow**:
  - **Data Loading and Initial Inspection**: Using `.head()` and `sns.heatmap(df.isnull())` to find missing data.
  - **Data Cleaning**: Imputing missing 'Age' values based on 'Pclass' and dropping the 'Cabin' column.
  - **Visualization**: Extensive use of Seaborn plots (`countplot`, `distplot`, `boxplot`) to understand relationships between variables like survival, sex, class, and age.
  - **Feature Engineering**: Converting categorical variables ('Sex', 'Embarked') into numerical dummy variables using `pd.get_dummies()`.
  - **Model Building**: A basic machine learning model is built using `LogisticRegression` from Scikit-learn to predict survival.
  - **Evaluation**: The model's performance is assessed using `classification_report` and `confusion_matrix`.

---

## Utilities

### `pyforest.ipynb`
A brief demonstration of the `pyforest` library.
- **Key Concept**: `pyforest` provides the convenience of lazy-importing popular data science libraries, meaning you can use libraries like `pandas` and `numpy` without explicitly writing the import statements at the top of your script. The `active_imports()` function is used to show which imports were triggered.