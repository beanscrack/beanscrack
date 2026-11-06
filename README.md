### Software Engineer | Systems, GPU Computing & ML Infrastructure

Computer Science at the **University of Waterloo**. I build low-level systems in **C++, CUDA, Rust, and Go**, with a focus on performance, memory efficiency, and correctness.

[LinkedIn](https://www.linkedin.com/in/jerry-wu-03210a30b/) · [Email](mailto:sumsjerrywu@gmail.com)

## Featured Projects

### [Native LLM Inference Engine](https://github.com/beanscrack/LLM-Inference-C-CUDA-) — C++ / CUDA
Built a custom inference runtime for a **27B-parameter Qwen model on 16 GB VRAM**, implementing NVFP4/FP8 kernels, Gated-DeltaNet, attention, and asynchronous CPU-to-GPU weight streaming. Validated numerical correctness against a NumPy reference.

### Swift FlashNext Optimization — CUDA / Triton / vLLM
Optimized 27B LLM inference on NVIDIA Blackwell, improving single-request decoding throughput from **195 to 256 tokens/s (+31%)** through speculative decoding, CUDA graphs, optimized GEMMs, and L2 prefetching.


### RDec — Rust / Compilers
Building an **x86-64 to C decompiler** from scratch, featuring an intermediate representation, instruction lifting, control-flow analysis, and translation validation. Verified x86 flag semantics through **9.7 billion hardware comparisons** without mismatches.


### Swarm — Rust / AI Infrastructure
Built a multi-agent runtime with concurrent task scheduling, provider abstractions, persistent execution state, tool orchestration, and MCP integration.


### Coalign — Go / Distributed Systems
Developing a coordination platform enabling coding agents to exchange authorized context, negotiate changes, and produce evidence-backed proposals through authenticated APIs, durable storage, background workers, and isolated execution.

*Repository currently private.*

## Open Source

- **[LLVM](https://github.com/llvm/llvm-project/pull/235209)** — contributed a proposed TailCallElim correctness fix with regression tests (PR open).
- **[Haven-HV](https://github.com/1KingOfCurses1/Haven-HV/pulls?q=is%3Apr+author%3Abeanscrack+is%3Amerged)** and **[SkinSight](https://github.com/Anasthecode/SkinSight/pulls?q=is%3Apr+author%3Abeanscrack+is%3Amerged)** — 7 merged PRs across AI infrastructure, ML, and application development.

---

Interested in **inference engineering, compilers, systems programming, and high-performance computing**.
