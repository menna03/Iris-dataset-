# Iris-dataset-

So, this is a Python code that performs K-means clustering on the Iris dataset. It is used to group similar data points together in different clusters based on their features. Let me walk you through the code step by step:

First, we import the necessary libraries such as pandas, numpy, matplotlib, seaborn, and KMeans from the sklearn.cluster module. These libraries provide us with tools for data manipulation, visualization, and clustering.

Next, we read the Iris dataset using the pd.read_csv() function and stored it in a variable called 'iris'. We then displayed the first few rows of the dataset using the head() function.

After that, we checked for duplicates and missing values in the dataset using the duplicated() function and the isna() function. We also calculated the percentage of missing values in each column.

Moving on, we visualized the data using seaborn's relplot() function to create scatterplots of the SepalLengthCm vs SepalWidthCm and PetalLengthCm vs PetalWidthCm variables. The hue parameter is used to distinguish the three different species of Iris. We also used seaborn's pairplot() function to create pairwise scatterplots of all variables in the dataset.

Then, we preprocessed the data by converting the 'Species' column from categorical to numerical using pandas' Categorical() and cat.codes methods. We also converted the dataframe to a numpy matrix and stored the first four columns in a variable called 'data', and the 'Species' column in a variable called 'category'.

Next, we set the number of clusters to 3 and generated random centers for each cluster using numpy's mean() and std() functions.

Finally, we plotted the data using matplotlib's scatter() function. We iterated over each row of the 'data' matrix and plotted the SepalLengthCm vs SepalWidthCm variables with different colors for each species. We also plotted the randomly generated cluster centers as blue dots.
