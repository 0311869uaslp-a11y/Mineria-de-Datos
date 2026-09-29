# Data Mining

Repository containing exercises, analyses, and practical work developed during my academic training in **Data Mining** as part of the **Data Science & Artificial Intelligence program at Universidad Autónoma de San Luis Potosí (UASLP)**.

The coursework focuses on the complete process of extracting useful information from structured datasets, including **data preprocessing, missing-value treatment, outlier analysis, normalization, exploratory analysis, correlation analysis, dimensionality reduction, regression, clustering, and association-rule mining**.

The repository demonstrates the transition from raw data to interpretable patterns and predictive or descriptive analytical results.

---

## Course Overview

Data Mining combines statistical, computational, and Machine Learning techniques to discover patterns and useful information in datasets.

A typical workflow can be represented as:

```text
Raw Data
   |
   v
Data Understanding
   |
   v
Data Cleaning
   |
   v
Preprocessing
   |
   v
Exploratory Analysis
   |
   v
Feature Analysis
   |
   +-------------------+
   |                   |
   v                   v
Supervised          Unsupervised
Methods               Methods
   |                   |
   v                   +----------+
Regression             |          |
                       v          v
                     PCA       K-Means
                                  |
                                  v
                         Pattern Discovery
                                  |
                                  v
                         Association Rules
```

---

# Topics Covered

The repository includes practical work related to:

- Data preprocessing
- Data cleaning
- Missing values
- Outlier detection and analysis
- Data normalization
- Exploratory Data Analysis
- Descriptive statistics
- Correlation analysis
- Feature relationships
- Principal Component Analysis (PCA)
- Dimensionality reduction
- Regression
- K-Means clustering
- Unsupervised learning
- Association rules
- Pattern discovery
- Data visualization
- Interpretation of analytical results

---

# Data Preprocessing

A significant part of Data Mining occurs before a model or algorithm is applied.

Real-world datasets frequently contain:

- Missing observations
- Inconsistent values
- Outliers
- Variables with different numerical scales
- Redundant information
- Highly correlated features

The preprocessing workflow explored in the coursework can be summarized as:

```text
Raw Dataset
     |
     v
Data Inspection
     |
     v
Missing Values
     |
     v
Outlier Analysis
     |
     v
Data Transformation
     |
     v
Normalization
     |
     v
Clean Dataset
```

Preparing the data correctly is essential because the quality of the analytical results depends directly on the quality of the input data.

---

# Missing Values

The coursework explores the identification and treatment of **missing data**.

The first step is determining where information is incomplete:

```text
Dataset
   |
   v
Missing-Value Detection
   |
   v
Analyze Missingness
   |
   v
Select Treatment
   |
   v
Processed Dataset
```

Handling missing values is important because incomplete observations can affect:

- Statistical summaries
- Correlations
- Regression models
- Distance calculations
- Clustering algorithms
- Dimensionality-reduction techniques

The appropriate treatment depends on the characteristics of the dataset and analytical objective.

---

# Outlier Analysis

The repository also includes work related to identifying and analyzing **outliers**.

An outlier is an observation that differs substantially from the general behavior of the dataset.

Conceptually:

```text
Typical observations:

      • •
   • • • •
  • • • • •
   • • • •

                         •  <- potential outlier
```

Outlier analysis is important because extreme observations can influence:

- Means and standard deviations
- Correlation coefficients
- Regression models
- Clustering results
- Feature scaling

An important part of the analysis is determining whether an unusual observation represents an error or legitimate information.

---

# Data Normalization

Variables in a dataset may have very different numerical scales.

For example:

```text
Feature A:  0 - 1
Feature B:  0 - 100
Feature C:  0 - 100000
```

Without appropriate scaling, variables with larger numerical magnitudes can dominate algorithms based on distances or numerical optimization.

Normalization transforms variables into more comparable scales.

The general workflow is:

```text
Original Features
       |
       v
Analyze Scale
       |
       v
Normalization / Scaling
       |
       v
Comparable Features
```

This is particularly relevant for methods such as **K-Means clustering and PCA**.

---

# Exploratory Data Analysis

Before applying more advanced techniques, the dataset is explored to understand its structure and behavior.

Exploratory analysis includes concepts such as:

- Variable distributions
- Descriptive statistics
- Relationships between variables
- Data quality
- Potential anomalies
- Feature behavior

Conceptually:

