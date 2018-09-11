# Amazon Redshift Parallel Ingestion

_Abstract_—Amazon Redshift supports parallel data ingestion. When data is ingested from a single file, Amazon Redshift performs a serialized load, which takes longer than a parallel load. To perform parallel ingestion, the data must be split into multiple files.

In this paper, we test and analyze parallel ingestion on Amazon Redshift looking specifically how ingestion times change based on the number of nodes on a cluster and the number of files the data has been parsed into. For the purposes of this study the “Node type” being used is dc2.large as using this node type reduces the costs of the analysis.

# GMM Training Times Using Spark

_Abstract_—Apache Spark is a cluster framework designed to handle big data. It provides high-level machine learning tools via its Machine Learning Library (MLlib). When data is used to train a machine learning model, the process can be optimized in different ways to reduce cost and/or decrease the time required to train the model.

In this paper, we test and analyze different hypotheses regarding the time to train a Gaussian Mixture Model (GMM) using Apache Spark. Parameters that we experiment with include: the number of partitions a file is split into, the size of the data, the number of instances and instance types, and the number of components used to construct the GMM.
