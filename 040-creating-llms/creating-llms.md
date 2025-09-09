
# Creating LLMs

Large Language Models (LLMs) are created through a multi-step process starting with gathering massive amounts of text data from books, websites, and other sources. This data is used to train a deep neural network, typically based on the Transformer architecture, which learns to predict and generate text by recognizing patterns and relationships within the data. 

LLMs are built through a multi-stage process, consisting of pre-training, fine-tuning, and reinforcement learning.



## Pre-Training

The model learns language patterns by predicting missing or next words in massive text datasets without explicit instructions. While this helps it develop a general understanding of language structure and context, this is not what is expected by end users.

For example, if using a pre-trained model, if the user prompts the model with:

```
Explain the theory of relativity.
```


... the model may output the following unfiltered next-token prediction:

```
Explain the theory of relativity. This topic often comes up in physics discussion boards. One contributor, afficio92, explained: "Gravity isn’t really a force in the traditional sense—it’s the bending of spacetime itself. Massive bodies distort that cosmic fabric, and we experience that distortion as gravity." Another participant, UniverseFan2000, added an important note: "And remember, near a black hole, time itself runs slower because of this effect!"
```

As you can see, the base pre-trained model sees the prompt `Explain the theory of relativity.` as the beginning of a document. It will continue the text in a way that might look like it's answering, but it's actually just mimicking patterns it has seen online. The result is often unstructured and unpredictable. To specialize this base model for specific tasks, such as instruction following, we need to fine-tune the model.



## Fine-Tuning

After pre-training, *fine-tuning* (or *supervised fine-tuning*) customizes the model to specific tasks or domains using smaller labeled datasets, improving accuracy and relevance. These smaller datasets may consist for example, of high-quality, curated Q&A (question & answers) pairs, carefully selected code snippets, and similar.



## Reinforcement Learning (RL)

Finally, RL with human feedback aligns the model’s behavior with human preferences, enhancing its ability to generate useful and safe responses.