```text
Dataset
   |
   +------> Summary Statistics
   |
   +------> Distributions
   |
   +------> Correlations
   |
   +------> Outliers
   |
   +------> Feature Relationships
   |
   v
Data Understanding
```

Exploratory analysis provides the information necessary to make better preprocessing and modeling decisions.

---

# Correlation Analysis

The repository includes exercises analyzing relationships between numerical variables through **correlation**.

A correlation matrix can conceptually be represented as:

```text
         X1     X2     X3     X4
X1      1.00   0.82  -0.15   0.41
X2      0.82   1.00  -0.10   0.36
X3     -0.15  -0.10   1.00   0.61
X4      0.41   0.36   0.61   1.00
```

Correlation analysis helps identify:

- Strong relationships
- Weak relationships
- Positive relationships
- Negative relationships
- Potentially redundant variables

This information can support feature analysis and dimensionality reduction.

---

# Principal Component Analysis

The coursework includes **Principal Component Analysis (PCA)** as a dimensionality-reduction technique.

PCA transforms a set of potentially correlated variables into a new set of components.

Conceptually:

```text
Original Dataset

X1
X2
X3
X4
X5
X6
 |
 v
Standardization
 |
 v
PCA
 |
 v
Principal Components

PC1
PC2
PC3
```

The first principal components attempt to retain as much of the original variance as possible.

---

## Why PCA?

High-dimensional datasets can contain variables that are correlated or partially redundant.

PCA can be used to:

- Reduce dimensionality
- Identify major directions of variation
- Reduce redundancy
- Simplify visualization
- Create compact representations of data

The transformation can be summarized as:

```text
High-Dimensional Data
          |
          v
        PCA
          |
          v
Lower-Dimensional Representation
          |
          v
Analysis / Visualization
```

PCA also introduces the importance of understanding the relationship between **variance and information preservation**.

---

# Regression

The repository includes practical work with **regression**, representing the supervised-learning component of the Data Mining coursework.

Regression attempts to model the relationship between a set of input variables and a continuous target.

```text
Input Features
      |
      v
Regression Model
      |
      v
Continuous Prediction
```

In general:

```text
y = f(X)
```

where:

- `X` represents the predictor variables.
- `y` represents the continuous target.
- `f` represents the relationship estimated from the data.

Regression provides a bridge between exploratory statistical analysis and predictive modeling.

---

# Unsupervised Learning

Unlike supervised learning, unsupervised methods operate without a predefined target variable.

```text
Dataset
   |
   v
No Target Labels
   |
   v
Unsupervised Algorithm
   |
   v
Discover Structure
```

The Data Mining coursework explores this perspective primarily through **K-Means clustering and PCA**.

---

# K-Means Clustering

The repository includes exercises using **K-Means**, one of the most widely used clustering algorithms.

The objective is to divide observations into `K` groups according to their similarity.

```text
Unlabeled Data
      |
      v
Choose K
      |
      v
Initialize Centroids
      |
      v
Assign Points to Nearest Centroid
      |
      v
Update Centroids
      |
      v
Repeat Until Convergence
      |
      v
Final Clusters
```

A conceptual result might look like:

```text
Cluster A           Cluster B

  • •                  x x
 • • •                x x x
  • •                  x x


             Cluster C

               + +
              + + +
               + +
```

---

## K-Means Workflow

The basic iterative process is:

```text
1. Select K
      |
      v
2. Initialize centroids
      |
      v
3. Calculate distances
      |
      v
4. Assign observations
      |
      v
5. Recalculate centroids
      |
      v
6. Repeat
```

This introduces important concepts including:

- Similarity
- Distance
- Centroids
- Cluster assignment
- Iterative optimization
- Unsupervised pattern discovery

Because K-Means relies on distances, preprocessing and normalization can significantly influence the resulting clusters.

---

# Association Rules

The repository also covers **association-rule mining**, a Data Mining technique used to discover relationships between items or events that frequently occur together.

The general idea can be represented as:

```text
Transactions
     |
     v
Frequent Itemsets
     |
     v
Association Rules
     |
     v
Interesting Relationships
```

A rule can be expressed conceptually as:

```text
A -> B
```

meaning that observations containing `A` frequently exhibit a relationship with `B`.

---

## Association-Rule Concepts

Association-rule analysis introduces concepts related to the frequency and relevance of relationships between items.

A typical rule:

```text
{Item A, Item B} -> {Item C}
```

can be analyzed to determine whether the observed relationship is sufficiently frequent or meaningful to investigate.

