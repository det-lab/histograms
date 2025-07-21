# Understanding Histograms
A **histogram** is a type of graph used to represent the distribution of a set of numerical data. Unlike a line or a bar graph where each value or category is plotted directly, a histogram groups data into ranges, called **bins**, and then counts how many data points fall into each range. This makes it especially useful for identifying patterns in large datasets such as:

* Where are the values concentrate?

* Are there clear peaks?

* Are there gaps or outliers?

* What's the range and shape of the data distribution?

In the case of gamma spectroscopy, each detection event is recorded at a specific **channel** number which corresponds to a range of **photon energies**. Because there are often hundreds or thousands of individual channels, plotting each one as a bar is more likely to be overwhelming and noisy for elements which aren't as strongly radioactive. A histogram helps us view the overall shape of the data.
## Bins
**Bins** divide the range of x-values (channel numbers here) into equal-width segments. Each bin groups all the data points that fall within its range and tallies how many there are, giving the y-axis of a histogram plot. For example, as the detector used 2048 channels, if you decided to use 128 bins for the data each bin would represent 16 adjacent channels/energy levels.

Choosing the right number of bins is a balance between **detail** and **readability**:

* More bins $\to$ More detail, higher resolution, but potentially noisier. This may help you resolve closely spaced peaks, but it can also amplify noise or fluctuations.

* Fewer bins $\to$ Smoother curve, but less resolution. This can help to clarify general trends and reduce noise, but it may blur out small but relevant peaks.

You can experiment with different bin settings depending on what it is that you want to analyze. To locate a peak: start with more bins. To estimate the general shape: start with fewer bins.
## Shape of the Data
Histograms are useful for diagnosing the statistical nature of your data. A single sharp peak may indicate a well-isolated energy level. A broad peak could point to resolution limitations or overlapping emissions. A tail or skew might suggest background noise, scattering effects, or data artifacts. Understanding such shapes will help in interpreting physical results and deciding whether additional calibration or filtering might be needed. 

Histograms come in six possible variations:

* Symmetric

![wiki symmetric](https://upload.wikimedia.org/wikipedia/commons/1/15/Symmetric-histogram.png)


* Skewed right

![wiki skewed right](https://upload.wikimedia.org/wikipedia/commons/1/12/Skewed-right.png)

* Skewed left

![wiki skewed left](https://upload.wikimedia.org/wikipedia/commons/7/7b/Skewed-left.png)

* Bimodal

![wiki bimodal](https://upload.wikimedia.org/wikipedia/commons/7/7a/Bimodal-histogram.png)

* Multimodal

![wiki multimodal](https://upload.wikimedia.org/wikipedia/commons/3/39/Multimodal.png)

In a histogram plot, the tallest bar represents the data's **mode** (usually - this can be incorrect if the bin size is poorly chosen or the data is especially noisy). 

In a symmetric plot the **mean**, **median**, and **mode** should all occur near the same point. 

In a skewed plot, the **mean** and **median** typically shift towards the direction of the skew. 

* Right skew: mean > median > mode

* Left skew: mean < median < mode

For bimodal and multimodal plots, the **mean** and **median** do not necessarily fall at one of the peaks, and can even lie **between the modes** depending on the relative height and width of the peaks. So they can become harder to visualize from the plot alone in this case.

## When Not to Use a Histogram
Histograms are best when your data is continuous or pseudo-continuous, and when you care about frequency distributions. If you're comparing a small number of distinct categories, a bar chart is likely a better choice. 

---

Now that we have a basic understanding of how to use histograms, [click here to continue to the next section](03_plotting_data.md) where we can try creating one and comparing it to a bar graph using our spectroscopy data.