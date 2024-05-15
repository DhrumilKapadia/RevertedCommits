# RevertedCommits
A project to analyze and predict about reverted commits on GIT using pandas, sklearn and pydriller.

**Why Focus on Reverted Commits?**
A reverted commit is a code change that is undone or rolled back after being part of a software project.
The primary motivation for focusing on reverted commits is to enhance software development efficiency and quality. Reverted commits often disrupt the development process and increase maintenance efforts. By identifying and addressing these commits early, it's possible to prevent integration of problematic code, reduce time spent on fixing issues, and improve the overall health and progress of the software project.

**The Flowchart of a commit:**
![image](https://github.com/DhrumilKapadia/RevertedCommits/assets/51952678/ea37b30c-8357-468f-abb0-944b966f5d60)

**Our Research Questions**
![image](https://github.com/DhrumilKapadia/RevertedCommits/assets/51952678/1081fd70-13b7-46f1-86c7-dfbdb07e843c)

**Dataset Overview**

**Scope of the Dataset:** The dataset encompasses a total of 10 different open-source projects, covering a diverse range of application domains.
**Volume of Data:** It includes an extensive collection of 9000+ commits, offering a rich source of information for analysis.
**Identification of Reverted Commits:** A meticulous process was employed to identify reverted commits. This process involved analyzing commit messages and comparing changed content across commits to accurately determine reversions.
**Significance:** The dataset provides a broad and realistic perspective on commit practices and reversion trends, making it highly relevant for studying the dynamics of software development.

**Study Methodology**
We meticulously extracted a total of XX distinct commit features. These features provide comprehensive insights into the nature and context of each commit.
Feature Dimensions:
Change Dimension: Features related to the code changes made in the commit, such as the number of lines added or removed, files modified, and subsystems affected.
Developer Dimension: Attributes capturing the developer's historical activities and experience, like the number of previous commits and experience with the codebase.
Message Dimension: Analyzing the textual content of commit messages for indicators of potential reversion, including keywords and the nature of the change (e.g., bug fix, feature addition).
Classification Model: Utilizing these features, we built a predictive model using Random Forest classifier to identify commits likely to be reverted. The model was rigorously evaluated for accuracy and effectiveness

**Identification Model**
To accurately identify commits prone to reversion, we developed a sophisticated identification model based on machine learning techniques. Key components of our model include:
Random Forest Classifier: We employed a Random Forest classifier, a powerful ensemble learning method known for its high accuracy and robustness. This classifier works by building multiple decision trees and merging their predictions to improve overall accuracy and control overfitting.
Feature Utilization: The classifier utilizes the XX commit features extracted from the three dimensions—change, developer, and message—effectively combining these diverse data points to predict commit reversion.
Validation Settings:
Cross-Validation: To ensure the reliability of our model, we applied a 10-fold cross-validation method. This technique involves dividing the dataset into ten subsets, using nine for training and one for testing, iteratively across all subsets.
Performance Metrics: The model’s effectiveness was measured using standard performance metrics such as accuracy, precision, recall, and the Area Under the Curve (AUC) for the Receiver Operating Characteristic (ROC) curve.

**Results**
![image](https://github.com/DhrumilKapadia/RevertedCommits/assets/51952678/937f5341-7f74-4b11-8d66-b72e46ae9f6c)

![image](https://github.com/DhrumilKapadia/RevertedCommits/assets/51952678/b7cd160a-6b63-49d3-a973-4d9c454a565c)

![image](https://github.com/DhrumilKapadia/RevertedCommits/assets/51952678/084304bc-8170-4e44-8c7d-f44a92e1dfa1)







