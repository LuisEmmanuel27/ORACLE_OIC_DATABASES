# Preguntas curso

## 1 - 5 Fundamentals of Large Language Models

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

# Respuestas

1. `Iteratively refining the ask to elicit a desired response` - Prompt engineering in the context of Large Language Models (LLMs) refers to the practice of designing and refining prompts or input instructions to elicit desired responses from the model. It involves crafting specific textual cues or queries that guide the model towards generating outputs that align with the user's intentions or requirements.
2. `The phenomenon where the model generates factually incorrect information or unrelated content as if it were true` - Hallucination occurs when the model generates text that seems plausible or coherent but is not grounded in factual reality or relevant to the task at hand. Hallucination can be problematic, especially in applications where generating accurate and reliable information is crucial, such as question answering, summarization, or content generation for decision-making.
3. `Conditioning the model with task-specific instructions or demonstrations` - In-context learning in Large Language Models (LLMs) involves updating or fine-tuning a pretrained language model with additional data or examples specific to a particular context or domain. This process enables the model to adapt its knowledge and capabilities to better suit the requirements of a specific task or application.
4. `Fine-tuning modifies all parameters using labeled, task-specific data, whereas Parameter Efficient Fine-Tuning updates a few, new parameters also with labeled, task-specific data.` - Fine-tuning involves adjusting all parameters of the pretrained model using labeled, task-specific data. This means that the entire model architecture is modified based on the new task or domain-specific data. Parameter Efficient Fine-Tuning updates only a subset of parameters within the pre-trained model, typically focusing on specific layers or components that are relevant to the new task. Despite this, both Fine-tuning and Parameter Efficient Fine-Tuning utilize labeled, task-specific data for training.
5. `To adjust the sharpness of probability distribution over vocabulary when selecting the next word` - When decoding with an LLM, the model assigns probabilities to each word in the vocabulary for the next word in the sequence. Temperature controls the sharpness or smoothness of this probability distribution. A low temperature value results in a sharper distribution, which means that the model is more confident in its predictions and tends to select the most likely word with higher probability. Conversely, a higher temperature value smooths out the distribution, making it more likely for lower probability words to be chosen, leading to more diverse and varied output.