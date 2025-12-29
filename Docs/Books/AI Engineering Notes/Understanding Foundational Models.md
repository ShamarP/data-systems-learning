
## What this chapter is about
In this chapter we go over the entire workflow of building foundational models. From how training data is acquired and used. Then it discusses how the models are built and what architectures are commonly used to build foundational models. After training the models there is a post training step that "validates" the output from the pre-trained model. This step is key for ensuring that the models output is safe for user consumption. It then finishes off with discussing the probabilistic nature of Foundational models and how this leads to hallucinations and how this affects AI products.

## Key Concepts
- [[Foundational Models]]

## My Explanation
This chapter introduces how foundational models are trained, model architecture and size, post training and sampling.

Training foundational models is challenging because high-quality, curated data is expensive to obtain at scale. As a result, training data is often scraped from the internet, where quality and reliability are not guaranteed. This can introduce factual errors, social and cultural biases, and harmful content into the training set, which may then be reflected in the model’s outputs. In addition, internet-scraped data does not represent all groups equally. Content associated with certain languages, cultures, regions, or communities may be underrepresented or absent altogether, causing foundational models to perform unevenly across populations and perspectives.

In addition to data, model architecture and scale play a critical role in the effectiveness of foundational models. Architectural choices determine how efficiently a model can represent complex patterns, capture long-range dependencies, and generalize across tasks. Increasing model size has shown to improve performance but, this leads to increased compute costs.

Because foundational models are trained on large, imperfect datasets, post-training fine-tuning is necessary to correct undesirable behaviors learned during pretraining. Through techniques such as supervised fine-tuning and alignment methods, models can be made safer, more reliable, and better aligned with human expectations.

Sampling can determine how your model generates responses for your application.  One such method is sampling with temperature this essentially increases the probability of seeing rarer tokens. Which gives your model more creative responses. 

In many applications you will need the llm to generate structured outputs. Such tasks include turning natural language to sql or tasks that send output to downstream systems. AI can be used to validate such outputs to determine if they're valid or you can post process for commonly found mistakes such as syntax issues. This also leads to fine-tuning where you can fine-tune a model to get the desired results for these tasks.
## Misunderstandings I corrected
The heavy ML aspect of this chapter when discussing model architecture and size

## Open Questions
(Things to revisit later)

## Related Notes

