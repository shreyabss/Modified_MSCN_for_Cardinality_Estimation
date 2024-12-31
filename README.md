# Modified_MSCN_for_Cardinality_Estimation
Introduction
Cardinality estimation plays a crucial role in query optimization within database management systems (DBMS). This project explores how machine learning (ML) can address challenges in cardinality estimation and improve query efficiency. Our focus was to evaluate ML techniques applied to database cardinality and selectivity estimation problems, specifically implementing a modified Multi-Set Convolutional Network (MSCN) model.

Dataset
We used the IMDB dataset containing various features such as production year, movie companies, and cast information. The dataset was split into 90% training and 10% testing, with a training generator employed to produce query representations for ML models. Key statistics and binary representations for feature encoding were included to prepare the data.

Models
We studied and implemented several models, including:
Neural Networks: For both range and string predicate selectivity.
Multi-Set Convolutional Network (MSCN): A baseline for handling correlated joins and relational query plans.
Modified MSCN: Integrated 1D convolutional layers, residual connections, and improved normalization for enhanced learning capacity.
Hyperparameter tuning optimized the models, with 150 epochs, a batch size of 400, and an Adam optimizer with a 0.001 learning rate.

Results
The modified MSCN model demonstrated the best performance, achieving:
Improved generalization and reduced outliers, indicating robust performance.
The modified model excelled in accurately predicting correlated joins and complex queries.
