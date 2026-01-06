# Evaluation Methodology

## What this chapter is about

This chapter goes over various metrics and methods used to evaluate foundational models. It discusses the challenges of evaluating these models such challenges arise due to how intelligent models are nowadays. It is easy to tell if a summary is bad because it can just be gibberish but very difficult to say if the summary is truly coherent and interpreting the material correctly. It then discusses various language model metrics such as entropy, cross entropy, bits-per-character and bits-per-byte, and perplexity. The final topic was surrounding using AI as a judge to evaluate these models and how this can be accomplished.


## Key Concepts
- [[Concepts/Concept A]]
- [[Concepts/Concept B]]
- [[Concepts/Concept C]]

## My Explanation

Evaluation methods are important as the more these models are used the more opportunity there is for failure. So being sure that they work as intended and provide value is an essential step of AI development. The question becomes how do you evaluate something that can produce anything as output. When thinking about simple use cases such as getting a summary on an article. There are many things that can go wrong such as hallucinating facts, not providing enough details and missing key information. Ensuring that your application is meeting the requirements of the users while also providing factually correct information is the major concerns of AI development.

## Evaluation metrics

- Entropy: How much information on average a token carries
- Cross Entropy: How difficult it is for the language model to predict what comes next.
- Perplexity: measures the amount of uncertainty the model has when predicting the next token

## AI as a Judge

Given the complexity of the responses produced by language models some workflows have resorted to using humans as judges. This process while it works great is costly and takes time. This has lead to the introduction of the idea of using AI as a judge. AI judges are fast and cheap compared to using humans as a judge. They can evaluate without needing reference data and given a criteria and correct model choice they cna produce sufficiently good results. Using AI as a judge introduces additional latency and costs which may not be feasible given the application. Given that language models are probabilisitic they are inconsistent and can produce conflicting answers. 



## Misunderstandings I corrected
Evaluation metrics

## Open Questions
I want to play around with using AI as a judge in a sandbox environment. Just to see how much a prompt may affect the scoring of a response. Also would like to see the differences between various models when judging.


## Related Notes

[[Foundational Models]]
