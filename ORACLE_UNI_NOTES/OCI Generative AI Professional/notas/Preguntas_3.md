# IZ0-1027-24 Generative AI Dump

## Preguntas

1. In LangChain, which retriever search type is used to balance between relevancy and diversity?
    1. top k
    2. mmr
    3. similarity_score_threshold
    4. similarity<br><br>
2. What does a dedicated RDMA cluster network do during model fine-tuning and inference?
    1. It leads to higher latency in model inference
    2. It enables the deployment of multiple fine-tuned models within a single cluster
    3. It limits the number of fine-tuned models deployable on the same GPU cluster
    4. It increases GPU memory requirements for model deployment<br><br>
3. Which role a "model endpint" serve in the inference workflow ofthe OCI Generative AI service?
    1. Hosts the training data for fine-tuning custom models
    2. Evaluates the performance metrics of the custom models
    3. Servers as a designated point for user requests and model responses
    4. Updates the weights of the base model during the fine-tuning process<br><br>
4. Which is a distinguishing feature of "Parameter-Effcient Fine-tuning (PEFT) as opposed to classic "Fine- tuning' in Large Language Model training?
    1. PEFT involves only a few or new parameters and uses labeled, task-specific data.
    2. PEFT modifies all parameters and uses unlabeled, task-agnostic data.
    3. PEFT does not modify any parameters but uses soft prompting with unlabeled data.
    4. PEFT modifies all parameters and is typically used when no training data exists.<br><br>
5. How does the Retrieval-Augmented Generation (RAG) Token technique differ from RAG Sequence when generating a model's response?
    1. Unlike RAG Sequence, RAG Token generates the entire response at once without considering individual parts.
    2. RAG Token does not use document retrieval but gengrates responses based on pre-existing knowledge only.
    3. RAG Token retrieves documents only at the beginning of the response generation and uses those for the entire content.
    4. RAG Token retrieves relevant documents for each part of the response and constructs the answer incrementally.<br><br>
6. Which component of Retrieval-Augmented Generation (RAG) evaluates and prioritizes the information retrieved by the retrieval system?
    1. Retriever
    2. Encoder-decoder
    3. Ranker
    4. Generator<br><br>
7. Which statement describes the difference between "Top k" and "Top p" in selecting the next token in the OCI Generative AI Generation models?
    1. Top k selects the next token based on its position in the list of probable tokens, whereas "Top p" selects based on the cumulative probability of the top tokens.
    2. Top k considers the sum ofprobabilities of the top tokens, whereas "Top p" selects from the "Top k" tokens sorted by probability.
    3. Top k and "Top p" both select from the same set of tokens but use different methods to prioritize them based on frequency.
    4. Top k and "Top p" are identical in their approach to token selection but differ in their application of penalties to tokens.<br><br>
8. Which statement is true about the "Top p" parameter of the OCI Generative Al Generation models?
    1. Top p assigns to frequently occurring tokens.
    2. Top p determines the maximum number oftokens
    3. Top p limits token selection based on the sum of their probabilities.
    4. Top p selects tokens from the "Top k" tokens sorted by probability.<br><br>
9. What is the primary function ofthe "temperature" parameter in the OCI Generative Al Generation models?
    1. Determines the maximum number of tokens the model can generate per response
    2. Specifies a string that tells the model to stop generating more content
    3. Assigns a penalty to tokens that have already appeared in the preceding text
    4. Controls the randomness of the model's output, affecting its creativity<br><br>
10. What distinguishes the Cohere Embed v3 model from its predecessor in the OCI Generative Al service?
    1. Improved retrievals for Retrieval-Augmented Generation (RAG) systems
    2. Capacity to translate text in over 20 languages
    3. Support for tokenizing longer sentences
    4. Emphasis on syntactic clustering of word embeddings<br><br>
11. What is the purpose ofthe "stop sequence" parameter in the OCI Generative AI Generation models?
    1. It controls the randomness ofthe model's output, affecting its creativity.
    2. It specifies a string that tells the model to stop generating more content.
    3. It assigns a penalty to frequently occurring tokens to reduce repetitive text.
    4. It determines the maximum number of tokens the model can generate per response.<br><br>
