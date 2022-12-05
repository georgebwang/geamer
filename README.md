# Geamer
This is a self-made minimalist LaTeX Beamer theme. Please check out the working example ([PDF](example.pdf)) for the layout features. 


## Usage

For a one-time use, simply copy the `geamer.tex` template/preamble file into the directory where your main Beamer `.tex` file is located at. Type `\input{geamer.tex}` in the preamble of your Beamer file to use the theme.

To conveniently allow for repetitive usage, copy the `geamer.tex` file into your preferred directory in your operating system, and then include the following commands in the preamble of your main Beamer file:

```
\usepackage{import} % to import files from other directories

\import{/path/to/geamer/file/}{geamer.tex}
```
For the `\import` command, type the full path of the directory in which your `geamer.tex` file is stored in the first set of braces. For example, if you stored the `geamer.tex` file in `"C:\Users\xxx\Documents\geamer.tex"` then for the `\import` command type the following: `\import{C:/Users/xxx/Documents/}{geamer.tex}`. **Important note to Windows users:** note that one must use *trailing slashes* when defining path in LaTeX files. Windows paths use forward slashes (`\`) by default, and you need to replace those with trailing slashes (`/`) in your path definition to avoid causing compilation errors.  
