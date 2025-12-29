## What this concept means 
A foundation model is a large, pre-trained model trained on broad data at scale that learns general representations and can be adapted (fine-tuned or prompted) to perform many downstream tasks.

## Why this concept matters
Foundational models are important because they dramatically lower the barrier to building AI applications. By training large, general-purpose models on massive and diverse datasets, companies create models that can be reused across many tasks without requiring users to collect data or train models themselves. This allows organizations without the resources or knowledge to train these models to build powerful AI systems.

## Core ideas
- Training data used to train these models. [Common Crawl](https://commoncrawl.org/)
- The model size and architecture used.
- Post training how these models are adapted for specific use cases.

## Simple example

**Foundation model:** a pre-trained large language model (LLM)

**How it’s used:**

- A company wants a chatbot to answer customer questions.
    
- Instead of training a model from scratch, they use a pretrained foundation model.
    
- They provide:
    
    - A short system prompt (“You are a customer support agent for an online store”)
        
    - Optionally a small set of FAQs or past conversations.
        
- The same model can now:
    
    - Answer questions
        
    - Summarize complaints
        
    - Draft responses
        
    - Escalate issues when needed
        

**Why this works:**

- The foundation model already understands language, tone, and common question patterns.
    
- The company only adapts it via prompting or light fine-tuning—no massive dataset or training infrastructure required.

## Real-world systems that use this
- ChatGPT → Uses foundational models to act as a personalized assistant for users
- Github Copilot → Uses foundational models to be used as a coding assistant.
- Google → Uses foundational models to summarize search results

## Tradeoffs / limitations

- Foundational models are trained on massive, heterogeneous datasets, often scraped from the public internet. As a result, **prior to post-training and alignment**, these models may reproduce **biases, stereotypes, or harmful language** present in the training data, making them **unsafe for direct human-facing deployment**.
- These models are generalized so depending on the use case you may not get the results needed. This leads to having to fine-tune the model for said use case.
- Foundational models are not deterministic so this leads to it being difficult to test/validate things.

## Related concepts
- [[Reliability]] : not directly related but the idea that AI applications need to be reliable applies. 

## Misunderstandings I corrected
- A lot of the Model specific terminology was new to me. So I spent sometime understanding the definitions in [[Glossary]]

## Questions I still have
[[Recurrent Neural Network (RNN)]]
