# EmbraceLimitedImperfectData

Embrace limited and imperfect data in plant disease recognition using deep learning.

Currently maintained by [Mingle Xu](https://xml94.github.io/ "Personal website").

# Motivation
>Recent advancements in deep learning have brought significant improvements to plant disease recognition.
However, achieving satisfactory performance often requires high-quality training datasets, 
which are challenging and expensive to collect. 
Consequently, the practical application of current deep learning-based methods in real-world scenarios 
is hindered by the scarcity of high-quality datasets.
Consequently, we argue that embracing non-high-quality datasets is more convincing and practical.
Although this embrace brings opportunities, new challenges exist.
A taxonomy of related challenges is, therefore, proposed to enrich our understandings.
With this perspective, we do hope that deep learning can be implemented 
in real-world applications with satisfactory performance.


# Taxonomy of the challenges

* Limited data: the training dataset is not in large-scale.
* * Class-level: consider the variation of different classes within the training dataset.
* * * ![](https://img.shields.io/badge/-Few--shot-ffe8d1): All classes have similar few annotated images, where trained models may get low performance for all classes.
* * * ![](https://img.shields.io/badge/-Class%20imbalance-ffd7e1): One class has many more annotated images than another class, where trained models may get high performance in the former class but suffer in the latter class.
* * Dataset-level: consider the diversity between the training and test datasets.
* * * ![](https://img.shields.io/badge/-Domain%20shift-red): The training and test datasets share the same label spaces but are in different distribution spaces, where trained models may get low test performance.
* * * ![](https://img.shields.io/badge/-Unknown%20class-purple): Unknown (new) classes exist in the test dataset, where trained models will consider the corresponding image into a known class and not distinguish the unknown from known classes.
* Imperfect data: the training dataset is annotated in an undesired way.
* * ![](https://img.shields.io/badge/-Incomplete%20annotation-green): Training datasets have labeled and unlabeled images simultaneously, where utilizing the unlabeled images may contribute to the test performance.
* * ![](https://img.shields.io/badge/-Inexact%20annotation-yellow): Training datasets are given with only coarse-grained annotations, where utilizing these annotations is challenging to train models.
* * ![](https://img.shields.io/badge/-Inaccurate%20annotation-blue): Some annotations may be inaccurate, where it is challenging to get decent test performance by utilizing these annotations to train models.




# Related research