12. What does a higher number assigned to a token signify in the "Show Likelihoods" feature ofthe language model token generation?
    1. The token is less likely to follow the current token.
    2. The token is more likely to follow the current token.
    3. The token is unrelated to the current token and Will not be used
    4. The token will be the only one considered in the next generation step.<br><br>
13. Given the following code: <br> Prompt Template <br> (imput_variables["human_input", "city"], template-template) <br> Which statement is true about Promt Template in relation to input_variables?
    1. Prompt Template requires a minimum of two variables to function properly
    2. Prompt Template can support only a single variable at time.
    3. Prompt Template supports any number of variables, including the possibility of having none.
    4. Prompt Template is unable to use any variables.<br><br>
14. Which is NOT a built-in memory type in LangChain?
    1. ConversationTokenBufferMemory
    2. Conversation ImageMemory
    3. ConversationBufferMemory
    4. Conversation SummaryMemory<br><br>
15. Given the following code: <br> chain = prompt | llm <br> Which statement is true about LangChain Expression Language (LCEL)?
    1. LCEL is a programming language used to write documentation for tangChain.
    2. LCEL is alegacy method for creatin chains in LangChain
    3. LCEL is a declarative and preferred way to compose chains together.<br><br>
16. Given a block of code: <br> qa = Conversational Retrieval Chain.from llm (llm, retriever-retv, memory-memory) <br> when does a chain typically interact with memory during execution?
    1. Continuously throughout the entire chain execution process
    2. Only after the output has been generated
    3. After user input but before chain execution, and again after core logic but before output
    4. Before user input and after chain execution<br><br>
17. Which is NOT a category of pretrained foundational models available in the OCI Generative AI service?
    1. Translation models
    2. Summarization models
    3. Generation models
    4. Embedding models<br><br>
18. How are fine-tuned customer models stored to enable strong data privacy and security in the OCI Generative AI service?
    1. Stored in Object Storage encrypted by default
    2. Shared among multiple customers for eficiency
    3. Stored in Key Management service
    4. Stored in an unencrypted form in Object Storage<br><br>
19. Why is normalization of vectors important before indexing in a hybrid search system?
    1. It converts all sparse vectors to dense vectors.
    2. It significantly reduces the size of the database.
    3. It standardizes vector lengths for meaningful comparison using metrics such as Cosine Similarity.
    4. It ensures that all vectors represent keywords only.<br><br>
20. How does the architecture of dedicated AI clusters contribute to minimizing GPU memory overhead for T-Few fine-tuned model inference?
    1. By sharing base model weights across multiple fine-tuned models on the same group of GPUs
    2. By optimizing GPU memory utilization for each model's unique parameters
    3. By allocating separate GPUs for each model instance
    4. By loading the entire model into GPU memory for eficient processing<br><br>

## Respuestas

1. `mmr`
2. `It enables the deployment of multiple fine-tuned models within a single cluster`
3. `Servers as a designated point for user requests and model responses`
4. `PEFT involves only a few or new parameters and uses labeled, task-specific data.`
5. `RAG Token retrieves relevant documents for each part of the response and constructs the answer incrementally.`
6. `Ranker`
7. `Top k selects the next token based on its position in the list of probable tokens, whereas "Top p" selects based on the cumulative probability of the top tokens.`
8. `Top p limits token selection based on the sum of their probabilities.`
9. `Controls the randomness of the model's output, affecting its creativity`
10. `Improved retrievals for Retrieval-Augmented Generation (RAG) systems`
11. `It specifies a string that tells the model to stop generating more content.`
12. `The token is more likely to follow the current token.`
13. `Prompt Template supports any number of variables, including the possibility of having none.`
14. `Conversation ImageMemory`
15. `LCEL is a declarative and preferred way to compose chains together.`
16. `After user input but before chain execution, and again after core logic but before output`
17. `Translation models`
18. `Stored in Object Storage encrypted by default`
19. `It standardizes vector lengths for meaningful comparison using metrics such as Cosine Similarity.`
20. `By sharing base model weights across multiple fine-tuned models on the same group of GPUs`