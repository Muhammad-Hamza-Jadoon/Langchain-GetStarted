# Langchain Roadmap
These notebooks will walk you through my entire process of learning langchain. It contains all the steps I had to go through to master my grip on implementing RAG pipelines from sratch.  
I would recommend jumping straight into the notebooks and keep an eye for this Readme here. All notebooks explain every process extensively with self-made diagrams.

### Prerequisites
-----------

You will need to install Langchain for a start.

Notebooks specify rest of the requiremnets, including TogetherApi key.

### Notebook 1
-----------

* I tried to create simple chain to chat with model using prompt.
* Then I tried to maintain history of my conversation as well this time but couldn't pull it off. I was introduced to a new prblem named ``hallucination``.
* Figured how I could use prompt to directly do any task like summarize, translate from language to language etc.


### Notebook 2
-----------

* Here is whenre external sources (text in this case) are used when getting response from an LLM.
* Created vector store for the first time, I was still relatively unfamilar with what a Vector Store is and understood it well later on (in my notebooks).
* Understood these certain ``RunnableParallel`` and ``RunnablePassthrough`` and how they can assist me with creating chains in langchain for inference.
* Finally understood what vector-store does. Used `FAISS` vector-store, then explained and used all these chains: `create_stuff_documents_chain` and `create_retrieval_chain` to implement a simple RAG pipeline where I would be able to provide a pdf file and ask question related to it


### Contact
-------------

* Muhammad Hamza Jadoon
* muhammadhamzajadoon@gmail.com


