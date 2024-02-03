# About the Project

Through this project, I use AI to address a pressing issue in healthcare: manually reviewing lengthy medical transcripts to extract important information quickly. The ultimate goal is to create AI-powered agents that can quickly and accurately analyze these transcripts, extract relevant clinical information, and present it in an user-friendly format for healthcare professionals. 

By streamlining this process, AI can help improve operational efficiency, enhance diagnostic accuracy, and accelerate the processing of information in healthcare. This project specifically focuses on developing AI agents skilled at extracting specific clinical information from medical transcripts, ultimately contributing to a more efficient and technologically advanced healthcare system.

# Dataset
The input data for the here is typically medical transcripts or summaries, which provide an overview of a patient's medical records.  
  
  To test the model, I used a dataset from the Medical Transcriptions dataset on KAGGLE. This dataset includes a wide range of medical transcription data from mtsamples.com, which was used to train and evaluate the project's performance.  
  
To analyze and process the data, the dataset needs to be formatted and provided to the project as a text file. This ensures that the project can effectively understand and gain insights from the medical transcript data during the analysis and interaction processes.

# Architecture
The project implemented used this architecture: <a href="https://imgbb.com/"><img src="https://i.ibb.co/tHJ9TLj/Picture1.png" alt="Picture1" border="0"> </a>
Figure 1
-   **User Prompt**: This is where the user asks a question or gives a command.
-   **Action Agent**: This agent takes the user’s input, figures out what they want, and decides what it should do.
-   **Chain of Thoughts**: This is the bot's thought process. It understands the user’s input, finds the important information, and figures out the best response.
-   **LLM**: This is the AI model that can understand and generate human language. For this project, I’m using Google’s flan-t5 model.
-   **Tool**: This is any extra resources or functions it uses.  Here it’s used to call the Langchain API powered by Huggingface Embeddings.
-   **Retrieve from Vector Store**: This is how the model gets the final response or information from my memory bank, the Vector Store.
-   **Final Answer Agent**: After it's figured out the best response, this agent gets that response from the Vector Store.

# Results
<a href="https://ibb.co/Vq7tWjM"><img src="https://i.ibb.co/rwCmG75/Screenshot-2024-02-03-212427.png" alt="Screenshot-2024-02-03-212427" border="0"></a>
<a href="https://ibb.co/yWJp8zJ"><img src="https://i.ibb.co/pJpQ3Hp/Screenshot-2024-02-03-212440.png" alt="Screenshot-2024-02-03-212440" border="0"></a>
<a href="https://ibb.co/6FqW7N6"><img src="https://i.ibb.co/bXGKM7p/Screenshot-2024-02-03-212415.png" alt="Screenshot-2024-02-03-212415" border="0"></a>

Here’s a semi-formal version of your model’s performance for a GitHub repo:

-   The coherence score of my model was off the charts at **0.99999999999**, showing that it can generate sentences that logically connect to each other almost flawlessly.
-   When it comes to text summarization, my model nailed it with perfect precision scores of **1.0** in ROUGE-1, ROUGE-2, and ROUGE-L metrics, meaning it matched the reference summaries exactly.
-   The F1 scores for ROUGE-1, ROUGE-2, and ROUGE-L were a bit lower, showing there’s still some room for improvement.
-   My model scored a **40.161** in perplexity, which is pretty good! It shows that my model can predict words in context quite effectively.
-   The LSA-based topic coherence score of my model was a solid **0.767**, showing that it’s pretty good at generating topics that are logically connected and relevant.
-   My model scored a **0.523** on the ESIM (Enhanced Sequential Inference Model), which means it’s doing a good job at generating text that’s semantically similar to the reference text.
-   The Cohesion Score of my model was **0.52337074**, suggesting that the text it generates has a decent level of unity. But, like any good model, there’s always room for improvement!
- The model was well-received in human evaluations, showing its potential for various applications. The evaluators were happy with the summaries it produced, which closely matched the reference summaries. This indicates that the model is ready for use in different areas. Its ability to align with human evaluators highlights its usefulness in speeding up information retrieval, improving understanding, and aiding decision-making in various contexts, demonstrating its real-world value.

# Conclusions
This model is pretty good at analyzing medical transcripts and having meaningful conversations. It’s skilled at pulling out the right info from large datasets and understanding the context. It uses advanced techniques to go through medical records, and it can understand complex terms. It’s also good at connecting queries to give more insightful responses. This model is a big leap in using AI for medical data and can really help in interpreting medical info and making informed decisions in healthcare.

# Contributions
If you have ideas for improvement or wish to contribute, please open an issue or submit a pull request. Collaboration is highly encouraged!
