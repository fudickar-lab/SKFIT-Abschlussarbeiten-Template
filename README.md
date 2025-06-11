# SKFIT-Abschlussarbeiten-Template

This is a template for writing your thesis in LaTeX at SKFIT. It is an adapted version of Prof. Tantau's default UzL template.

## Getting started

### Installing a TeX Distribution

As this template does not compile in the free version of Overleaf, you need to set up a local TeX environment. This is highly recommended anyway because you can integreate it into your git repository to use version control on your thesis.

There are a bunch of different ways to install TeX. In my opinion, the easiest is [TeXLive](https://www.tug.org/texlive/). The installation takes a while, but once it's done you're all set up.

### Configuring your Editor

Again, this is your own choice, but I would recommend using
[Visual Studio Code](https://code.visualstudio.com/) with the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension. If you're familiar with Overleaf, LaTeX workshop comes with a lot of features you already know, such as snippets and code completion.

If you're using LaTeX workshop, I highly recommend changing the following settings:

1. Auto Build -> onFileChange
2. Latex: Recipe -> lastUsed
3. Latex: Recipes -> click on "Edit in settings.json" -> In the json, move the entry containing "latexmk (lualatex)" to the top of the list

This ensures that when saving, lualatex is run as the default compilation backend.

### Testing your environment

To test your environment, do the following:

1. Fork this repository, if you haven't already
2. In VSCode, open the command palette (Ctrl+Shift+P) and look for `LaTeX Workshop: Build with recipe`
3. Choose `latexmk (lualatex)` and hit enter

The first build should take a while and generate some files. If you encounter an error during this build, there is probably something wrong with your TeX installation.

If the first build is a success (you get a checkmark in the bottom left), try adding some text to one of the chapters (e.g. Results.tex), hit save, and see if it compiles again without errors. Every compilation is going to take a bit of time, it does **not** mean that anything is wrong, necessarily.

## Tips and tricks

I have included the tutorial provided by Prof. Tantau with the template. It includes some pointers on how to work with LaTeX, and some great pointers for writing your thesis in general. I highly recommend you read it.

If you need additional packages for your thesis, include those in the Masterarbeit.tex file. There are also some comments that explain what some commands do (e.g. for changing your thesis language to German).

## Troubleshooting

The first line in your Masterarbeit.tex might throw an error (at least it does for me). In my experience, **you can safely ignore this**.

Should you encounter any further errors in the process of writing your thesis, I encourage you to:

1. Check the log file. It might give you some pointers as to which package is causing the issue
2. If the issue is with a certain file, it should be marked in red and the problem zone should be highlighted (just like when working with code)

In case there is an error you cannot fix, **or** there is an error that took you a while to fix, please do not hesitate to send me a [mail](mailto:w.philipp@uni-luebeck.de).

&copy; William Philipp, 2025
