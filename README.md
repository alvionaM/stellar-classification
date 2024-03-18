<div id="header" align="center">
    <img alt="Stars and Moon" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExa3R0cjFjdGNsazNwdWhrbHg0MnpiNnlwY3FpdG5yMTliaG5zbGI0ZCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/j1tWwa9isoleIIZDmr/giphy.gif" height="200"">
</div>

## Description📌
The objective of this project is to implement and apply various machine learning algorithms to a chosen multi-class classification task. More specifically the assignment includes the implementation and application of the following algorithms: 

1. Principal Component Analysis
2. Least Squares
3. Logistic Regression
4. K Nearest Neighbors
5. Naïve Bayes
6. Multilayer Perceptron
7. K-Means

Each algorithm serves a specific purpose, ranging from dimensionality reduction (1) to classification (2-6) and clustering (7). When necessary, $\LaTeX$ is used to show the relevant mathematical background for each algorithm. The results obtained from these implementations provide insights into the performance of each algorithm in the context of the chosen classification task. After developing the algorithms, comparisons are made with ready-made implementations.

### Stellar Classification Dataset - SDSS17 🌙🌌
The data consists of 100,000 observations of space taken by the SDSS (Sloan Digital Sky Survey). Every observation is described by 17 feature columns and 1 class column which identifies it to be either a $\color{teal}Galaxy$, $\color{magenta}Star$, $\color{violet}Quasar Object$.

In astronomy, stellar classification is the classification of stars based on their spectral characteristics. The classification scheme of galaxies, quasars, and stars is one of the most fundamental in astronomy. The early cataloguing of stars and their distribution in the sky has led to the understanding that they make up our own galaxy and, following the distinction that Andromeda was a separate galaxy to our own, numerous galaxies began to be surveyed as more powerful telescopes were built. This datasat aims to classificate stars, galaxies, and quasars based on their spectral characteristics.

## Interact with the project 💻
This project consists of a Jupyter Notebook (`/notebooks/Stellar_Classification_Project.ipynb`) with all code cells already ran, so that you can easily examine the data visualizations, the algorithms' performance displayed on the relative classification reports and other results. Also, you can find the dataset in csv form (`/resources/star_classification.csv`).


## Project Structure 🧱
The project consists of the following sections:
1. **Introduction**
2. **Imports**
3. **Fetch Data**: In this section the star classification dataset is loaded. The dataset consists of 100.000 cases. Therefore, for the sake of speed the algorithms are applied on a randomly chosen sample of 20.000 cases. Then we review the dataset and decide on the features that are going to be used in the analysis. Lastly, the data is visualized using various types of diagrams.

4. **General Purpose Methods**: This section contains three subsections (*Distance*, *Curves* and *Reporting Tables*) each one of which defines a class and respective methods. As the section heading suggests, these are general purpose methods used in various sections later in the project.  

5. **Principal Component Analysis (PCA)**: An algorithm used for dimensionality reduction. The structure is the following:
    - First, the relevant mathematical/theoretical background is presented.
    - Then, a class is defined containing the methods needed for the algorithm's custom implementation. Also, other relevant useful functions are defined outside of the class.
    - Following is an *Execution* subsection where first the custom implementation and then the Scikit-Learn's implementation is applied on the data. 

        | custom                    | scikit-learn                                        |              
        |---------------------------|-----------------------------------------------------|
        | PCACustom      |  <a href="https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html">PCA</a>                                        | 

    - Lastly, an *Observations* subsection is included consisting of comparison results and other observations.

6. to 10. **All Classification Algorithms**: These sections share a common structure described below:
     - First, the relevant mathematical/theoretical background is presented (when necessary).
     - Then, a class is defined containing the methods needed for the algorithm's custom implementation. Typically each class contains a `fit` and a `predict` method, as well as any auxiliary methods needed. Also, other relevant useful functions are defined outside of the class.
     - Following is a *Training & Testing* subsection. If the algorithm has any hyperparameters, those are tuned in this subsection. After that, first the custom implementation and then the Scikit-Learn's implementation is applied on the data for both the training and the testing set. For each of these cases, a classification report is presented for performance comparisons.

         | custom                    | scikit-learn                                        |              
        |---------------------------|-----------------------------------------------------|
        | LeastSquares      |  <a href="https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.RidgeClassifier.html">RidgeClassifier</a>                                        | 
        | LogisticRegressionClassifier  |  <a href="https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html">LogisticRegression</a>               |
        | kNN      |  <a href="https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html">KNeighborsClassifier</a>                                        | 
        | GaussianNaiveBayes      |  <a href="https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.GaussianNB.html">GaussianNB</a>                                        | 
        | MlpCustomClassifier      |  <a href="https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPClassifier.html">MLPClassifier</a>                                        | 

     - Lastly, an *Observations* subsection is included consisting of comparison results between the two implementations (custom and Scikit-Learn's) and other observations.

<ol start="11">
    <li><b>K-means Clustering</b>: An algorithm used for clustering. The structure is as follows:
        <ul>
            <li> First, the relevant mathematical/theoretical background is presented. </li>
            <li> Then, a class is defined containing the methods needed for the algorithm's custom implementation </li>
            <li> Following is a <i>Training & Testing</i> subsection. First the custom implementation and then the Scikit-Learn's implementation is applied on the data for both the training and the testing set. For each of these cases, a cost evolution diagram, the values of the <i>ARI</i>, <i>AMI</i>, <i>FM</i> metrics as well as pair-plot colored by actual class and learned cluster are displayed for performance comparisons. 
                <table>
                    <thead>
                        <tr>
                        <th>custom</th>
                        <th>scikit-learn</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                        <td>kMeans</td>
                        <td><a href="https://scikit learn.org/stable/modules/generated/sklearn.cluster.KMeans.html">KMeans</a></td>
                        </tr>
                    </tbody>
                </table>
            </li>
            <li> Lastly, an <i>Observations</i> subsection is included consisting of comparison results and other observations. </li>
        </ul>
    </li>
</ol>

## Contributors
- Alviona Mancho [<a href="https://github.com/alvionaM">alvionaM</a>]
- Panagiotis Triantafillidis [<a href="https://github.com/Panattack">Panattack</a>]


