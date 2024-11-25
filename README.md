This project is an AI-powered solution for creating personalized newsletters based on user-defined topics of interest. It utilizes various AI tools and APIs to deliver a seamless process from fetching relevant news articles to generating a polished newsletter with summaries and visuals.

Project Workflow
User Input:
The user specifies their topics of interest.

Article Retrieval:
Relevant news articles are fetched using the News API, tailored to the user’s chosen topics.

Data Preprocessing:

The fetched articles are divided into smaller, manageable chunks.
Embeddings are generated for these chunks using a vector embedding model.
Embedding Storage:
The embeddings are stored in a ChromaDB database, allowing for efficient retrieval.

Summary Generation:

Language Model: The Large Language Model (LLM) used for summarization is Groq, providing fast and accurate text generation.
Individual Summaries: Summaries are created for each article within the user's topics of interest.
Comprehensive Summary: A combined summary is generated, synthesizing key insights from the individual summaries.
Image Generation:

A prompt is created based on the article content and passed to the Stable Diffusion 3.5 model.
Relevant and visually appealing images are generated to complement the newsletter content.
Newsletter Compilation:
The summaries and generated images are combined into a cohesive newsletter.

Key Features
Personalized Content: News tailored to user-defined interests.
Efficient Storage and Retrieval: Utilizes ChromaDB for embedding management.
AI-Powered Summarization: Summaries generated at both granular and comprehensive levels using Groq LLM.
Visual Enhancements: AI-generated images created using Stable Diffusion 3.5.
This pipeline ensures the delivery of an engaging and informative newsletter with minimal user effort.
