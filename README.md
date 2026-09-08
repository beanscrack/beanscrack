# Jerry Wu

### Software engineer. Interested in what happens underneath.

Computer Science at the **University of Waterloo**. I build systems in **C++ and CUDA**, apply machine learning to real problems, and make tools for building software.

The questions I come back to: Where does the memory go? What is the bottleneck? How do I know the result is right?

[LinkedIn](https://linkedin.com/in/jerry-wu) · [Email](mailto:sumsjerrywu@gmail.com)

## Start here

| Project | What I built | A useful place to look |
| :--- | :--- | :--- |
| **[Native LLM inference](https://github.com/beanscrack/LLM-Inference-C-CUDA-)** | A C++/CUDA runtime for Qwen with quantized weights, hybrid attention, and CPU-to-GPU weight streaming. | [Weight residency and prefetching](https://github.com/beanscrack/LLM-Inference-C-CUDA-/blob/main/src/qwen_weights.cpp) · [Numerical reference](https://github.com/beanscrack/LLM-Inference-C-CUDA-/blob/main/scripts/verify_forward.py) |
| **[TruthTone++](https://github.com/beanscrack/Truth-Tone)** | Audio deepfake detection with spectral analysis and a per-second confidence timeline. **Best Audio AI Hack, CxC 2026.** | [Watch the 36-hour hackathon build](https://www.youtube.com/watch?v=M-fwg9Zm7v8) · [Architecture and setup](https://github.com/beanscrack/Truth-Tone#technical-architecture) |
| **[Claude–Codex Duo](https://github.com/beanscrack/claude-codex-duo)** | An experiment in coordinating a read-only planner and a code-writing implementer through a local message board and shared workspace. | [How the loop works](https://github.com/beanscrack/claude-codex-duo#claude-codex-duo) |

## One engineering problem I’m working on

**Running a 27B model on a 16 GB GPU.**

My inference engine keeps part of the model in GPU memory and streams the remaining layers from pinned host memory. The work is in the details: packed weight formats, asynchronous copies, kernel behavior, and checking the output against a NumPy reference.

The next step is to measure how much transfer time prefetching actually hides, then improve the streamed decode path. The [engineering notes](https://github.com/beanscrack/LLM-Inference-C-CUDA-/blob/main/HANDOFF.md) include the measured results, numerical differences, and unfinished work.

## Smaller builds, foundational ideas

- **[Microheap](https://github.com/beanscrack/Microheap-A-Minimalist-Manual-Memory-Manager-in-C)** — a learning-focused C allocator with explicit chunk metadata, gap reuse, and memory-layout inspection.
- **[Generic merge sort in C](https://github.com/beanscrack/libmsort-Generic-Merge-Sort-Library-in-C)** — working with generic data and low-level memory operations.
- **[Risk-parity optimizer](https://github.com/beanscrack/Multi-Layer-Risk-Parity-Portfolio-Optimizer)** — a Python exploration of risk budgets and combining portfolio scenarios.

---

Open to software engineering opportunities and conversations about **systems, ML infrastructure, and developer tools**.
