# finalCapstone Project - Unsupervised Learning
An unsupervised learning project to explore the relationships between variables within the 'USArrests' dataset. This involves
undertaking a correlation analysis as well as principal component analysis to understand the impact that the variables have 
on the data. To prevent overfitting and to increase efficiency and interpretability, some variables may need to be removed,
so it is important to preserve as much information as possible through the remaining variables.

### Table of Contents
* [Installation](#installation)
* [Usage](#usage)

### Installation
Download the ZIP file located under the green 'Code' tab. This file should contain both the main code and the csv file with
the 'USArrests' dataset.

Extract to a folder of your choosing, and open the file.

Some of the libraries may not be installed on your system. It is necessary to ensure the installation of the necessary
libraries in order for the code to execute.

After the libraries have been installed on your system, the code should run as required.

### Usage
The code begins with an overview of the data, which is displayed in table form and a subplot of histograms showing the
distributions of each variable within the dataset, this is shown below:

<img src="https://user-images.githubusercontent.com/125564099/219648321-000a5e91-011b-490f-b097-7b213e32f95d.png">

A correlation matrix is then plotted, showing the relationships between each variable within the dataset, during PCA, these
scores will help the PCA model transform the data to the desired number of components, which in this example is 2.

<img src="https://user-images.githubusercontent.com/125564099/219648850-a08d54b8-2f73-4d3d-909e-fe52cf2b47e6.png" width=40%>

The code then uses the PCA model to generate a biplot of the data. Initially seems that 'Assault' and 'UrbanPop' variables
have too much influence over the data, so the data needed to be scaled to prevent domination.

<img src="https://user-images.githubusercontent.com/125564099/219651154-2adf7665-6d9b-4f77-9ee6-c95ff5bf7fe9.png" width=40%>

The project then continues to apply multiple clustering techniques, such as hierarchical clustering and K-means clustering.
A dendrogram with complete linkage and euclidean distancing is generated.

![image](https://user-images.githubusercontent.com/125564099/219651658-c3253681-1c08-4918-a2aa-54f0d57179f2.png)

Finally, scatterplots are generated to display the clusters that both hierarchical and K-means generate. It was found that in this
example, both clustering methods generated identical scatterplots.

<img src="https://user-images.githubusercontent.com/125564099/219651972-27417c6c-1105-4ffd-9453-cb27acc66603.png" width=80%>
