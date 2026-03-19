# 🚀 Awesome LLM Physics Benchmarks

[![Stargazers](https://img.shields.io/github/stars/SpiritsYouthHarmony/awesome-llm-physics-benchmarks?style=social)](https://github.com/SpiritsYouthHarmony/awesome-llm-physics-benchmarks/stargazers)
[![Last Commit](https://img.shields.io/github/last-commit/SpiritsYouthHarmony/awesome-llm-physics-benchmarks)](https://github.com/SpiritsYouthHarmony/awesome-llm-physics-benchmarks/commits/main)

A curated and comprehensive list of benchmarks for evaluating Large Language Models (LLMs) and Multimodal LLMs (MLLMs/VLMs) on **physics reasoning, problem-solving, and physical world understanding**. This list covers everything from text-only university problems and vision-grounded diagrams to video dynamics, research-level challenges, and specialized subfields like quantum and condensed matter physics.

The goal is to provide a one-stop resource for researchers and developers to track progress and select appropriate benchmarks for evaluating models across a spectrum of capabilities: Knowledge Recall → Symbolic Derivation → Multi-step Reasoning → Diagram Grounding → Quantitative Verification → Frontier Research.

Inspired by [Awesome-AI-for-Physics](https://github.com/AI4Phys/Awesome-AI-for-Physics). Contributions are highly welcome! Please give a ⭐ if you find this useful!

## 📊 Leaderboards & Platforms

| Name | Description | Link |
|------|-------------|------|
| [PhyArena](https://phyarena.github.io/) | Open leaderboard for physics reasoning in LLMs/MLLMs (Olympiads + mixed difficulty). | [Official Site](https://phyarena.github.io/) |
| [Open LLM Leaderboard](https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard) | Hugging Face's general LLM leaderboard, includes physics subsets like GPQA and SciBench. | [Hugging Face](https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard) |
| [VLLM Leaderboard](https://leaderboard.vllm.ai/) | MLLM leaderboard that often includes physics benchmarks like SeePhys and PHYBench. | [Official Site](https://leaderboard.vllm.ai/) |

## 🏷️ Benchmarks by Category

### 1. Text-Only Physics Problem-Solving (University/Olympiad)
*Focus: High-school to PhD-level problems requiring derivations and multi-step reasoning without visual input.*

| Benchmark | Scale/Difficulty | Key Features | Links |
|-----------|------------------|--------------|-------|
| [PHYSICS](https://github.com/allenai/PhysicsQA) | 1,297 university problems | Covers 6 core areas (mechanics, EM, quantum, etc.), with an automated evaluation system. | [GitHub](https://github.com/allenai/PhysicsQA) &#124; [Paper](https://arxiv.org/abs/2405.12771) |
| [UGPhysics](https://github.com/YangLabHKUST/UGPhysics) | 5,520 undergrad problems | 13 subjects, English/Chinese, Model-Assistant Rule-based Judgment (MARJ), 7 answer types. | [GitHub](https://github.com/YangLabHKUST/UGPhysics) &#124; [arXiv](https://arxiv.org/abs/2502.00334) |
| [PhyArena (HiPhO & Mixed)](https://phyarena.github.io/) | Mixed (HS-PhD), Olympiads | Compares model scores against human medal cutoffs. | [Official Site](https://phyarena.github.io/) |
| [GPQA (Physics subset)](https://github.com/togethercomputer/GPQA) | 448+198 PhD-level MCQs | "Google-proof" questions designed by experts. Physics is a subset. | [GitHub](https://github.com/togethercomputer/GPQA) &#124; [Hugging Face](https://huggingface.co/datasets/togethercomputer/gpqa) |
| [SciBench (Physics)](https://github.com/TIGER-AI-Lab/SciBench) | Collegiate-level science | Physics is a subset, some problems have visual contexts. | [GitHub](https://github.com/TIGER-AI-Lab/SciBench) |
| [OlympiadBench (Physics)](https://github.com/centerforaisafety/OlympiadBench) | Olympiad-level STEM | Physics is ~25% of the dataset. Open-ended and bilingual (English/Chinese). | [GitHub](https://github.com/centerforaisafety/OlympiadBench) |

### 2. Multimodal (Image/Diagram-Grounded) Physics Reasoning
*Focus: Problems where diagrams (circuits, force diagrams, optics) are essential for understanding and solving.*

| Benchmark | Scale | Key Features | Links |
|-----------|--------|--------------|-------|
| [SeePhys](https://github.com/AI4Phys/SeePhys) | ~2,000 (MS-PhD) | High ratio of "vision-essential" problems to prevent text-only shortcuts. | [GitHub](https://github.com/AI4Phys/SeePhys) &#124; [arXiv](https://arxiv.org/abs/2505.19099) |
| [PhysReason](https://github.com/dxzxy12138/PhysReason) | 1,200 multi-domain | Evaluates theorem/step recall; 75% of problems require reasoning. | [GitHub](https://github.com/dxzxy12138/PhysReason) &#124; [Site](https://dxzxy12138.github.io/PhysReason/) |
| [PhysicsArena (Multimodal)](https://phyarena.github.io/) | N/A | Diagnostic 3-stage evaluation: Variable ID → Process Modeling → Solution. | [Official Site](https://phyarena.github.io/) |
| [PhysUniBench](https://github.com/PrismaX-Team/PhysUniBenchmark) | 3,304 undergrad problems | Focus on undergraduate-level multimodal reasoning with open-ended answers. | [GitHub](https://github.com/PrismaX-Team/PhysUniBenchmark) &#124; [OpenReview](https://openreview.net/pdf?id=TqgPgCvBnF) |
| [PhyX](https://github.com/killthefullmoon/PhyX) | 3,000 visual problems | Covers 6 reasoning types and 25 subdomains. | [GitHub](https://github.com/killthefullmoon/PhyX) &#124; [Site](https://phyx-bench.github.io/) |
| [PHYBench](https://github.com/phybench-official/phybench) | 500+ problems | Focus on physical perception and robust reasoning across 5 domains. | [GitHub](https://github.com/phybench-official/phybench) &#124; [Site](https://phybench-official.github.io/phybench-demo) |
| [PhysBench (VLM World)](https://github.com/USC-GVL/PhysBench) | 10k+ entries (19 tasks) | Evaluates physical world understanding (properties, relations, events), not exam-solving. | [GitHub](https://github.com/USC-GVL/PhysBench) &#124; [Site](https://physbench.github.io/) |

### 3. Video/Dynamic Physics (Temporal Reasoning)
*Focus: Understanding motion, causality, and quantitative physics from video inputs.*

| Benchmark | Scale | Key Features | Links |
|-----------|--------|--------------|-------|
| [PhysGame](https://github.com/PhysGame/PhysGame) | 880 videos | Identifies physics commonsense violations ("glitches") in gameplay videos. | [GitHub](https://github.com/PhysGame/PhysGame) |
| [QuantiPhy](https://arxiv.org/abs/2402.14932) | 3,300+ video-text pairs | Strong focus on numerical precision in quantitative physics questions. | [arXiv](https://arxiv.org/abs/2402.14932) (Repo TBA) |
| [Physics-IQ](https://github.com/google-deepmind/physics-IQ-benchmark) | N/A | A benchmark for generative video models to test intuitive physics understanding. | [GitHub](https://github.com/google-deepmind/physics-IQ-benchmark) |

### 4. Research-Level & Subfield-Specific
*Focus: Frontier physics problems that are non-textbook, designed to resist memorization, and dive deep into specific domains.*

| Benchmark | Focus | Key Features | Links |
|-----------|--------|--------------|-------|
| [CritPt](https://github.com/CritPt-Benchmark/CritPt) | 71 research challenges | Designed by 50+ physicists; requires structured outputs (arrays, symbols, Python functions). | [GitHub](https://github.com/CritPt-Benchmark/CritPt) |
| [TPBench](https://tpbench.org/) | Theoretical Physics (HEP/Cosmo) | Problems sourced from non-public materials to reduce data contamination. | [Official Site](https://tpbench.org/) |
| [CMPhysBench](https://github.com/CMPhysBench/CMPhysBench) | Condensed Matter Physics | 520 graduate-level calculations; uses SEED (expression tree distance) for scoring. | [GitHub](https://github.com/CMPhysBench/CMPhysBench) |
| [QuantumBench](https://huggingface.co/datasets/QuantumBench) | Quantum Computing | Systematically evaluates LLMs on quantum domain knowledge and application. | [Hugging Face](https://huggingface.co/datasets/QuantumBench) &#124; [arXiv](https://arxiv.org/abs/2308.01398) |
| [SPhyR](https://arxiv.org/abs/2402.14932) | Topology/Structural Optimization | Tests spatial and physical reasoning in an engineering context. | [arXiv](https://arxiv.org/abs/2402.14932) (Repo TBA) |

## 🛠️ Evaluation Tools & Frameworks

- [**EleutherAI/lm-evaluation-harness**](https://github.com/EleutherAI/lm-evaluation-harness): The standard for text-based LLM evaluation. Supports benchmarks like GPQA and SciBench out of the box.
- [**OpenCompass/opencompass**](https://github.com/open-compass/opencompass): A comprehensive evaluation suite for both LLMs and MLLMs, supporting many science benchmarks.
- [**AI4Phys/SeePhys Eval**](https://github.com/AI4Phys/SeePhys): Official evaluation code for the SeePhys benchmark.

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingBenchmark`)
3.  Commit your Changes (`git commit -m 'Add some AmazingBenchmark'`)
4.  Push to the Branch (`git push origin feature/AmazingBenchmark`)
5.  Open a Pull Request

Please ensure your submission is a well-established benchmark with a corresponding paper or public dataset.

## 📜 License

This project is licensed under the [CC0-1.0 Universal](LICENSE) License.
