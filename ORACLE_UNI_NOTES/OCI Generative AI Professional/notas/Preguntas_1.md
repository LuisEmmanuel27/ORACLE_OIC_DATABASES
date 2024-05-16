# Preguntas curso

## 1 - 5 Fundamentals of Large Language Models
## 6 - 10 Generative AI Service

1. What is prompt engineering in the context of Large Language Models (LLMs)?
   1. Iteratively refining the ask to elicit a desired response
   2. Training the model on a large data set
   3. Adjusting the hyperparameters of the model
   4. Adding more layers to the neural network<br><br>
2. What does the term "hallucination" refer to in the context of Language Large Models (LLMs)?
   1. The model's ability to generate imaginative and creative content
   2. The process by which the model visualizes and describes images in detail
   3. A technique used to enhance the model's performance on specific tasks
   4. The phenomenon where the model generates factually incorrect information or unrelated content as if it were true<br><br>
3. What does in-context learning in Large Language Models involve?
   1. Pretraining the model on a specific domain
   2. Conditioning the model with task-specific instructions or demonstrations
   3. Training the model using reinforcement learning
   4. Adding more layers to the model<br><br>
4. Which statement accurately reflects the differences between these approaches in terms of the number of parameters modified and the type of data used?
   1. Parameter Efficient Fine Tuning and Soft prompting modify all parameters of the model using unlabeled data.
   2. Fine-tuning modifies all parameters using labeled, task-specific data, whereas Parameter Efficient Fine-Tuning updates a few, new parameters also with labeled, task-specific data.
   3. Soft prompting and continuous pretraining are both methods that require no modification to the original parameters of the model.
   4. Fine-tuning and continuous pretraining both modify all parameters and use labeled, task-specific data.<br><br>
5. What is the role of temperature in the decoding process of a Large Language Model (LLM)?
   1. To determine the number of words to generate in a single decoding step
   2. To increase the accuracy of the most likely word in the vocabulary
   3. To decide to which part of speech the next word should belong
   4. To adjust the sharpness of probability distribution over vocabulary when selecting the next word<br><br>
6. What happens if a period (.) is used as a stop sequence in text generation?
   1. The model generates additional sentences to complete the paragraph.
   2. The model stops generating text after it reaches the end of the current paragraph.
   3. The model stops generating text after it reaches the end of the first sentence, even if the token limit is much higher.
   4. The model ignores periods and continues generating text until it reaches the token limit.<br><br>
7. Which is a distinctive feature of GPUs in Dedicated AI Clusters used for generative AI tasks?
   1. GPUs are used exclusively for storing large data sets, not for computation.
   2. Each customer's GPUs are connected via a public Internet network for ease of access.
   3. GPUs are shared with other customers to maximize resource utilization.
   4. The GPUs allocated for a customer’s generative AI tasks are isolated from other GPUs.<br><br>
8. What is the main advantage of using few-shot model prompting to customize a Large Language Model (LLM)?
   1. It allows the LLM to access a larger data set.
   2. It provides examples in the prompt to guide the LLM to better performance with no training cost.
   3. It significantly reduces the latency for each model request.
   4. It eliminates the need for any training or computational resources.<br><br>
9. What is the purpose of frequency penalties in language model outputs?
   1.  To ensure that tokens that appear frequently are used more often
   2.  To penalize tokens that have already appeared, based on the number of times they have been used
   3.  To reward the tokens that have never appeared in the text
   4.  To randomly penalize some tokens to increase the diversity of the text<br><br>
10. What is the purpose of embeddings in natural language processing?
    1.  To create numerical representations of text that capture the meaning and relationships between words or phrases
    2.  To increase the complexity and size of text data
    3.  To compress text data into smaller files for storage
    4.  To translate text into a different language

# Respuestas

1. `Iteratively refining the ask to elicit a desired response` - Prompt engineering in the context of Large Language Models (LLMs) refers to the practice of designing and refining prompts or input instructions to elicit desired responses from the model. It involves crafting specific textual cues or queries that guide the model towards generating outputs that align with the user's intentions or requirements.
2. `The phenomenon where the model generates factually incorrect information or unrelated content as if it were true` - Hallucination occurs when the model generates text that seems plausible or coherent but is not grounded in factual reality or relevant to the task at hand. Hallucination can be problematic, especially in applications where generating accurate and reliable information is crucial, such as question answering, summarization, or content generation for decision-making.
3. `Conditioning the model with task-specific instructions or demonstrations` - In-context learning in Large Language Models (LLMs) involves updating or fine-tuning a pretrained language model with additional data or examples specific to a particular context or domain. This process enables the model to adapt its knowledge and capabilities to better suit the requirements of a specific task or application.
4. `Fine-tuning modifies all parameters using labeled, task-specific data, whereas Parameter Efficient Fine-Tuning updates a few, new parameters also with labeled, task-specific data.` - Fine-tuning involves adjusting all parameters of the pretrained model using labeled, task-specific data. This means that the entire model architecture is modified based on the new task or domain-specific data. Parameter Efficient Fine-Tuning updates only a subset of parameters within the pre-trained model, typically focusing on specific layers or components that are relevant to the new task. Despite this, both Fine-tuning and Parameter Efficient Fine-Tuning utilize labeled, task-specific data for training.
5. `To adjust the sharpness of probability distribution over vocabulary when selecting the next word` - When decoding with an LLM, the model assigns probabilities to each word in the vocabulary for the next word in the sequence. Temperature controls the sharpness or smoothness of this probability distribution. A low temperature value results in a sharper distribution, which means that the model is more confident in its predictions and tends to select the most likely word with higher probability. Conversely, a higher temperature value smooths out the distribution, making it more likely for lower probability words to be chosen, leading to more diverse and varied output.
6. `The model stops generating text after it reaches the end of the first sentence, even if the token limit is much higher` - Stop sequences, in the context of text generation, are special tokens or symbols used to signal the end of the generated text. These sequences serve as markers for the model to halt its generation process. Common stop sequences include punctuation marks such as periods (.), question marks (?), and exclamation marks (!), because they typically denote the end of sentences in natural language.
7. `The GPUs allocated for a customer’s generative AI tasks are isolated from other GPUs` - The GPUs allocated for a customer’s generative AI tasks are isolated from other GPUs to maintain the security and privacy of the customer data and workloads.
8. `It provides examples in the prompt to guide the LLM to better performance with no training cost` - The main advantage of using few-shot model prompting to customize a Large Language Model (LLM) is its ability to adapt the model quickly and effectively to new tasks or domains with only a small amount of training data. Instead of retraining the entire model from scratch, which can be time-consuming and resource-intensive, few-shot prompting leverages the model's pre-existing knowledge.
9. `To penalize tokens that have already appeared, based on the number of times they have been used` - Frequency penalties in language model outputs aim to discourage the repetition of tokens that have already appeared in the generated text. When generating text, language models may tend to produce repetitive phrases or words, which can lead to less diverse and less interesting outputs. By applying frequency penalties, tokens that have been used multiple times are penalized, reducing the likelihood of their repetition in subsequent generations.
10. `To create numerical representations of text that capture the meaning and relationships between words or phrases` - Embeddings map words or text onto a continuous vector space where similar words are located close to each other. This allows NLP models to capture semantic relationships between words, such as synonyms or related concepts. For example, in a well-trained embedding space, the vectors for "king" and "queen" would be closer to each other than to unrelated words like "car" or "tree." Embeddings also provide a dense, low-dimensional representation of words compared to traditional one-hot encodings. This makes them more efficient and effective as input features for machine learning models, reducing the dimensionality of the input space, and improving computational efficiency.