This type of analysis is commonly associated with problems involving transactional and co-occurrence data.

---

# Supervised vs. Unsupervised Analysis

The coursework provides exposure to both analytical perspectives:

| Supervised | Unsupervised |
|---|---|
| Target variable available | No predefined target |
| Learns relationship with target | Discovers hidden structure |
| Regression | K-Means |
| Prediction-oriented | Pattern-oriented |

PCA and association-rule mining further extend the unsupervised perspective by exploring dimensional structure and relationships between observations or variables.

---

# Data Mining Workflow

The techniques explored throughout the repository can be integrated into a broader workflow:

```text
                  Raw Dataset
                       |
                       v
                 Data Cleaning
                       |
              +--------+--------+
              |                 |
              v                 v
        Missing Values       Outliers
              |                 |
              +--------+--------+
                       |
                       v
                 Normalization
                       |
                       v
              Exploratory Analysis
                       |
              +--------+--------+
              |                 |
              v                 v
         Correlation           PCA
              |                 |
              +--------+--------+
                       |
              +--------+--------+
              |                 |
              v                 v
          Regression         K-Means
                                |
                                v
                        Association Rules
                                |
                                v
                       Pattern Discovery
                                |
                                v
                          Interpretation
```

This emphasizes that Data Mining is not a single algorithm but a complete analytical process.

---

# Relationship with Machine Learning

Data Mining and Machine Learning overlap but emphasize different parts of the analytical process.

```text
Data Mining
    |
    +------ Data Cleaning
    |
    +------ Exploratory Analysis
    |
    +------ Pattern Discovery
    |
    +------ Dimensionality Reduction
    |
    +------ Clustering
    |
    +------ Association Rules
    |
    +------ Predictive Analysis
```

Machine Learning algorithms can therefore be used as components inside a broader Data Mining workflow.

---

# Relationship with Data Science

The Data Mining coursework forms part of a broader Data Science training path:

```text
                    Data Science
                         |
          +--------------+--------------+
          |              |              |
          v              v              v
     Data Mining   Machine Learning  Deep Learning
          |
    +-----+-----+
    |     |     |
    v     v     v
   PCA K-Means Association Rules
```

The course complements training in:

- Artificial Intelligence
- Machine Learning
- Deep Learning
- Graph Theory
- NoSQL Databases
- Statistical analysis
- Python-based data processing

---

# Skills Developed

Through the exercises in this repository, the course develops practical knowledge in:

- Data preprocessing
- Data cleaning
- Missing-value analysis
- Outlier analysis
- Data normalization
- Exploratory Data Analysis
- Descriptive statistics
- Correlation analysis
- Feature analysis
- Principal Component Analysis
- Dimensionality reduction
- Regression
- Unsupervised learning
- K-Means clustering
- Association-rule mining
- Pattern discovery
- Data visualization
- Interpretation of analytical results
- Python-based data analysis

---

# Academic Context

This repository contains coursework developed as part of my specialized training in:

**Data Science & Artificial Intelligence**  
**Universidad Autónoma de San Luis Potosí (UASLP)**  
San Luis Potosí, Mexico

The complete specialized training comprised **195 hours** and covered:

- Machine Learning
- Artificial Intelligence
- Data Mining
- Deep Learning
- Graph Theory
- Data preprocessing
- Statistical and computational analysis
- Python-based scientific data processing

---

# Repository Purpose

The purpose of this repository is to preserve and document the practical exercises completed during my academic training in Data Mining.

The repository demonstrates the progression from raw information to analytical insight:

```text
Raw Data
   |
   v
Clean Data
   |
   v
Exploratory Analysis
   |
   v
Feature Relationships
   |
   +--------------------+
   |                    |
   v                    v
  PCA                Regression
   |
   v
Reduced Representation
   |
   v
K-Means
   |
   v
Clusters
   |
   v
Pattern Discovery
```

Together, these exercises provide foundations for transforming raw datasets into useful statistical, descriptive, and predictive information.

---

# Author

**José Luis Romero Vázquez**

Electronics Engineer and Data Scientist with international graduate education in Electronic Engineering, Telecommunications, and Computer Networks, with applied experience in Machine Learning, time-series forecasting, IoT analytics, statistical modeling, research, and software development.

**LinkedIn:**  
https://www.linkedin.com/in/jose-luis-romero-vazquez-486569209

**GitHub:**  
https://github.com/0311869uaslp-a11y
