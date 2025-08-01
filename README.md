# llm-medmcqa

## Purpose and Goal
Test how lightweight LLM models preform with medical multiple choice questions and see if we can improve the results by adding context with RAG. Current top LLM models are expensive to run. If successful, this will show that even light weight and cheaper models can have valuable application in the healthcare domain.

## Approach
- Filter from [this](https://huggingface.co/datasets/openlifescienceai/medmcqa) dataset to get just the anesthesia questions
- Use Gemini Flash model to see preformance of base model
- Implement a simple RAG with anesthesia context
- We will use [chroma db](https://www.trychroma.com/) for the rag database and [sbert](https://www.sbert.net/) for the sentence transformer
- Use the same Gemini Flash model to see preformance with the RAG running
- Compare and analyse results
