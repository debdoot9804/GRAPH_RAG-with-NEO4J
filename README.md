## Knowledge Graph QnA + RAG using NEO4j on Tabular Dataset
--------------------------------------------------------------------------------------------------------------------------
This is an imeplementation of RAG architecture using GraphDB (Neo4j) in this case.
The dataset used was a movies dataset generated through ChatGpt for Indian movies, the number of rows in the dataset were 40 and had 10 columns.

### Speciality of GraphDB like Neo4j
--------------------------------------------------------------------------------------------------------------------------
Neo4j boasts a powerful and elegant architecture designed specifically for handling complex, highly connected data. At its core lies the native graph storage and processing engine, purpose-built to store and traverse data as nodes, relationships, and properties—the foundational elements of the property graph model. Unlike traditional databases, Neo4j excels at uncovering patterns and connections through lightning-fast graph traversals powered by its intuitive Cypher query language. Its architecture ensures ACID compliance for reliable transactions, while offering horizontal scalability and fault tolerance through a robust leader-follower cluster setup. With Neo4j, data isn’t just stored—it’s meaningfully connected and effortlessly explored.

### Folders and Files
---------------------------------------------------------------------------------------------------------------------------
Under notebooks folder, the following files are present:

1)GraphDB_data_preparation.ipynb:  

Creates a connection with Neo4j Client.

Ingests the CSV tabular dataset using Cyoher Query to create Knowledge graph
                                  
Creates Vector Index for the Neo4j


2)RAG_Retrieval.ipynb:    
Creates a connection with Neo4j Client
  
Embeds user's query
                         
Performs Similarity Search on the GraphDB Neo4j
                         
Uses LLM to produce final result to user.
                          

### Movie Knowledge Graph

![image](https://github.com/user-attachments/assets/b26334f8-78b9-4891-8951-e2d5078c0086)

### Project Schema 

![image](https://github.com/user-attachments/assets/71184a8e-4e4c-445e-8273-0228094e34fc)



