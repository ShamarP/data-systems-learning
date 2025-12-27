## What this chapter is about
This chapter gives a high level overview of the world of AI engineering. It goes through the rise of AI engineering starting from language models all the way to Foundation models. It then discusses the potential use cases for these models and how you build an AI application. 
## Key Concepts
- Foundation Models
- ML engineering vs AI engineerings
- Planning AI applications

## My Explanation
It discusses what foundation models are and how they came to be in modern day AI engineering. It begins with the idea of a language model and how it simply encodes statistical information about a language.  It can predict the next word in a sequence based on the language. It briefly discusses tokenization and the idea of how these models tokenize a prompt. With language models the output is open ended which means that it isn't a trivial problem to validate the output of said models. Language models are self-supervised meaning they don't require explicit labels for training data. What makes a model large is the number of parameters it has and this will constantly change as compute improves. Foundation models now expand the capabilities of language models and can take text, images, and videos as input. This expands the capabilities and opens a whole new world of possibilities.

AI engineering is now the process of building applications on top of these foundational models. Foundational models are general purpose and can be used for a variety of tasks. Most of the heavy lifting is done by the Foundational model providers (e.g OpenAI) there is a lower barrier to entry to producing AI native applications. 

AI engineering doesn't require the knowledge/background to build these applications from the ground up like the traditional ML engineering does. The main challenges that arise now that you don't need to train the model from ground up is how do you optimize inference and have more efficient training. You must also clearly define evaluation metrics for your AI application since output is open ended.

## Examples + Diagrams
```python
from openai import OpenAI

client = OpenAI()  # uses OPENAI_API_KEY from env

def summarize(text: str) -> str:
    response = client.responses.create(
        model="gpt-4.1-mini",
        input=f"Summarize this in one sentence:\n\n{text}"
    )

    return response.output_text


if __name__ == "__main__":
    text = """
    Artificial intelligence systems are increasingly being used
    in data engineering workflows to automate feature extraction,
    validation, and model deployment.
    """

    summary = summarize(text)
    print(summary)

```

very bare bones example of how we can use these foundation models to perform tasks in production.

## How this shows up in real systems
- Chat bots
- Workflow automation. Creating synthetic data
- Github copilot/ claude code / etc

## Misunderstandings I corrected
- Tokenization
- 

## Open Questions
(Things to revisit later)

## Related Notes
- [[Related concept]]
- [[Experiment note]]
