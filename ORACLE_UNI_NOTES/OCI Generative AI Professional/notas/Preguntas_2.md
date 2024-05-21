# Sample Exam Questions - Part 1 & 2

1. How does the temperature setting in a decoding algorithm influence the probability distribution over the Vocabulary?
   1. Increasing temperature removes the impact of the most likely word.
   2. Decreasing temperature broadens the distribution, making less likely words more probable.
   3. Increasing temperature flattens the distribution, allowing for more varied word choices.
   4. Temperature has no effect on the probability distribution; it only changes the speed of decoding.<br><br>
2. In which scenario is soft prompting especially appropriate compared to other training styles?
   1. When there is a significant amount of labeled, task-specific data available.
   2. When the model needs to be adapted to perform well in a different domain it was not originally trained on.
   3. When there is a need to add learnable parameters to a large language model (LLM) without task-specific training.
   4. When the model requires continued pre-training on unlabeled data.<br><br>
3. An LLM emits intermediate reasoning steps as part of its responses. Which of the following techniques is being utilized?
   1. In-context Learning.
   2. Step-Back Prompting.
   3. Least-to-most Prompting.
   4. Chain-of-Thought.<br><br>
4. How does a presence penalty function in language model generation when using OCI Generative AI service?
   1. It penalizes all tokens equally, regardless of how often they have appeared.
   2. It only penalizes tokens that have never appeared in the text before.
   3. It applies a penalty only if the token has appeared more than twice.
   4. It penalizes a token each time it appears after the first occurrence.<br><br> 
5. What is the characteristic of T-Few fine-tuning for Large Language Models (LLMs)?
   1. It updates all the weights of the model uniformly.
   2. It selectively updates only a fraction of weights to reduce the no. of parameters.
   3. It selectively updates only a fraction of weights to reduce computational load and avoid overfitting.
   4. It increases the training time as compared to Vanilla fine tuning.<br><br>
6. You create a fine-tuning dedicated AI cluster to customize a foundational model with your custom training data. **How many unit hours are required for fine-tuning if the cluster is active for 10 days?**
   1. 480 unit hours
   2. 240 unit hours
   3. 744 unit hours
   4. 20 unit hours<br><br>
7. An AI development company is working on an AI assisted chatbot for a customer which happens to be an online retail company. The goal is to create an assistant that can best answer queries regarding the company polices as well as retain the chat history throughout a session. **Considering the capabilities, which type of model would be the best?**
   1. A keyword search-based AI that responds based on specific keywords identified in customer queries.
   2. An LLM enhanced with Retrieval-Augmented Generation (RAG) for dynamic information retrieval and response generation.
   3. An LLM dedicated to generating text responses without external data integration.
   4. A pre-trained LLM model from Cohere or OpenAI.<br><br>
8. How does the structure of vector databases differ from traditional relational databases?
   1. It stores data in a linear or tabular format.
   2. It is not optimized for high-dimensional spaces.
   3. It uses simple row-based data storage.
   4. It is based on distances and similarities in a vector space.<br><br> 
9. When does a chain typically interact with memory in a run within the LangChain framework?
   1.  Only after the output has been generated.
   2.  Before user input and after chain execution.
   3.  After user input but before chain execution, and again after core logic but before output.
   4.  Continuously throughout the entire chain execution process.<br><br>

# Respuestas

1. `Increasing temperature flattens the distribution, allowing for more varied word choices.`
2. `When there is a need to add learnable parameters to a large language model (LLM) without task-specific training.`
3. `Chain-of-Thought.`
4. `It penalizes a token each time it appears after the first occurrence.`
5. `It selectively updates only a fraction of weights to reduce computational load and avoid overfitting.`
6. `480 unit hours`
7. `An LLM enhanced with Retrieval-Augmented Generation (RAG) for dynamic information retrieval and response generation.`
8. `It is based on distances and similarities in a vector space.`
9. `After user input but before chain execution, and again after core logic but before output.`

# [Siguiente](./Preguntas_3.md)