---
layout: page
title: Dissertation
permalink: /thesis
---

# Energy Efficiency in Machine Learning
## Approaches to Sustainable Data Stream Mining

---
### Abstract

Energy efficiency in machine learning explores how to build machine learning algorithms and models with low computational and power requirements.
Although energy consumption is starting to gain interest in the field of machine learning, still the majority of solutions focus on obtaining the highest predictive accuracy, without a clear focus on sustainability.

This thesis explores green machine learning, which builds on green computing and computer architecture to design sustainable and energy efficient machine learning algorithms.
In particular, we investigate *how to design machine learning algorithms that automatically learn from streaming data in an energy efficient manner*.

We first illustrate how energy can be measured in the context of machine learning, in the form of a literature review and a procedure to create theoretical energy models.
We use this knowledge to analyze the energy footprint of Hoeffding trees, presenting an energy model that maps the number of computations and memory accesses to the main functionalities of the algorithm. We also analyze the hardware events correlated to the execution of the algorithm, their functions and their hyper parameters.

The final contribution of the thesis is showcased by two novel extensions of Hoeffding tree algorithms, the Hoeffding tree with *nmin adaptation* and the Green Accelerated Hoeffding Tree. These solutions are able to reduce their energy consumption by twenty and thirty percent, with minimal effect on accuracy. This is achieved by setting an individual splitting criteria for each branch of the decision tree, spending more energy on the fast growing branches and saving energy on the rest.

This thesis shows the importance of evaluating energy consumption when designing machine learning algorithms, proving that we can design more energy efficient algorithms and still achieve competitive accuracy results.

---
### Thesis description and author contribution
This dissertation is a compilation thesis that consists of a number of published or publishable papers, synthesized into a thesis introduction.
The thesis author has been the main driver of all the publications. The author has planned the studies, designed the experiments, conducted the experiments, conducted the analysis and written the manuscripts.

