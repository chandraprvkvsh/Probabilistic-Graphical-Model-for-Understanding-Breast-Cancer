# Probabilistic-interpretation-of-factors-affecting-Breast-Cancer
# Brief Introduction

Objective of this project was to build a Probabilistic Graphical Model on breast cancer dataset to generate the conditional probability distributions for each factor affecting the likelihood of breast cancer. 

The project involved creating a Naive Bayes probabilistic graphical model with parent node as 'diagnosis' and the rest of features as child node then generate CPDs(conditional probability distributions) of all nodes.

Naive Bayes algorithm from PGMPY library was used.

# Details about the project

You are given a Breast Cancer Dataset, and the description of the dataset is given below: 

1) id number- Patient's ID

2) diagnosis- The diagnosis of breast tissue, where M is malignant which means tumor is cancerous and B stands for benign which means non-cancerous tumor. 

3) radius_mean- The mean of distances from center to points on the perimeter

4) texture_mean- Standard deviation of gray-scale values

5) perimeter_mean- Mean size of the core tumor

6) area_mean

7) smoothness_mean- Mean of local variation in radius lengths

8) compactness_mean- Mean of perimeter^2 / area - 1.0

9) concavity_mean- Mean of severity of concave portions of the contour

10) concave points_mean- Mean for number of concave portions of the contour

11) symmetry_mean

12) fractal_dimension_mean- Mean for "coastline approximation" - 1

13) radius_se -Standard error for the mean of distances from center to points on the perimeter

14) texture_se- Standard error for standard deviation of gray-scale values

15) perimeter_se

16) area_se

17) smoothness_se- Standard error for local variation in radius lengths

18) compactness_se- Standard error for perimeter^2 / area - 1.0

19) concavity_se- Standard error for severity of concave portions of the contour

20) concave points_se- Standard error for number of concave portions of the contour

21) symmetry_se

22) fractal_dimension_se- Standard error for "coastline approximation" - 1

23) radius_worst- Worst or largest mean value for mean of distances from center to points on the perimeter

24) texture_worst- Worst or largest mean value for standard deviation of gray-scale values

25) perimeter_worst

26) area_worst

27) smoothness_worst- Worst or largest mean value for local variation in radius lengths

28) compactness_worst- Worst or largest mean value for perimeter^2 / area - 1.0

29) concavity_worst- Worst or largest mean value for severity of concave portions of the contour

30) concave points_worst- Worst or largest mean value for number of concave portions of the contour

31) symmetry_worst

32) fractal_dimension_worst- Worst or largest mean value for "coastline approximation" - 1

The above mentioned coulmn names are the real-valued features computed for each cell nucleus.
The mean, standard error and worst or largest (mean of the three largest values) of these features are computed for each image, resulting in 30 features. For instance, field 3 is Mean Radius, field 13 is Radius SE, field 23 is Worst Radius.
All feature values are recorded with four significant digits.
Missing attribute values: none
Class distribution: 357 benign, 212 malignant


Part1: For the given Breast Cancer datasets, fit the Naive Bayes and logistic regression models. Compare their results on test set.
Carry out the following tasks:

1. Load and read ,the data from the input file data.csv
2. Remove the unwanted columns(id,unnamed 0, unnamed32)
3. Find out accuracy score by using Naive Bayes Classifier and Logistic regression model
4. Print your output to a csv file

Part2: For the Breast Cancer dataset, learn the Naive Bayes graphical model by learning a graph with ‘diagnosis’ as parent and rest of the features as ‘child’. Learn the cpds of model by fitting given data.
Things to take care:

1. Load and read the dataset
2. Remove unwanted columns(id and unnamed 32)
3. Convert all numerical features into discrete features with bins [low, med, high]. [HINT: use pandas.cut]
4. Genrate CPD of all nodes
5. Write the CPD of perimeter_worst to a csv file
