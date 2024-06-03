#Creating AI assitant For guilding aircraft

In this project, step through the process of using information from multiple documents (in this case, PDF files) to create a vector database. A vector database is specially designed to manage data as vectors, which in the area of machine learning and natural language processing, can represent everything from words and sentences to entire documents. With this knowledge and large language models (LLM), you are able to retrieve information in the context of AI-assisted conversations. Essentially, you have an AI assistant that is tailored to the knowledge that you have. This approach is beneficial for companies with vast repositories of information. By integrating AI, they can efficiently and quickly access and communicate with their knowledge databases. This information could range from text-based customer conversations to sales data described in CSV formats.

IBM Watson
This project aims to build a system that can provide answers to specific questions based on the content from multiple PDF files that are related to aircraft and mechanics. The following steps provide a high-level overview.

Environment setup: Setting up the necessary libraries and determining if the computations can be run on a GPU, which would provide faster performance than a CPU.
Data acquisition: Fetching content from PDF files that are in a directory. These PDFs contain data that is related to aircraft.
Embeddings setup: Representing the text data from these PDFs in a format that can be understood and processed by machine learning models. The code establishes embeddings using a pretrained model.
Text processing: Acquiring data, then breaking down into smaller text chunks that are suitable for further analysis.
Embeddings database creation: Creating a database to store the embeddings of these chunks, facilitating faster retrieval during the question-answering process.
Language learning model setup: A pretrained language learning model is set up to process questions and, combined with the embeddings, provide answers.
Prompt definition: A template is defined that sets the tone and format for asking questions.
Q/A system creation: Combining the previous elements, a question-answering chain is constructed.
Query and output: A question is posed to the system, and the result, along with the source documents containing relevant information, is displayed.
Gradio interface for Ccatbot: A chatbot interface for further Q/A with the source documents.