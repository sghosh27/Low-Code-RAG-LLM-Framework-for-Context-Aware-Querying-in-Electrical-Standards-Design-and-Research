# RAG-LLM-Framework-for-Context-Aware-Querying-in-Electrical-Standards-Design-and-Research

Implementation of the paper "RAG-LLM Framework for Context-Aware Querying in Electrical Standards, Design, and Research" by Soham Ghosh and Gaurav Mittal.

N8N workflow files associated with the manuscript and supplementary Jupyter Notebooks being provided are listed below:

N8N templates:
* RAG_Google_Drive_Tool.json - This template retrieves files from Google Drive, parses them, and stores them in a vector database. When a query is made, the workflow searches the vector database for adequate data retrieval. 
* RAG_Google_Drive_Tool_with_Reranker.json - This template is similar to the 'RAG_Google_Drive_Tool.json' workflow, but improves performance through the usage of reranking (Cohere reranking V 3.5 for this case).
* RAG_Google Drive_with_Contextual_Retrival_1.json - This is an advanced template that enhances the chunking strategy by adding context, improving performance. Higher token counts are expected.
* Knowledge_Graph_RAG.json - This N8N RAG knowledge graph workflow connects to knowledge graph(s) residing in the Infranodus platform. The workflow can be used to manage diverse and disconnected data. 

Jupyter Notebook: 
* LLM_Evaluation.ipynb - For LLM evaluation and scoring. The notebook uses the input prompt, a ground truth, and the LLM's actual output for evaluation and scoring. 
* Parsing_Documents.ipynb - Can be used to create Markdown files, which can be uploaded into Anything LLM. This can be used to emulate section 3 of the manuscript to develop a private RAG-LLM workflow. 

Notes: 
1. You have to generate application-specific API keys to use the N8N templates or Jupyter notebook.
2. Please contact the corresponding author at sghosh27@ieee.org for further technical assistance.
