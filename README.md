# 100DaysofAIbyCTOAdvisor
#100DaysOfAI By CTO Advisor (aka  Keith Townsend)

I’m going to start #100DaysOfAI inspired by all of the folks doing #100DaysOfCode.


## Day 01 of #100DaysOfAI: Foundational Models
https://x.com/CTOAdvisor/status/1802764900986761554

Day 1 is about the foundation, so we’ll start with the foundation: Foundational Models.

On Day 1 of my 100 days of AI, I’ll focus on the concept of Foundational Models. A foundational model is any large model trained on a vast and diverse dataset using self-supervised learning techniques. These models serve as a base for various downstream tasks and are characterized by their transfer learning capabilities. Transfer learning means that once a model has been trained on a large dataset, it can be fine-tuned for specific tasks with much smaller datasets, leveraging the knowledge it has already gained.

In the days of generative AI, we hear a lot about large language models (LLM). A large language model is a type of foundational model trained on— you guessed it— a large language dataset. These models are pre-trained on extensive text data and can generate or understand human language with high proficiency.

Vision Models are another type of foundational model. Think of Amazon’s original hot dog/not hot dog vision demo from re:Invent a few years ago. These models are pre-trained on large image datasets and can be used for various tasks such as classification, detection, and segmentation.

You’ve seen OpenAI combine vision modeling with their LLM to deliver multi-modal AI, which can process and understand both text and images simultaneously.

There are other types of foundational models, such as Tabular Data Models and Time Series Models. You can start a journey of learning via this Microsoft Azure product announcement blog with the link below:

[Microsoft Azure Product Announcement Blog](https://techcommunity.microsoft.com/t5/ai-machine-learning-blog/announcing-foundation-models-in-azure-machine-learning/ba-p/3827481)

It’s very important to understand the various model types, as it will help you determine which models are best for the types of data you want to infer.

What foundational topic of AI would you like me to overview in the coming weeks?

https://x.com/CTOAdvisor/status/1802777215215747358

## Day 02 of #100DaysOfAI: Talking Parameters.
https://x.com/CTOAdvisor/status/1803215573683413494

When context isn't clear, weights and biases in the neural network help determine meaning. Weights prioritize certain words, while biases adjust overall tendencies, enabling the model to make educated guesses based on learned patterns from extensive training data. For instance, if the phrase is "I love Chrome," the model uses weights to consider surrounding words and biases to lean towards common uses, deciding if "Chrome" refers to the web browser or car wheels based on subtle clues.

Advantages of More Parameters:
- Better Accuracy: More parameters allow the model to learn more complex patterns and nuances, improving its ability to make accurate predictions.
- Flexibility: Larger models can handle a wider range of tasks and adapt to different types of data more effectively.

Disadvantages of More Parameters:
- Computational Resources: Training and running models with many parameters require significant computational power and memory, making them expensive to deploy. This is why GPU’s are so important. More GPUs=More Tokens per unit of time. What’s a token? We’ll talk about it tomorrow. 
- Overfitting: With too many parameters, the model might learn noise in the training data rather than general patterns, reducing its ability to perform well on new, unseen data. This is potential source for hallucination. Which is better a 3B parameter model for your support data set or a 1T parameter model? 

Balancing the number of parameters is crucial for achieving high performance while managing resource constraints and maintaining generalization capability.

https://x.com/CTOAdvisor/status/1803177295693357455

## Day 03 of #100DaysOfAI: Tokens

https://x.com/CTOAdvisor/status/1803471105975280019

A token is a piece of data that AI models use to do their thing. The most common example is text. When we talk about text, a token is like a chunk of a word or even a whole word, depending on how it's broken down. Usually, people say a token is about 3/4 of a word. So, for example, the sentence "OpenAI develops advanced AI models" could be split into tokens like "Open", "AI", "develops", "advanced", "AI", "models."

Once text is turned into tokens, AI models can start spotting patterns. By adding parameters to the model, data scientists set up weights and biases to help the model understand the context better. Parameters are the bits that the model learns from the data during training. They allow the model to generalize from specific examples to a broader understanding.

There's a direct link between the model algorithm, the number of parameters, and the data type on how many tokens a particular compute setup can handle. More complex models with more parameters can process tokens more effectively but need more computational power.

Understanding how tokens, models, and compute power work together is critical to optimizing AI systems and getting the best performance for different tasks.
## Day 4 of #100DaysOfAI: Considerations for Selecting a Model
https://x.com/CTOAdvisor/status/1803852178370760712

When choosing an AI model, thinking that bigger is always better is tempting. Larger models, like LLaMA 70B, offer significant advantages in reducing hallucinations. However, it's crucial to consider several practical counterarguments:

Comparable Knowledge Compression
Both 70B and 7B models compress vast amounts of data into a few gigabytes. While a larger model has more parameters to interpret this data, the fundamental challenge of data compression and potential information loss remains. Thus, the risk of hallucination, although reduced, is not entirely eliminated in larger models.

Practical Considerations in Application
Integrating open-source models into practical applications requires careful dataset curation and management to minimize hallucinations. Limiting the dataset to your specific knowledge base and expected answers is crucial for ensuring relevant and accurate responses.

Balancing Size and Efficiency
A 70B model might offer improved accuracy and reduced hallucinations, but it also demands significantly more computational resources. For many applications, especially those with limited infrastructure, a 7B model might be more practical. Efficient fine-tuning and dataset management can mitigate hallucination risks without the overhead of a larger model.

Focusing on Customization
Over the next few days, we'll explore practical strategies for customizing models to your needs. This includes fine-tuning models, regardless of size, to ensure they generate accurate and reliable outputs. By tailoring the model to your knowledge base, you can effectively address the hallucination challenge without relying solely on model size.

In summary, while larger models have clear advantages, practical application and efficient customization are crucial to managing hallucination in any AI model. Stay tuned as we begin to get hands-on keyboard in a few days.
