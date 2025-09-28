# Introduction
Histograms are a way to see how often certain values appear in your dataset, helping to quickly determine the answer to many statistical questions. They are widely used and are a critical tool for any scientist to have in their pocket. In Python, it's possible to quickly create histogram plots using libraries like `matplotlib`, and `pandas`. These tools allow you to not only plot the raw data but to adjust bin sizes, add labels, and layer in additional information to make your data clearer. For more power, the Python library `numpy` allows you to make histogram data structures that you can work with programmatically or plot. In this lesson, you'll learn how to:

* Create simple histograms using `matplotlib` and `pandas`

* Understand bins and learn to customize their number and sizes

* Compare multiple datasets on the same histogram

* Interpret the shapes of histograms to learn about your data.

* Use `numpy` to make histogram data structures

For this lesson, we'll be using real data taken in the University of Colorado Denver's physics program from a Gamma Spectroscopy lab. The data was collected from exposing a scintillator and photomultiplier tube to multiple different known radioactive sources with the goal of determining the composition of a final unidentified source. 

>If you are new to programming, it's recommended that you first take a few minutes to go over [this short lesson](https://det-lab.github.io/reading-documentation/) talking about how to read technical documentation.

---

Let's get started by installing the newest versions of Python, matplotlib, and pandas. [Click here to continue to the next section](01_setup.md) to setup our machine and download the necessary files for this lesson.