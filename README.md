# Text-classification-using-deep-neural-networks
In this project, I have used some text files to classify them according to their labels. The Reuters corpus is one of the most famous datasets for text categorization tasks. A subset of this dataset is used to build a classifier. There is more information about this dataset available on http://disi.unitn.it/moschitti/corpora.htm.

1. Downloaded zip files and extracted it.
2. Each folder contains some XML files. Explored XML files to find a list of all fields available there.
3. created a function to extract a Pandas's Dataframe containing: (1) headline, (2) text, (3) bip:topics,(4) dc.date.published, (5) itemid, (6) XMLfilename
4. A python function is created to find all the possible values for bip:topics. Considering that each news can belong to more than one topic.
5. created a function to prepare text data by methods such as removing stop word and to cluster all the documents as a preprocessing step. This function assigns a cluster-id to each document. After clustering documents, we generate a different classifier for each identified cluster.
6. A function is created to evaluate the quality of clusters. 
7. Applied the following paper to enhance feature selection method. Generated a set of features for each extracted cluster separately. 
• [Paper 1] Liang, Hong et al. “Text feature extraction based on deep learning: a review.” EURASIP journal on wireless communications and networking vol. 2017,1 (2017): 211. doi:10.1186/s13638-017-0993-1
8. Improved classification approach by using new features and taking advantage of deep neural networks. 
