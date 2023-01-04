HIMdata
=========
The HIMdata dataset consists of two parts:
* same_city folder represents the Same_City Relationship dataset;
* advisor_advisee folder represents the Advisor_Advisee Relstionship dataset.

-------------------------------------

The Same_City Relationship dataset:
----------------
### refined_data/data.txt 

all the connection pairs in the Same_City Relationship network. The first and second columns of data represent the two nodes that form a link (mutual following relationship) in the network. The third column represents the same-city relationship, where 1 represents the two users in the same city, and 0 represents the two users in different cities.

### refined_data/node_features.mat 
the attributes information of all nodes in the network.

### refined_data/node_ind.txt 
the index information of all nodes in the network, represented by the users' id information in the Weibo social network.

### refined_data/node_node.mat 
the adjacency matrix of graph.

### refined_data/one_hot_vector.mat 
the one-hot encoding of node attributes, which is generated according to the attributes dimension of the nodes.

### data/relation_false.txt 
a decomposed version of refined_data/data.txt, which represents mutual following relationship pairs without same-city relationship.

### data/relation_true.txt 
a decomposed version of refined_data/data.txt, which represents mutual following relationship pairs with same-city relationship.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

The Advisor_Advisee Relationship dataset:
-------------------------

### refined_data/data.txt 
all the connection pairs in the Advisor_Advisee Relationship network. The first and second columns of data represent the two nodes that form a link (co-author relationship) in the network. The third column represents the advisor-advisee relationship, where 1 represents that there is an advisor-advisee relationship between the two scholars, and 0 represents that there is no advisor-advisee relationship between the two scholars.

### refined_data/aut_institution.mat 
the part of the attributes of the scholars, representing the information between scholars and their institutions.

### refined_data/author_paper.mat 
the part of the attributes of scholars, representing the information between scholars and their papers.

### refined_data/paper_attribute.mat 
the attributes information of all papers. The paper nodes and scholar nodes in the network are related to each other, which means that the scholar has published the paper.

### refined_data/author_index.txt 
the index information of all scholars in the network, represented by the scholars' name information in the academic network.

### refined_data/author_author.mat 
the adjacency matrix of graph.

### refined_data/node_ind.txt 
the index information of all nodes in the network, represented by the nodes' number information in the network.

### refined_data/one_hot_vector.mat 
the one-hot encoding of node attributes. refined_data/one_hot_vector.mat contains two one-hot vector matrices, one is according to the attributes dimension of authors, and the other is generated according to the attributes dimension of institutions.

### data/relation_false.txt 
a decomposed version of refined_data/data.txt, which represents co-author relationship pairs without advisor-advisee relationship.

### data/relation_true.txt 
a decomposed version of refined_data/data.txt, which represents co-author relationship pairs with advisor-advisee relationship.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

The above is the introduction of these two datasets, where refined_data/data.txt and attributes data are the metadata. If the required data file does not exist, the required data can be generated from the metadata.
