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
    1. Only after the output has been generated.
    2. Before user input and after chain execution.
    3. After user input but before chain execution, and again after core logic but before output.
    4. Continuously throughout the entire chain execution process.<br><br>
10. What does a cosine distance of 0 indicate about the relationship between two embeddings?
    1. They have the same magnitude
    2. They are similar in direction
    3. They are completely dissimilar
    4. They are unrelated<br><br>
11. How does a presence penalty function in language model generation?
    1. It penalizes a token each time it appears after the first occurrence.
    2. It penalizes only tokens that have never appeared in the text before.
    3. It penalizes all tokens equally, regardless of how often they have appeared.
    4. It applies a penalty only if the token has appeared more than twice.<br><br>
12. What is the purpose of Retrievers in LangChain?
    1. To combine multiple components into a single pipeline
    2. To break down complex tasks into smaller steps
    3. To train Large Language Models
    4. To retrieve relevant information from knowledge bases<br><br>
13. How does the temperature setting in a decoding algorithm influence the probability distribution over the vocabulary?
    1. Decreasing the temperature broadens the distribution, making less likely words more probable.
    2. Increasing the temperature flattens the distribution, allowing for more varied word choices.
    3. Increasing the temperature removes the impact of the most likely word.
    4. Temperature has no effect on probability distribution; it only changes the speed of decoding.<br><br>
14. Which statement is true about string prompt templates and their capability regarding variables?
    1. They require a minimum of two variables to function properly.
    2. They are unable to use any variables.
    3. They support any number of variables, including the possibility of having none.
    4. They can only support a single variable at a time.<br><br>
15. Why is it challenging to apply diffusion models to text generation?
    1. Because text is not categorical
    2. Because text representation is categorical unlike images
    3. Because diffusion models can only produce images
    4. Because text generation does not require complex models<br><br>
16. What do prompt templates use for templating in language model applications?
    1. Python's list comprehension syntax
    2. Python's lambda functions
    3. Python's class and object structures
    4. Python's str.format syntax<br><br>
17. How can the concept of "Groundedness" differ from "Answer Relevance" in the context of Retrieval Augmented Generation (RAG)?
    1. Groundedness refers to contextual alignment, whereas Answer Relevance deals with syntactic accuracy.
    2. Groundedness measures relevance to the user query, whereas Answer Relevance evaluates data integrity.
    3. Groundedness focuses on data integrity, whereas Answer Relevance emphasizes lexical diversity.
    4. Groundedness pertains to factual correctness, whereas Answer Relevance concerns query relevance.<br><br>
18. Which LangChain component is responsible for generating the linguistic output in a chatbot system?
    1. Vector Stores
    2. Document Loaders
    3. LLMs
    4. LangChain Application<br><br>
19. What does the RAG Sequence model do in the context of generating a response?
    1. For each input query, it retrieves a set of relevant documents and considers them together to generate a cohesive response.
    2. It retrieves a single relevant document for the entire input query and generates a response based on that alone.
    3. It modifies the input query before retrieving relevant documents to ensure a diverse response.
    4. It retrieves relevant documents only for the initial part of the query and ignores the rest.<br><br>
20. In the context of generating text with a Large Language Model (LLM), what does the process of greedy decoding entail?
    1. Selecting a random word from the entire vocabulary at each step
    2. Picking a word based on its position in a sentence structure
    3. Using a weighted random selection based on a modulated distribution
    4. Choosing the word with the highest probability at each step of decoding<br><br>
21. Given the following code block: history = StreamlitChatMessageHistory(key="chat_messages") memory = ConversationBufferMemory(chat_memory=history) <br><br> Which statement is NOT true about StreamlitChatMessageHistory?
    1. StreamlitChatMessageHistory can be used in any type of LLM application.
    2. A given StreamlitChatMessageHistory will NOT be persisted.
    3. StreamlitChatMessageHistory will store messages in Streamlit session state at the specified key.
    4. A given StreamlitChatMessageHistory will not be shared across user sessions.<br><br>
22. Which statement is true about Fine-tuning and Parameter-Efficient Fine-Tuning (PEFT)?
    1. PEFT requires replacing the entire model architecture with a new one designed specifically for the new task, making it significantly more data-intensive than Fine-tuning.
    2. Both Fine-tuning and PEFT require the model to be trained from scratch on new data, making them equally data and computationally intensive.
    3. Fine-tuning requires training the entire model on new data, often leading to substantial computational costs, whereas PEFT involves updating only a small subset of parameters, minimizing computational requirements and data needs.
    4. Fine-tuning and PEFT do not involve model modification; they differ only in the type of data used for training, with Fine-tuning requiring labeled data and PEFT using unlabeled data.<br><br>
