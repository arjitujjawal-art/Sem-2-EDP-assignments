# Experiment - 18: Data Visualization using Advanced Graphs

Complex visualization in Python involves using libraries like Plotly, Bokeh, or Seaborn to create multi-dimensional, interactive, or hierarchical charts that go beyond standard bar and line graphs. These techniques, such as treemaps or 3D plots, are used to uncover hidden patterns and relationships within large, high-dimensional datasets that simple visuals cannot capture. By providing interactivity and depth, they allow stakeholders to intuitively explore data and make more informed, data-driven decisions.

## 🎯 Aim
To visualize Data using Advanced Graphs.

## 🛠️ Tools Used
* Google Colab or Jupyter Notebook

## 📚 Theory

To visualize data using Advanced Graphs, certain libraries are needed other than Seaborn and matplotlib. These are:

* **`plotly.express`**: A high-level interface for Plotly that allows for rapid creation of complex, interactive figures with minimal code. In this notebook, it is specifically used to generate a Treemap to visualize department budgets.
* **`scipy.cluster.hierarchy`**: A module used for hierarchical and agglomerative clustering. The notebook utilizes its linkage and dendrogram functions to compute the relationships between data points and visualize them as a Dendrogram.
* **`matplotlib_venn`**: A library designed for plotting area-weighted Venn diagrams. While mentioned in your list, this specific notebook primarily focuses on advanced graphs like Treemaps and Dendrograms for visualization.
* **`plotly.graph_objects`**: A lower-level interface to Plotly that provides more granular control over figure customization and structure. It is the foundation upon which Plotly Express is built, offering more flexibility for intricate chart designs.

### Advanced Graphs

Traditional charts like bar charts and line graphs are useful for visualizing basic trends. Advanced graphs are essential for uncovering hierarchical structures, multi-dimensional relationships, and complex data flows.

#### 1. Treemap
A Treemap is a visualization that represents hierarchical data using nested rectangles.
**Key Features:**
* Each rectangle represents a category.
* Size of rectangle = value of data.
* Smaller rectangles are inside larger ones.

#### 2. Dendrogram
A Dendrogram is a tree-like diagram used to show hierarchical clustering.
**Key Features:**
* Shows how data points are grouped.
* Branches represent clusters.
* Height shows similarity/distance.

#### 3. Venn Diagram
A Venn Diagram shows relationships between sets using overlapping circles.
**Key Features:**
* Each circle = a set.
* Overlapping area = common elements.
* Non-overlapping = unique elements.

#### 4. Heatmap
A heatmap is a graphical representation of data where values are shown using colors.
**Key Features:**
* Show correlationship between variables.
* Identify patterns quickly.
* Highlight strong/weak correlations.

#### 5. 3D Scatter Plot
A 3D scatter plot is used to display the relationship between three numerical variables.
* **X-axis** → first variable
* **Y-axis** → second variable
* **Z-axis** → third variable

**Key Features:**
* Analyze 3 variables at once.
* Identify patterns in multi-dimensional data.
* Used in scientific and business analysis.

#### 6. Sankey Diagram
A flow diagram in which the width of the arrows is proportional to the flow rate. It visualizes the transformation and movement of data between multiple states or nodes.
**Key Features:**
* Proportional Link Width.
* Flow Conservation.
* Visualizing Many-to-Many Mappings.

#### 7. Radar Chart
A 2D chart that displays multivariate data on three or more quantitative variables represented on axes starting from the same central point.
**Key Features:**
* Common Central Origin.
* Comparison of multiple entities in the same graph.
* Pattern & Outlier Detection.

## 🎓 Learning Outcomes
* Implementation of Hierarchical Visualizations
* Mastery of Clustering Visuals
* Proficiency in Python Visualization Libraries

## 🚀 Applications
* **Corporate Finance**
* **Data Science & Machine Learning:** Using Dendrograms to determine the optimal number of clusters for algorithms like K-Means or Agglomerative Clustering.
* **Biological & Genetic Research:** Identifying similarities between different species or gene expressions based on multi-dimensional feature sets.

## ✨ Advantages
* **Space Efficiency:** Treemaps allow for the display of hundreds of categories in a compact space while maintaining the ability to see part-to-whole relationships.
* **Clarity in Relationships:** Dendrograms provide a clear visual map of how individual data points or groups are related based on their mathematical similarity (distance).
* **Interactivity:** Using tools like Plotly provides dynamic features (hovering for data labels) that static charts cannot offer, making data exploration more intuitive.

## 📝 Conclusion
This experiment demonstrates the effective use of advanced Python libraries like Plotly and SciPy to visualize complex hierarchical and clustered data through Treemaps and Dendrograms and the output is verified.
