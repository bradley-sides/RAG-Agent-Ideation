# RAG-Agent-Ideation
Steps:

  1. Author inputs their 3(?) most recent papers.

  2. Related works are located using RAG with sentence embeddings.

  3. With special consideration placed on the author's own papers, augmented with background context from the related works in addition to the model's own knowledge, generate a "baseline" research idea for the     
     author.

  4. Utilize harsh reviewing agents to assess the idea based on multiple criteria.

    a. Novelty agent checks that the idea is sufficiently different from already researched topics. Provides detailed feedback as well as a score.

    b. Fundability/Impact agent checks that the idea is both competitive for grants and focused on an important topic rather than simply something obscure. Provdes detailed feedback as well as a score.

  5. If score minimums are not met, return to idea generating agent with feedback from both reviewing agents to improve upon the idea, iterate until passing.

  6. Once score minimums are met, the idea is finalized.

Models Used:

LLM: Llama 3 70B 8192

Sentence Encoder: sentence-transformers all-MiniLM-L6-v2

Tokenizer: GPT2