23. Which is a characteristic of T-Few fine-tuning for Large Language Models (LLMs)?
    1. It updates all the weights of the model uniformly.
    2. It does not update any weights but restructures the model architecture.
    3. It selectively updates only a fraction of the model's weights.
    4. It increases the training time as compared to Vanilla fine-tuning.<br><br>
24. In the simplified workflow for managing and querying vector data, what is the role of indexing?
    1. To categorize vectors based on their originating data type (text, images, audio)
    2. To compress vector data for minimized storage usage
    3. To convert vectors into a nonindexed format for easier retrieval
    4. To map vectors to a data structure for faster searching, enabling efficient retrieval<br><br>
25. What does accuracy measure in the context of fine-tuning results for a generative model?
    1. How many predictions the model made correctly out of all the predictions in an evaluation
    2. The depth of the neural network layers used in the model
    3. The proportion of incorrect predictions made by the model during an evaluation
    4. The number of predictions a model makes, regardless of whether they are correct or incorrect<br><br>
26. What does the Loss metric indicate about a model's predictions?
    1. Loss indicates how good a prediction is, and it should increase as the model improves.
    2. Loss measures the total number of predictions made by a model.
    3. Loss describes the accuracy of the right predictions rather than the incorrect ones.
    4. Loss is a measure that indicates how wrong the model's predictions are.<br><br>
27. How are documents usually evaluated in the simplest form of keyword-based search?
    1. According to the length of the documents
    2. Based on the presence and frequency of the user-provided keywords
    3. Based on the number of images and videos contained in the documents
    4. By the complexity of language used in the documents<br><br>
28. What is the purpose of Retrieval Augmented Generation (RAG) in text generation?
    1. To generate text using extra information obtained from an external data source
    2. To retrieve text from an external source and present it without any modifications
    3. To generate text based only on the model's internal knowledge without external data
    4. To store text in an external database without using it for generation<br><br>
29. When is fine-tuning an appropriate method for customizing a Large Language Model (LLM)?
    1. When you want to optimize the model without any instructions
    2. When the LLM does not perform well on a task and the data for prompt engineering is too large
    3. When the LLM already understands the topics necessary for text generation
    4. When the LLM requires access to the latest data for generating outputs<br><br>
30. Accuracy in vector databases contributes to the effectiveness of Large Language Models (LLMs) by preserving a specific type of relationship. What is the nature of these relationships, and why are they crucial for language models?
    1. Linear relationships; they simplify the modeling process
    2. Temporal relationships; necessary for predicting future linguistic trends
    3. Hierarchical relationships; important for structuring database queries
    4. Semantic relationships; crucial for understanding context and generating precise language<br><br>
31. What is LangChain?
    1. A Java library for text summarization
    2. A Python library for building applications with Large Language Models
    3. A Ruby library for text generation
    4. A JavaScript library for natural language processing<br><br>

# Respuestas

1. `Increasing temperature flattens the distribution, allowing for more varied word choices.`
2. `When there is a need to add learnable parameters to a large language model (LLM) without task-specific training.` - Soft prompting refers to a technique where additional parameters are introduced into a model's input layer in the form of embeddings, which are tuned during training. This can be particularly useful when one wants to adapt a large pretrained model to a new task without modifying the entire model's weights, which is resource-intensive. When there is a significant amount of labeled, task-specific data available, traditional fine-tuning or transfer learning might be more suitable.
   When the model needs to be adapted to perform well in a different domain it was not originally trained on, domain adaptation techniques that may involve fine-tuning or prompt-based approaches are commonly used, but this doesn't specifically denote soft prompting.
   When the model requires continued pretraining on unlabeled data, unsupervised or self-supervised learning techniques are typically employed, not soft prompting.
