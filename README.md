# Langchain-Instructor-QA

This repository contains two Python scripts that demonstrate how to use Instructor Embeddings and Langchain to create a retrieval-based question answering (QA) system for an educational context.

#Scripts

###langchain_helper.py: This script contains two functions:

create_vector_db(): This function creates a vector database from a CSV file containing question-answer pairs. The vector database stores the documents using Instructor Embeddings, which            are a type of text embedding that is specifically designed for question answering tasks.
        
get_qa_chain(): This function creates a retrieval-QA chain that can be used to answer questions based on the vector database. The chain uses a retriever to find documents that are                  relevant  to the question, and then uses a prompt template to guide the language model in generating an answer.

###main.py: 

This script creates a Streamlit app that allows users to ask questions about the educational content. The app first creates a vector database and retrieval-QA chain using the functions from the langchain_helper module. Then, it creates a user interface with a button to create the knowledge base and a text input field for users to enter questions. When a user enters a question, the app retrieves the retrieval-QA chain, passes the question to the chain, and displays the answer to the user.

##Installation

To run this project, you will need to install the dependencies in the requirements.txt

You can install the dependencies using the following command: pip install -r requirements.txt

##Usage

To run the Streamlit app, run the following command from the project directory:

streamlit run main.py

This will open a web browser window with the Streamlit app. You can then ask questions by typing them into the text input field and clicking the "Submit" button.

##License

This project is licensed under the MIT License.
