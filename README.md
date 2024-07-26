# gene-expression-invasive-vs-noninvasive-cancer
Using both unsupervised and supervised learning techniques, we aim to analyse a random subset to explore 2000 observed gene expression levels in a dataset, with a focus on discriminating between invasive and non-invasive cancer kinds. The study employs dimension-reduction techniques such as PCA and supervised methods to analyze cancer genetic data, aiming to retain vital information while reducing complexity. Clustering methods like k-means, hierarchical clustering, and UMAP unveil inherent gene and patient groups. Supervised learning models including Logistic Regression, LDA, QDA, k-NN, Random Forest, SVM, and additional methods to predict cancer invasiveness, optimizing hyperparameters for performance. Natural group understanding enhances model robustness and prediction accuracy. This holistic approach improves cancer classification, showcasing the synergy between unsupervised and supervised machine learning in genomic data analysis.

# Introduction
The importance of statistics is increasing due to the growing amount of data from various sources. Applied statistics provides methods for collecting and analyzing data, and drawing meaningful conclusions based on findings. Most statistical learning problems can be categorized into supervised and unsupervised approaches. This project aims to analyze a random subset of 2000 gene ranks from 4948 random numbers and explore both supervised and unsupervised dimension reduction methods to improve classification models. Supported learning focuses on predicting outcomes for new data using supervised methods like logistic regression, LDA, QDA, k-NN, random forest, and SVM. Unsupervised learning operates without labelled data but can find unknown patterns and generate valuable information from unlabelled data. It can be broken down into three tasks: clustering, association, and dimension reduction.

#Preliminary Analysis
First, we start our analysis by focusing on a subset of 2000 gene expression values from a larger dataset of 4948 initial genes. This was determined by setting our seed with the largest registration number (2311712) among team members. We employed the imputation method to replace the missing values with the median of each gene variable after the check, the result showed that there were 67 missing values out of the total observations. By substituting the median for the missing values, a bias that can arise from a non-random distribution of the missing data can be avoided. This project aims to analyse gene expression using unsupervised and supervised learning techniques with the R programming language. By doing Dimension Reduction Analysis, we aim to identify significant patterns and reduce the complexity of the gene dataset. Using unsupervised learning models such as Principal Component Analysis (PCA), K-means clustering, Hierarchical clustering, and UMAP (Uniform Manifold Approximation and Projection), we identify clusters to discover natural groupings among genes and patients that could reveal distinct properties that display key biological causes of cancer. On the other hand, supervised learning will involve selecting and justifying hyperparameters and using resampling techniques for model comparison. Utilizing methods such as Logistic regression, linear discriminant analysis, Quadratic discriminant analysis, K-Nearest Neighbours (K-NN), Random Forest, Survey vector machine (SVM), and Rig regression.

#Discussion
The sample selected (2000) from a total of 4948 genes for this project, was obtained randomly but by setting a seed with the largest registration number of the group member, we carefully observed the sample and discovered we had missing observations in our data set which we handled by imputation method (replace the missing values with the median). We also noticed that the genes had too many similarities raising the issue of Multicollinearity. The project objectives are as follows:
Dimension reduction analysis, where we applied PCA as an unsupervised dimension reduction and LDA as a supervised dimension reduction technique, aided in identifying patterns within the gene dataset and reduced complexity while retaining essential information about the entire data.
Using an unsupervised learning model to observe groups of genes and patients, we used the elbow method to get the optimal number of clusters to be 3. Principal component analysis revealed underlying structure by reducing dimensionality, K-means grouped the genes and patients based on similarities, hierarchical clustering organised the genes and patients according to their hierarchy, and UMAP was used to visualize high dimensional data.
Supervised machine learning model to predict the classes of future patients, where the hyperparameter of the models were tuned to increase the efficiency of prediction, the first ten principal component data were used for this task because of the collinearity between the genes. Employing the resampling technique by splitting the data used into training and test data, modelling was done with the training data and prediction was done with the test data. Afterwards, the confusion matrix of each model to calculate the level of accuracy.

#Conclusion
We concluded that clustering in unsupervised models helps identify natural groups among genes and patients, observations from our result show that genes and patients can be clustered into 3 groups. Supervised machine learning enables us to predict outcomes based on gene expression patterns. LDA, QDA, and Random Forest were better at predicting the class of future patients. Further investigation using Cluster validation for unsupervised machine learning justifies clustering improves the machine learning model.

