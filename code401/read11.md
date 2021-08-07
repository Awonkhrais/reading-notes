# What is Jupyter Lab

* JupyterLab is a next-generation web-based user interface for Project Jupyter.

* JL enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals and custom components in a flexible, intergrated, and extensible manner.

* All popular image formats are supported as standalone files and in notebooks.

* JSON files can be edited as cell outputs or searchable tree views.



# Numpy

* Numpy is a commonly used Python data analysis package. It allows you to speed up your workflow and interface with other packages in the Python ecosystem.

* Almost every data analysis or machine learning package for Python uses Numpy in some way.

## Numpy to Read In Files

It's possible to use Numpy to directly read csv or other files into arrays. We can do this by the `numpy.genfromtxt` function. Use it to read our initial data on red wines.

Use the `genfromtxt` function to read in the `winequality-red.csv` file.


## Alternative Methods for Creating NumPy Arrays with Numeric Elements

- `numpy.zeros(x,y)` - Makes an array with x/y dimensions where every element is an integer 0.
- `numpy.ones(x,y)` - Makes an array with x/y dimensions where every element is an integer 1.
- `numpy.random.rand(x,y)` - Makes an array with x/y dimensions where every element is an random floating point number.
- `np.genfromtxt("[file_name]", delimiter="[character]", skip_header=1)` - Reads data from a file directly into an array.