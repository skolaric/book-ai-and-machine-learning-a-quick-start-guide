
# LLM Agents

Large Language Models (LLMs) are currently the most prominent AI modules being used. An LLM is a type of artificial intelligence program that uses deep learning techniques to understand, generate, and predict human language. 

An LLM is trained on massive amounts of text data, allowing it to perform various natural language processing tasks such as answering questions, writing text, and translating languages. 

LLMs are built using neural networks called *transformers*, which enable them to capture context and complex relationships in language efficiently. Examples include GPT and Claude.

In this chapter, we focus on high-level aspects of LLMs, such as characteristics of LLM, how to deploy and use LLMs, and so on. For low-level technical details of LLMs, we refer the reader to existing texts such as [][][][].


## The Inner Architecture of LLMs

What is the inner makeup of LLMs? Large Language Models (LLMs) are built primarily on the **Transformer architecture**, which is a deep neural network designed to process sequences of text in parallel. The key components of this architecture include:

- **Input Embeddings:** Tokens (words or subwords) are converted into continuous vector representations that capture semantic meaning.
- **Positional Encoding:** Since transformers do not inherently understand word order, positional encodings are added to embeddings to provide the sequence context.
- **Self-Attention Mechanism:** This allows the model to weigh the influence of all tokens in the input sequence relative to each other, capturing long-range dependencies and contextual relationships.
- **Feedforward Neural Networks:** After attention, fully connected layers apply nonlinear transformations to interpret and refine the information.
- **Multi-Head Attention:** Multiple attention layers run in parallel, enabling the model to focus on different aspects of the input simultaneously.
- **Layer Normalization:** This stabilizes training and improves convergence by normalizing intermediate outputs.
- **Output Layers:** Finally, the model predicts the next token or generates text based on learned patterns.

Together, these components enable LLMs to understand, generate, and predict language effectively across many applications.
