# Data Analysis

## What is Jupyter Lab (Video on page)

[Source](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html)

Jupyter allows you to work with data and code together. Multiple documents and activities can be arranged side by side on your screen.

***Two modes:***

***Command*** - "designed for easily navigating and changing the framework of your notebook"

Utilizes cells to contain data

**Keyboard Shortcuts:**

`A` - Add a cell above

`B` - Add a cell below

`C` - Copy a cell

`V` - Paste a cell

`X` - Cut cell

`d d` - delete cell

`Z` - Undo

`Shift Z` - Redo

`Y` - Cell Format: Code

`M` - Cell Format: Markdown

`0 0` - Restart the kernel

***Edit*** - Press enter to edit the active cell

`Shift Enter` - Run the cell to see your edit. (Ex: if cell is in markdown format, a preview is shown. If cell is in code format, code is run)

## Numpy Tutorial

[Source](https://www.dataquest.io/blog/numpy-tutorial-python/)

NumPy - A Python data analysis package

SSV format - Semicolon Separated Values. Values are separated with a semicolon, rows are separated by starting on a new line

**Numpy 2- Dimensional Arrays** - aka a matrix

A matrix is made of rows and columns. To extract an element from the matrix, give a row number and column number.

Rank- number of dimensions

Axis - Each dimension. First axis would be rows, second axis would be columns

**Creating a Numpy Array** - elements in an array must be the same type (floats or integers).

`shape` - A property to get the number of rows and columns Ex: _nameofarray.shape_. Assign a tuple of array dimensions to reshape.

`numpy.zeros` - can be used to create an array where ever an element is zero. Useful when you need an array with a fixed size but no values.
> Ex: empty_array = np.zeros((1,2)) -An array with 1 row, 2 columns

`np.random.rand` - Creates an array where each element is randomized

**Using Numpy to Read In Files** - csv or other files can be read into arrays. Data type (integers or floats) are auto picked based on their format.

`np.genfromtxt` - function to put files into arrays.
> Ex: beverages = np.genfromtxt("beverage.csv", delimiter=";", skip_header=1)

- `delimiter=";"` - parses the fields
- `skip_header=1` - skips the header row that has a string of words

**Indexing Numpy Arrays**:

_NumPy is zero-indexed_ - First row and column are at the index of 0. Second row or column would have an index of 1, Third would be 2, etc.

Use two indexes to get an element: array[1, 2]

- > first index is rows(axis 1)
- > second index is columns(axis 2)

**Slicing Numpy Arrays**:

Use a colon (:) to select or "slice" certain elements from the array.

- Colon indicates starting index up to the ending index, does NOT include ending index. Ending index would be one index higher than the last one you want to include.

`array[0:3, 3]` - Slice starts at beginning through the 2nd rows. 3 rows total. (0,1, and 2.)

`array[:3, 3]` - Omitting 0 also starts at the beginning, a shortcut.

_Selecting all rows and columns_: Think of the grid. A row is made up of column elements, a column is made up of row elements. The semi colon is in the opposite of what you think it would be in because of how the grid is made.

`array[:, 3]` - Selects the entire fourth column. _ALL row elements go into the column_

`array[3, :]` - Selects the entire fourth row. _ALL column elements go into the row_

- `[1]` - One index is another shortcut for selecting an entire row

`array[:, :]` - Would select entire array, but is not good practice.

**Assigning Values to Numpy Arrays**: `array[1, 5] = 10`

Assigning values with slices - `array[:, 10] = 20` (this turns all values in 11th column to 20)

**1-Dimensional NumPy Arrays**



---

# Bookmark/Skim

[Source](https://www.tutorialspoint.com/numpy/index.htm)

<br>

[<<<Back](README.md)