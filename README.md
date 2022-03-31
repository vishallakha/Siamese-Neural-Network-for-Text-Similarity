## Description
I have implemented a Siamese Neural Network for text similarity. It takes two sentences as input and predicts the similarity between them. Here one input comes from the user and the other input is a entire dataset of documents in the data lake. 
It implements BERT embeddings for both the sentences, takes the average pooling and gives the output as 1024 dimensional vector embeddings. These embeddings are stored in Mongo DB so that they can be easily used again and again without recalculations.then the cosine similarity between the two sentences is calculated and a document is ranked through a special aggregation logic based on domain.
## Technology Stack
BERT, Siamese Neural Network, Hugging Face, MongoDB