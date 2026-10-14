A rapid-fire ML knowledge round covering a broad range of topics expected of a Senior MLE. The interviewer tests foundational understanding across classical ML, deep learning architectures, and modern LLM-era concepts.

Topics include:

1. Traditional ML (e.g., decision trees, SVMs, ensemble methods, bias-variance tradeoff)
2. Evaluation metrics (precision, recall, F1, AUC-ROC, calibration)
3. Transformer architecture (self-attention, multi-head attention, causal masking, what is inside one transformer block, positional encoding, layer norm)
4. LLM Agents (tool use, planning, memory)
5. MCP (Model Context Protocol — Anthropic's protocol for connecting LLMs to external tools/data)
6. Prompt engineering (few-shot, chain-of-thought, system prompts)
7. Knowledge distillation (teacher-student, soft labels, temperature scaling)
8. Activation functions (ReLU, GELU, Sigmoid, tanh, SwiGLU, dying ReLU problem)

### Constraints

- Expect 15-20 questions in 45 minutes
- Answers should be concise (1-3 minutes each)
- Senior-level depth expected — not just definitions but trade-offs and practical experience

### Examples

**Input:** Explain the transformer self-attention mechanism.

**Output:** Self-attention computes Q, K, V matrices from input embeddings. Attention weights = softmax(QK^T / sqrt(d_k)) * V. This allows each token to attend to all other tokens, capturing long-range dependencies. Multi-head attention runs this in parallel across h heads for richer representations.

**Explanation:** Should mention scaled dot-product, multi-head, and why sqrt(d_k) scaling is needed.

**Input:** What is knowledge distillation and when would you use it?

**Output:** Training a smaller student model to mimic a larger teacher model's soft probability outputs (using temperature-scaled softmax). Used when deploying to resource-constrained environments (mobile, edge) or reducing inference latency while preserving most of the teacher's performance.

**Explanation:** Mention soft labels, temperature parameter T, and KL-divergence loss.

A rapid-fire ML knowledge round covering a broad range of topics expected of a Senior MLE. The interviewer tests foundational understanding across classical ML, deep learning architectures, and modern LLM-era concepts.

Topics include:

1. Traditional ML (e.g., decision trees, SVMs, ensemble methods, bias-variance tradeoff)
2. Evaluation metrics (precision, recall, F1, AUC-ROC, calibration)
3. Transformer architecture (self-attention, multi-head attention, causal masking, what is inside one transformer block, positional encoding, layer norm)
4. LLM Agents (tool use, planning, memory)
5. MCP (Model Context Protocol — Anthropic's protocol for connecting LLMs to external tools/data)
6. Prompt engineering (few-shot, chain-of-thought, system prompts)
7. Knowledge distillation (teacher-student, soft labels, temperature scaling)
8. Activation functions (ReLU, GELU, Sigmoid, tanh, SwiGLU, dying ReLU problem)

### Constraints

- Expect 15-20 questions in 45 minutes
- Answers should be concise (1-3 minutes each)
- Senior-level depth expected — not just definitions but trade-offs and practical experience

### Examples

**Input:** Explain the transformer self-attention mechanism.

**Output:** Self-attention computes Q, K, V matrices from input embeddings. Attention weights = softmax(QK^T / sqrt(d_k)) * V. This allows each token to attend to all other tokens, capturing long-range dependencies. Multi-head attention runs this in parallel across h heads for richer representations.

**Explanation:** Should mention scaled dot-product, multi-head, and why sqrt(d_k) scaling is needed.

**Input:** What is knowledge distillation and when would you use it?

**Output:** Training a smaller student model to mimic a larger teacher model's soft probability outputs (using temperature-scaled softmax). Used when deploying to resource-constrained environments (mobile, edge) or reducing inference latency while preserving most of the teacher's performance.

**Explanation:** Mention soft labels, temperature parameter T, and KL-divergence loss.