---
### PDF
A PDF of the complete thesis can be found in the following link: [PDF](http://bth.diva-portal.org/smash/get/diva2:1374831/FULLTEXT03.pdf)

---


### Included papers
<br/>
* **García-Martín E.**, Rodrigues C., Riley G., & Grahn H.  (2019)  *Estimation of Energy Consumption in Machine Learning*. Journal of Parallel and Distributed Computing, 2019, Elsevier. DOI: <https://doi.org/10.1016/j.jpdc.2019.07.007> - **[[ScienceDirect]](https://www.sciencedirect.com/science/article/pii/S0743731518308773)**

  <details>
  <summary>Abstract</summary>

  Energy consumption has been widely studied in the computer architecture field for decades. While the adoption of energy as a metric in machine learning is emerging, the majority of research is still primarily focused on obtaining high levels of accuracy without any computational constraint. We believe that one of the reasons for this lack of interest is due to their lack of familiarity with approaches to evaluate energy consumption. To address this challenge, we present a review of the different approaches to estimate energy consumption in general and machine learning applications in particular. Our goal is to provide useful guidelines to the machine learning community giving them the fundamental knowledge to use and build specific energy estimation methods for machine learning algorithms. We also present the latest software tools that gives energy estimation values, together with two use cases that enhance the study of energy consumption in machine learning.
  </details><br/>
* **García-Martín E.**, Lavesson N., & Grahn H. (2017).  *Energy Efficiency Analysis of the Very Fast Decision Tree algorithm*. In: Missaoui R., Abdessalem T., Latapy M. (eds) Trends in Social Network Analysis. Lecture Notes in Social Networks, (pp. 229-252), Springer. DOI: <https://doi.org/10.1007/978-3-319-53420-6_10>   **[[PDF]](http://bth.diva-portal.org/smash/get/diva2:1156925/FULLTEXT01.pdf)**
  <details>
  <summary>Abstract</summary>
  Data mining algorithms are usually designed to optimize a trade-off between predictive accuracy and computational efficiency. This paper introduces energy consumption and energy efficiency as important factors to consider during data
  mining algorithm analysis and evaluation. We conducted an experiment to illustrate how energy consumption and accuracy are affected when varying the parameters of the Very Fast Decision Tree (VFDT) algorithm. These results are compared with a theoretical analysis on the algorithm, indicating that energy consumption is affected by the parameters design and that it can be reduced significantly while maintaining accuracy.
  </details><br/>

* **García-Martín E.**, Lavesson N., & Grahn H. (2017). *Identification of Energy Hotspots: A Case Study of the Very Fast Decision Tree*.  In: Au M., Castiglione A., Choo KK., Palmieri F., Li KC. (eds) Green, Pervasive, and Cloud Computing. GPC 2017. Lecture Notes in Computer Science, 10232, (pp. 267-281), Springer. DOI: <https://doi.org/10.1007/978-3-319-57186-7_21> **[[PDF]](http://bth.diva-portal.org/smash/get/diva2:1156958/FULLTEXT01.pdf)**
  <details>
  <summary>Abstract</summary>
  Large-scale data centers account for a significant share of
  the energy consumption in many countries. Machine learning technology requires intensive workloads and thus drives requirements for lots of
  power and cooling capacity in data centers. It is time to explore green
  machine learning. The aim of this paper is to profile a machine learning
  algorithm with respect to its energy consumption and to determine the
  causes behind this consumption. The first scalable machine learning algorithm able to handle large volumes of streaming data is the Very Fast
  Decision Tree (VFDT), which outputs competitive results in comparison
  to algorithms that analyze data from static datasets. Our objectives are
  to: (i) establish a methodology that profiles the energy consumption of
  decision trees at the function level, (ii) apply this methodology in an experiment to obtain the energy consumption of the VFDT, (iii) conduct
  a fine-grained analysis of the functions that consume most of the energy,
  providing an understanding of that consumption, (iv) analyze how different parameter settings can significantly reduce the energy consumption.
  The results show that by addressing the most energy intensive part of
  the VFDT, the energy consumption can be reduced up to a 74.3%
  </details><br/>


* **García-Martín E.**, Lavesson N., Grahn H., Casalicchio E., & Boeva V. (2018)  *Energy-Aware Very Fast Decision Tree*. Journal of Data Science and Analytics, Springer.*(Accepted)*
  <details>
  <summary>Abstract</summary>
  Recently machine learning researchers are designing algorithms that can run in embedded and mobile devices, which introduces additional constraints compared to traditional algorithm design approaches.
  One of these constraints is energy consumption, which directly translates to battery capacity for these devices.
  Streaming algorithms, such as the Very Fast Decision Tree (VFDT), are designed to run in such devices due to their high velocity and low memory requirements. However, they have not been designed with an energy efficiency focus.
  This paper addresses this challenge by presenting the nmin adaptation method, which reduces the energy consumption of the VFDT algorithm with only minor effects on accuracy.
  nmin adaptation allows the algorithm to grow faster in those branches where there is more confidence to create a split, and delays the split on the less confident branches. This removes unnecessary computations related to checking for splits but maintains similar levels of accuracy.
  We have conducted extensive experiments on 29 public datasets, showing that the VFDT with nmin adaptation consumes up to 31% less energy than the original VFDT, and up to 96% less energy than the CVFDT (VFDT adapted for concept drift scenarios), trading off up to 1.7 percent of accuracy.
  </details><br/>


* **García-Martín E.**, Bifet A., Lavesson N., (2019) *Energy Efficient Ensembles of Hoeffding Trees*. Intelligent Data Analysis *(Accepted)*.
  <details>
  <summary>Abstract</summary>

  Energy consumption reduction has been an increasing trend in machine
  learning over the past few years due to its socio-ecological importance. In new challenging areas such as edge computing, energy consumption and predictive accuracy are key variables during algorithm design and implementation. State-of- the-art stream mining algorithms are able to create highly accurate predictions in real-time while adhering to low computational requirements to run in edge devices. This is the case of ensembles of Hoeffding trees. While these algorithms obtain high levels of accuracy, that is done at a substantial energy cost. This paper introduces the nmin adaptation method to ensembles of Hoeffding tree algorithms,
  to further reduce their energy consumption without sacrificing accuracy. We have evaluated the energy efficiency and accuracy of the nmin adaptation
  method on five different ensembles of Hoeffding trees under 11 publicly available datasets.
  The results show that we are able to reduce the energy consumption significantly,
  by 21 % on average, affecting accuracy by less than one percent on average.

  </details><br/>

* **García-Martín E.**, Bifet A., Lavesson N., (2019) *Green Accelerated Hoeffding Tree*. The 24th Pacific-Asia Conference on Knowledge Discovery and Data Mining *(Under review)*
  <details>
  <summary>Abstract</summary>
  Stream mining algorithms are able to produce highly accurate models in real time, without strong computational demands. This is the case of the Hoeffding tree algorithm. Recent extensions to this algorithm focus on increasing predictive accuracy, but at the cost of a higher energy consumption. This paper presents the Green Accelerated Hoeffding Tree (GAHT) algorithm, which is able to achieve same levels of accuracy as the latest Hoeffding tree extension, i.e. Extremely Very Fast Decision Tree (EFDT), while reducing its energy consumption. In particular, the GAHT algorithm is able to reduce the energy consumption of the EFDT by 26 percent, averaged on 11 publicly available datasets, with minimal effect on accuracy.
  </details>
