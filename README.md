# BRIDGE
RAG benchmark which enables a comprehensive evaluation of both retrieval and generation, while accurately revealing their alignment.
BRIDGE incorporates (1) answer validation data (query, gold answer, generated answer, answer validation) and (2) RAG dataset (query, gold chunk, gold answer).

Here is the description of BRIDGE dataset components.

q_id: query id
query: question in QA dataset
gold_answer: ground-truth answer for query
generated_answer: LLM generated answer with Top 10 retrieved chunks from 16 various retrieval methods
answer_validation: human evaluation label whether generated answer is correct or incorrect (1: correct, 0: incorrect)
gold_chunk: ground-truth chunk for query refined by our multi-step chunk label correction pipeline
