# Chat with documents using RAG

## Introduction
Retrieval Augmented Generation using Gemini LLM
In the evolving landscape of artificial intelligence and natural language processing, the implementation of Retrieval-Augmented Generation (RAG) models has gained significant traction. This project combine the strengths of retrieval-based methods with the generative capabilities of advanced language models to provide more accurate and contextually relevant responses.

This introduction explores the integration of RAG using the Gemini Language Model (LLM), FAISS (Facebook AI Similarity Search), LangChain, and Streamlit, highlighting how these technologies collectively enhance the capabilities of modern AI applications.

### Gemini LLM

Gemini LLM is a state-of-the-art language model known for its robust performance in generating human-like text based on given inputs. Its architecture leverages deep learning to understand and generate text that is coherent, contextually appropriate, and relevant to the user's query. In the context of RAG, Gemini LLM's generative power is crucial for creating informative and nuanced responses.

### FAISS

FAISS, developed by Facebook AI Research, is a highly efficient library for similarity search and clustering of dense vectors. It enables rapid and scalable retrieval of relevant documents from large datasets. By incorporating FAISS into a RAG system, we can quickly fetch pertinent information from vast repositories, which the generative model can then use to craft more accurate and contextually enriched responses.

### LangChain

LangChain is a framework designed for developing applications that utilize large language models. It provides a streamlined interface to integrate and manage different components of a language model pipeline, including retrieval mechanisms and generative models. LangChain facilitates the seamless interaction between Gemini LLM and FAISS, ensuring that the retrieved data is effectively utilized to enhance the generative process.

### Streamlit

Streamlit is an open-source framework for creating interactive and dynamic web applications. It is particularly useful for building user-friendly interfaces that allow users to interact with machine learning models in real-time. By leveraging Streamlit, we can develop intuitive applications that enable users to experience the power of RAG models firsthand, adjusting inputs and observing outputs dynamically.

## Combining the Technologies

The integration of Gemini LLM, FAISS, LangChain, and Streamlit offers a comprehensive solution for deploying advanced RAG models. FAISS handles the efficient retrieval of relevant information, which is then processed by LangChain to ensure smooth interaction with Gemini LLM. The generative capabilities of Gemini LLM are then leveraged to produce high-quality responses, which can be presented through an interactive Streamlit interface.

This powerful combination enables the creation of sophisticated AI applications capable of delivering accurate, contextually relevant, and engaging user experiences. Whether for customer support, content generation, or information retrieval, the synergy of these technologies paves the way for innovative solutions in the AI domain.

## Workflow: Step-by-Step
1. Imports all the dependencies.
2. Fetches and reads the pdf using pyPDF reader.
3. Splits the text into appropriate length chunks.
4. Computes an embedding to be stored in the vector database.
5. Creates a prompt template to provide a standard response.
Once the vector database is created,
1. A user can query the system with raw text.
2. An embedding is computed for the query.
3. Searchs the vector database for contextually relevant data.
4. Gives the relevant context and query to an LLM.
5. Returns a contextually enriched response to the user.