3. `Chain-of-Thought.`
4. `It penalizes a token each time it appears after the first occurrence.`
5. `It selectively updates only a fraction of weights to reduce computational load and avoid overfitting.`
6. `480 unit hours`
7. `An LLM enhanced with Retrieval-Augmented Generation (RAG) for dynamic information retrieval and response generation.`
8. `It is based on distances and similarities in a vector space.`
9. `After user input but before chain execution, and again after core logic but before output.`
10. `They are similar in direction`
11. `It penalizes a token each time it appears after the first occurrence.`
12. `To retrieve relevant information from knowledge bases`
13. `Increasing the temperature flattens the distribution, allowing for more varied word choices.` - Increasing the temperature makes the distribution flatter, which means the difference between the probabilities of the most likely word and the less likely words is decreased. This allows for more varied and sometimes more creative or unexpected word choices.
14. `They support any number of variables, including the possibility of having none.`
15. `Because text representation is categorical unlike images` - Diffusion models work well with continuous data, where the process involves gradually adding noise to the data and then learning to reverse this process. In image generation, this works well because pixel values are inherently continuous. Text data, on the other hand, is discrete and categorical; words are symbols that come from a fixed vocabulary and they can't be meaningfully interpolated like pixel values. This discreteness means that you can't directly apply the same gradual noise and denoising process that works for images.
16. `Python's str.format syntax`
17. `Groundedness pertains to factual correctness, whereas Answer Relevance concerns query relevance.`
18. `LLMs`
19. `For each input query, it retrieves a set of relevant documents and considers them together to generate a cohesive response.`
20. `Choosing the word with the highest probability at each step of decoding` - The process of greedy decoding entails choosing the word with the highest probability at each step of decoding. In this approach, at every step of the sequence generation, the model looks at the probabilities it has assigned to each possible next word (given the context of all the previously selected words) and selects the
21. `StreamlitChatMessageHistory can be used in any type of LLM application.`
22. `Fine-tuning requires training the entire model on new data, often leading to substantial computational costs, whereas PEFT involves updating only a small subset of parameters, minimizing computational requirements and data needs.` - Fine-tuning typically involves adjusting the weights of a pretrained model across all layers to better perform on a specific task. It requires running the entire data set through the model, which can be computationally expensive, especially with large models. PEFT is a technique developed to fine-tune large models more efficiently. Instead of updating all the parameters, PEFT techniques update only a small subset of the parameters or add small, trainable modules within the model while keeping most of the original pretrained parameters frozen.
23. `It selectively updates only a fraction of the model's weights.` - In the context of fine-tuning Large Language Models (LLMs), the T-Few method is characterized by selectively updating a fraction of the model's weights. This approach is a form of parameter-efficient fine-tuning that aims to fine-tune large models without updating all of the weights, thus saving on computational resources and time.
24. `To map vectors to a data structure for faster searching, enabling efficient retrieval` - Indexing structures organize data in a way that optimizes retrieval operations, such as nearest neighbor search, which is commonly used for finding the most similar vectors. When dealing with high-dimensional data, like vectors representing complex entities or embeddings, linear search can be slow because it requires comparing the query vector to every vector in the data set.
25. `How many predictions the model made correctly out of all the predictions in an evaluation`
26. `Loss is a measure that indicates how wrong the model's predictions are.` - Loss is a quantification of the error between what the model predicts and what the actual value or label is. The higher the loss, the greater the error, and conversely, the lower the loss, the more accurate the model’s predictions are with respect to the provided data. During training, the objective is to minimize this loss to improve the model's performance. The loss function guides the optimization algorithm on how to adjust the model's weights to make more accurate predictions.
27. `Based on the presence and frequency of the user-provided keywords`
28. `To generate text using extra information obtained from an external data source` - The purpose of RAG in text generation is to generate text using extra information retrieved from an external source. RAG combines a retrieval step with a generation step: the model first retrieves relevant documents or passages from a large corpus like Wikipedia or a domain-specific dataset and then uses the content of these documents to inform the generation of text.
29. `When the LLM does not perform well on a task and the data for prompt engineering is too large` - Fine-tuning involves continuing the training of a pre-trained model on a specific data set to adapt the model to particular tasks or domains. This process adjusts the weights across all the layers of the model based on the new data, allowing the model to better understand and generate text relevant to the specifics of the data set or domain.
30. `Semantic relationships; crucial for understanding context and generating precise language` - Semantic relationships in vector spaces (often created through methods like word embedding) are foundational to the way LLMs understand and process language. They capture the meaning and context of words or phrases, enabling the model to produce relevant and contextually appropriate responses. If these relationships are accurately preserved in a vector database.
31. `A Python library for building applications with Large Language Models`

# [Siguiente](./Preguntas_3.md)
