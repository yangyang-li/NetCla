# [Automatic Analysis of Network Traffic](http://www.neteye-blog.com/netcla-the-ecml-pkdd-network-classification-challenge/)


## Challenge


**NetCla: The ECML-PKDD Network Classification Challenge**

In recent years, there have been many proposals pushing for the use of Machine Learning (ML) in automatic network management. This challenge is one of the first explorations of ML for automatic network analysis. Our goal is to promote the use of ML for network-related tasks in general and, at the same time, to assess the participants’ ability to quickly build a learning-based system showing a reliable performance.  Additionally, one difficulty of using ML for network-related applications is the lack of datasets for training and evaluating different algorithms. The challenge provides one of the few datasets for this field, which may become a reference point for future and more advanced research.
As this is one of the first initiative in network classification, we started with a relatively simple multi-class single label classification task, where the labels are standard applications and signals are static network parameters. A more detailed description follows.


## Dataset


The probe measures various Key Performance Indicators (KPIs) and parameters of transmissions generated by many Web Applications of different types. The objective of the challenge is, given a transmission in the network, to predict the type of the application that is transmitting the data. This is clearly a multi-classification task, single label.
More in detail, each data point corresponds to one http transmission. The data points were collected for an entire day and then split into train (20%), validation (20%) and test (20%) chronologically: morning hours correspond to the training set whereas evening hours constitute the test set.
To eliminate possible dependencies between data points, we left a gap of 20% of data between training, development and test sets. This way, training, validation and test time slots are not adjacent. 
