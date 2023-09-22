# document-retrieval
##Using Topic-Based Query Paraphrasing to improve document retrieval in Learning to Rank Model


###ABSTRACT
Query Reformulation is a popular information retrieval method
to retrieve relevant documents from a huge corpus for a given
search query. Query paraphrasing is one of the effective techniques
which improves retrieval effectiveness. However, query expansion
using existing techniques gives good results for general queries but
performs poorly on queries that require capturing the domain of the
query. For domain-specific queries, the query expansion techniques
do not take into consideration the relevance of a document in a
particular domain. Also, training a model for domain-specific query
reformulation requires a manually annotated dataset for every
domain. Dataset annotation is expensive, time-consuming, and
not a scalable option. Our project is aimed at using Topic-modeling
for domain-specific query expansion to improve document retrieval
for user-given queries. We have developed two models, one where
the query paraphrasing is done by performing topic-modeling for
query reformulation and the other uses a pre-trained Sentence
BERT model. Both the models are learning to rank models where
few documents are retrieved from a large collection using the BM25
retrieval model and then the retrieved documents are passed to a
BERT model which is trained using the topic-based and paraphrased
queries respectively. We evaluate and compare both models on
different metrics including MAP and NDCG
