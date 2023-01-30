# 3-Level-Classification-Approach

#### When performing classification on imbalanced data, we usually either perform undersampling or oversampling.

#### In this project, a multi level approach has been presented to classify imbalanced data.

<img align="centre" alt="model" src="3-level-classification-diagram.png">

#### The above diagram shows the 3 level classification approach.

#### The first level is trained as a binary classifier, where the data can either have a label, 3 or 1. Label 1 is the assigned to all the data points that have a target value 0, 1 2 or 4. Label 3 is assigned to all the data points that have a target value of 3. By using this labelling technique, we can reduce the imbalance in the data.

#### The second level model has 3 possible classes. Label 2 is assigned to all the data points that have a target value of 2. Label 4 is assigned to all the data points that have a target value of 4. Label 0 is assigned to all the data points that have a target value of 0 or 1. The remaining data points are assigned a label of -1 and are not included while trainging the level 2 model.

#### The third level is trained as a binary classifier, where the data can either have a label, 1 or 0. Label 1 is the assigned to all the data points that have a target value 1. Label 0 is assigned to all the data points that have a target value of 1. The remaining data points are assigned a label of -1 and are not included while trainging the level 3 model.
