# LLM-RAG


## Embedding

- Embedding은 대규모 언어 모델(LLM)에 있는 텍스트들의 연관성(Sementic meaning)을 벡터(Vector)로 표현합니다.  
  - Embeddings are numerical representations (vectors) created from generative AI that capture the semantic meaning of text input into a large language model (LLM)

![image](https://github.com/kyopark2014/LLM-RAG/assets/52392004/fc07e189-4767-42c4-92f6-1aca8ce6cd8d)
* [Building AI-powered search in PostgreSQL using Amazon SageMaker and pgvector](https://aws.amazon.com/blogs/database/building-ai-powered-search-in-postgresql-using-amazon-sagemaker-and-pgvector/) 참고
 
## Vector database

- 이미지, 문서(text document), 오디오와 같지 구조화되지 않은 컨텐츠(unstructured content)를 표현하는데 용이
- 벡터는 N개의 Dimension들을 가지고 있음
- Visual Search, 음악 검색, 개인화 추천

![image](https://github.com/kyopark2014/LLM-RAG/assets/52392004/993a666d-e4e9-493c-a5b4-35ce1c90d5bf)

Generative AI는 Vector database와 같은 외부 지식(External Knowledge Base)를 이용하여 Hallucination을 방지할 수 있습니다.

![image](https://github.com/kyopark2014/LLM-RAG/assets/52392004/2328ef01-5446-49ee-a25b-3a6af1266b3a)


### OpenSearch

[Amazon OpenSearch Service’s vector database capabilities explained](https://aws.amazon.com/ko/blogs/big-data/amazon-opensearch-services-vector-database-capabilities-explained/)와 같이 아래처럼 구성이 가능합니다.

![image](https://github.com/kyopark2014/LLM-RAG/assets/52392004/5c0f1df7-0f42-4086-a641-fe92a66835cf)


### PostgreSQL

2023년 5월 부터 RDS for PostgreSQL과 ML 모델 통합을 위해 [pgvector](https://aws.amazon.com/ko/about-aws/whats-new/2023/05/amazon-rds-postgresql-pgvector-ml-model-integration/)가 지원됩니다. 따라서, ML 모델의 Embedding을 데이터베이스에 저장하고 유사성검색(similarity search)을 할 수 있습니다.  

## Reference 

[Powering AI apps with AWS vector database options: Amazon OpenSearch Service and Amazon RDS for PostgreSQL - dbCON 2023](https://broadcast.amazon.com/videos/812948)

[Amazon OpenSearch Service’s vector database capabilities explained](https://aws.amazon.com/ko/blogs/big-data/amazon-opensearch-services-vector-database-capabilities-explained/)
