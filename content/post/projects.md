---
title: "Projects"
date: 2019-08-26T16:57:17+05:30
draft: false
type: "page"
---


These are some of projects I have worked on:

### 1. Classifying a dermoscopic image using deep Learning (multi-class classification problem)(Work in Progress)

Currently working on this project [here](https://colab.research.google.com/drive/1GrqpJwToJN9T2xz6pmUiJV-YrazMiPeR). Visit soon for an update!

<!-- <details><summary> Currently working on this project</summary>
<p>
<p align="center"> -->

### 2. Feature Optimization of contact map predictions based on inter-residue distances and U-Net++ architecture

<details><summary> Master Thesis Project (Jan 2019 - Jun 2019) conducted at Science for Life Laboratory under the supervision of Dr. Arne Elofsson (Click for details) </summary>
<p>
<p align="center">

#### Abstract:

</p>

**Background**: Determination of the three-dimensional structure of proteins has been a scientific challenge for decades. Since there are many hurdles associated with experimental determination of protein structures, there are attempts for making in-silico predictions of protein structures more accurate. Recent advances include prediction of contacts between residues in a protein using convolutional neural net- works. Based on the results of the latest global competition for protein structure prediction (called CASP13), inter-residue distances are found to contain key infor- mation required for structure prediction.

**Aim**: The primary objective of this study was to determine if inter-residue distance- based classification could improve predictions of contacts between residues in a pro- tein. The secondary objective was to determine whether contact predictions based on U-Net, a popular architecture for biomedical image segmentation could be im- proved by using an alternate nested architecture called U-Net++.

**Methods**: Using the inputs from state-of-the-art contact prediction model PconsC4, the distance between residue pairs in proteins were used to predict contacts as a clas- sification problem as compared to the regression approach used in PconsC4. The output of this study was a distance-based probability distribution as compared to S-score (a single quantity of distance measure). Additionally, the U-Net architec- ture was replaced and tested with U-Net++ architecture. The results from all the models deployed during this study were evaluated using performance metrics.

**Results**: Inter-residue contact distance predictions were calculated for three bin ranges - 7, 12 and 26. These showed low precision values between 0.07 and 0.3 while the absolute and relative error did not shown much variation among the models. The U-Net++ implementation showed improved precision from 0.59 to 0.67 for all residues for top L contacts. Despite recall slightly falling from 0.35 to 0.30 and no visual difference between the contact maps, there is more accurate determination of correctly predicted distances against the actual distances while testing 210 proteins.

**Conclusions**: Contrary to CASP13 results which showed improved contact predic- tions by using inter-distance, implementing distance-based classification on PconsC4 did not improve the predictions of contacts. However, U-Net++ architecture showed improved precision values than U-Net architecture for PconsC4 model of contact pre- dictions.

**Key Words**: Protein Folding; Convolutional Neural Networks; Contact Map; Pro- tein Structure Prediction; Ab-initio protein folding

</p>
</details>

### 3. Heart Disease Prediction System

<details><summary> During this project, I worked in an multi-disciplinary group consisting of physicians, nurses, physiotherapists, biomedical scientists and software engineers to develop a heart prediction system (October 2018) (Click for details) 
</summary>
<p>
<p align="center">

#### Abstract:

</p>

I spearheaded the development of a heart prediction system in multi-disciplinary group consisting of physicians, nurses, physiotherapists, biomedical scientists and software engineers using data from [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/heart+disease). 

This project was developed as a part of the course 'Project management and tools for health informatics' at Stockholm University under the Global Master's in Health Informatics Programme. This programme was a joint collaboration between Karolinska Institutet and Stockholm University in Sweden.

This team-based project consisted of the following steps:

* Description of the data and understanding the features in the dataset
* Data pre-processing (dealing with missing values, continuous to discrete values, dichotomize target variable, convert variables to factors and remove insignificant attributes)
* Tested classifiers - (Gradient Boosting, Random Forest, Logistic Regression, Support Vector Machine and Naive Bayesian)
* Selected optimal combination of datasets and trained using splitting criteria
* Evaluated using the metrics: Accuracy, Precision, Recall, F-Measure, AUC

The outcome of this project was a fully functional heart disease prediction system which was developed in R. The user interface to input the values for testing was developed using R Shiny. We were awarded a perfect A grade for this project with the feedback that the system we presented was one of the best in our class. The report on this project can be found [here](https://docs.google.com/document/d/1csdFuhRH-GVwEQIWAKGUyo7mMooAdiH9YdD-F4SkQa4/edit#) and the code can be found [here](https://github.com/aditishenoy/Heart-Disease-Prediction/blob/master/README.md).

</p>
</details>

### 4. H-Links: Supporting Physicians with Objective Pain Monitoring for the Comfort of Patients at Homes

<details><summary> Designed and prototyped an objective pain monitoring mobile health solution based on requirements of the physicians at Lille University Hospital (August 2018). (Click for details) 
</summary>
<p>

By working together with a multidisciplinary group of students having various backgrounds, we developed an objective pain monitoring mobile health solution based on requirements of the physicians at Lille University Hospital. We passed with great distinction. During this summer school, I developed skills for medical device development - CE Marking, Usability Analysis, Risk Analysis, Pre-Clinical Testing, Clinical Investigation, Post-Market Monitoring. 

> [Publication:](http://www.scitepress.org/DigitalLibrary/Link.aspx?doi=10.5220/0007696106370644)
Moustakim, S.; Julien, D.; Holubov, **A.; Shenoy**, A.; Carsch, D. and Battaglia, J. (2019). H-Links: Supporting Physicians with Objective Pain Monitoring for the Comfort of Patients at Homes. In Proceedings of the 12th International Joint Conference on Biomedical Engineering Systems and Technologies - Volume 5: ClinMed, ISBN 978-989-758-353-7, pages 637-644.
DOI: 10.5220/0007696106370644 
</p>
</details>

### 5. Evaluation of Co-morbidities of Melanoma using Real World Evidence (RWE)

<details><summary> Bachelor Thesis Project (Jan 2017 - Jul 2017) conducted at Novartis under the supervision of Dr. Reena Gollapudy, Srinivasa Rao Pelluri and Dr. Fayaz S M (Click for details) </summary>
<p>
<p align="center">

#### Abstract:

</p>

Real-world evidence (RWE) investigations are increasingly important contributors to biopharmaceutical R&D. Evidence from “real world” practice and utilization has the potential to tailor healthcare decision making more closely to the characteristics of individual patients, and thereby help in making health care more personalized and effective. RWE challenges the traditional paradigm in which the only authoritative medical evidence is generated through prospective randomized clinical trials (RCTs), validated through peer reviewed publication in reputable journals and incorporated into broadly applied clinical practice guidelines. Data from the real-world (RWE, Registry data, Electronic Medical Records (EMR) and Electronic Health Records (EHR)) can enhance our understanding of the disease (e.g. chronic cases of melanoma), and thereby support the development of new therapies and technologies to be incorporated into routine clinical practice.

In the present study, novel comorbidity patterns in a real world population of melanoma patients were identified and analyzed. Patient associated medical records were used to categorize chronic cases of melanoma into distinct comorbidity clusters, using probabilistic hierarchical clustering methods. These comorbidities were represented based on their association to each other and based on these patterns, phenotypic disease networks were created.

From these phenotypic disease networks, we were able to identify comorbidity patterns in a select group of melanoma patients. Understanding such patterns can give an insight into the progression of a particular disease and its manifestation in the ‘real world’ population.

The ongoing research at the organization aims to understand the similarities and differences in response to standard of care among the distinct categories of melanoma patients. The novel spatiotemporal, sequential diagnosis patterns that can be obtained, may help the clinician to diagnose and predict the course of the disease and treatment options along with cancer-specific therapeutic approaches to halt unusual moles, sores, lumps, blemishes and markings.


</p>
</details>







<!-- TEMPLATE
### 2. Evaluation of Co-morbidities of Melanoma using Real World Evidence (RWE)

<details><summary> Bachelor Thesis Project (Jan 2017 - Jul 2017) conducted at Novartis under the supervision of Dr. Reena Gollapudy, Srinivasa Rao Pelluri and Dr. Fayaz S M (Click for details) </summary>
<p>
<p align="center">

#### Abstract:

</p>



</p>
</details> -->