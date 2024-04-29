# Leveraging-LLM-RAG-for-Personalization
## Introduction
In today's fast-evolving digital space, personalization is key to enhancing user experience and satisfaction. This blog post aims to provide comprehensive insights into how Large Language Models (LLM) and Retrieval-Augmented Generation (RAG) can be leveraged to improve personalized product recommendations. By moving through the data preprocessing, embedding generation, and personalized reranking, we will demonstrate practical application of using LLM and RAG at generating recommendations that considers individual preferences.

## 1. Data Preprocessing
- **Libraries:** Import necessary Python libraries.
- **Dataset:** Load and preprocess the e-commerce dataset from Kaggle.
- **Preprocessing Steps:** Data cleaning including removal of null values, duplicates, and cancelled orders.
- **User History & Product Description Mapping:** Generate mappings for user purchase history and product descriptions.

## 2. Generating Product Embeddings
- **Embedding Model Setup:** Initialize and use the SentenceTransformer model for converting product descriptions into numerical embeddings.
- **ANN Index Setup:** Set up the Approximate Nearest Neighbor (ANN) index for embedding space.
- **Query-based Retrieval:** Implement functions to retrieve similar products based on user queries.
<h4 align=left> Query Retrieval Example </h4>
<img src="https://github.com/enisteper1/Leveraging-LLM-RAG-for-Personalization/assets/45767042/c014bd01-bc08-4982-801a-4d8afa3d901c" width="40%" height="40%">

## 3. Personalized Reranking
- **Model Setup:** Instructions for setting up and authenticating the Gemma-2B model from Hugging Face.
- **Showcasing Personalized Recommendations:** Demonstrates the use of structured prompts to guide the LLM in customizing product suggestions based on historical user data.
- **Why Utilize LLM for Reranking?:** Highlights the benefits of LLMs in reranking, focusing on their ability to contextualize recommendations and provide clear, rationale-driven outputs.
<h4 align=left> Basic Product Reranking</h4>
<img src="https://github.com/enisteper1/Leveraging-LLM-RAG-for-Personalization/assets/45767042/ba5722aa-e0b6-43de-95c6-4676c7347033"" width="40%" height="40%">
<h4 align=left> Product Reranking with Explanation</h4>
<img src="https://github.com/enisteper1/Leveraging-LLM-RAG-for-Personalization/assets/45767042/caa4989f-1b14-488d-8a2d-173b68b5c89f"" width="70%" height="70%">

## Conclusion
This exploration has shown the implementation of LLM and RAG in personalized recommendations. The goal of this post was to clarify how these technologies can be integrated into existing systems, moving through each step from initial data preprocessing to the reranking of products. The insights here are designed to help developers and businesses utilize the potential of LLM and RAG to advance personalized e-commerce experiences. Since the system has potential to enhance relevance and personal appeal of their product recommendations, one can ensure more engaging and satisfying customer journey.

You can access the full code for this blog post on either Colab or GitHub to illustrate results on your own.  I strongly suggest checking the references that formed the basis for my implementation.

## Future Works
Since the purpose of this post was to provide an insight about using LLM & RAG in personalization, results can be still enhanced. Here is the list of what can be done as a future work:

- **Using a larger dataset**: Expanding the dataset can increase potential reranking by exposing it to a more varied dataset.
- **Using more complex models**: Using advanced language models and sophisticated embedding techniques can enhance the quality and relevance of the recommendations.
- **Generating embeddings from item to item relations**: Generating embeddings from the relationships between items can enhance the potential for personalized reranking.
## References
- https://qdrant.tech/articles/what-is-rag-in-ai
- https://huggingface.co/learn/cookbook/en/rag_with_hugging_face_gemma_mongodb
- https://www.kaggle.com/datasets/carrie1/ecommerce-data/data
- https://www.kaggle.com/code/fabiendaniel/customer-segmentation
- https://huggingface.co/thenlper/gte-small
