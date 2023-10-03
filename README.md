# EcoMed Expert 👨‍⚕️🏭

Welcome to EcoMed 🤖 Expert, your trusted companion for a healthier you and a greener planet! Our chatbot is here to empower you with knowledge and solutions that not only enhance your well-being but also contribute to a sustainable world. Whether you have questions about your health or seek insights into environmental science, we've got you covered. Join us on a journey to treat yourself and the environment with care, making a positive impact every day.


We are using a methodology called as Retrieval Augmented generation:

![Retrival Augmented Generation Methodology](images/rag.jpg)

In RAG, the external data can come from multiple data sources, such as a document repository, databases, or APIs. The first step is to convert the documents and the user query in the format so they can be compared and relevancy search can be performed. To make the formats comparable for doing relevancy search, a document collection (knowledge library) and the user-submitted query are converted to numerical representation using embedding language models. The embeddings are essentially numerical representations of concept in text. Next, based on the embedding of user query, its relevant text is identified in the document collection by a similarity search in the embedding space. Then the prompt provided by the user is appended with relevant text that was searched and it’s added to the context. The prompt is now sent to the LLM and because the context has relevant external data along with the original prompt, the model output is relevant and accurate.