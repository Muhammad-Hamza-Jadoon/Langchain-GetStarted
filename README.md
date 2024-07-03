# Langchain Roadmap
These notebooks will walk you through my entire process of learning langchain. It contains all the steps I had to go through to master my grip on implementing RAG pipelines from sratch.  
I would recommend jumping straight into the notebooks and keep an eye for this Readme here. All notebooks explain every process extensively with self-made diagrams.

### Prerequisites
-----------

You will need to install Langchain for a start.

Notebooks specify rest of the requiremnets, including how to setup TogetherApi key.

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


### Notebook 3
-----------

* This is where sh*t finally started to make sense to me
* I downloaded multiple ML lecture pdf files from CS-32 Stanford website and decided to implement a RAG pipeline for multiple pdf files.
* Figured out how i could also use ``TogetherEmbeddings`` instead of ``OllamaEmbeddings``. Since finding embeddings takes alot of time, I had initially done this on Kaggle notebook with their provided gpu. For some reason OllamaEmbeddings was not working there so used TogetherEmbeddings instead and it worked well.
* This time around, I used chroma vector store and saved it in persist_directory to load later on.
* Understood the concept of smiliarity search and other similar search that can be used with the vector store created to find what relevant document pages are fetched from store when provided with a query.
* It the further dawned upon me that there are alot of different types of retrievers that are used to fetch relevant docs from vector database, like compression retriever, self-query-search retriever etc.
* Finally used the following two chains: ``ConversationalRetrievalChain`` and ``RetrievalQA`` to chat with pdfs using llms. Discovered how ``ConversationBufferMemory`` can also be used within these chains to keep track of conversation history.


### Contact
-------------

* Muhammad Hamza Jadoon
* muhammadhamzajadoon@gmail.com


