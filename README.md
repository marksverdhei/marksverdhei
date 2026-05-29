<h1 align="center">Markus Heiervang</h1>

<p align="center">
  <em>Teaching transformers to predict the next token.</em>
</p>

<p align="center">
  <a href="https://huggingface.co/marksverdhei"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-marksverdhei-yellow"></a>
  <a href="https://www.twitch.tv/hyperplane_t"><img src="https://img.shields.io/badge/Twitch-hyperplane__t-9146FF?logo=twitch&logoColor=white"></a>
  <a href="https://www.youtube.com/@marksverdhei"><img src="https://img.shields.io/badge/YouTube-marksverdhei-FF0000?logo=youtube&logoColor=white"></a>
  <img src="https://img.shields.io/badge/Location-Norway%20%F0%9F%87%B3%F0%9F%87%B4-blue">
</p>

---

### 👋 About

LLM engineer at the **[National Library of Norway](https://github.com/NationalLibraryOfNorway)**, where I help pretrain, post-train and evaluate Norwegian large language models. Off the clock I run **[Heiervang Technologies](https://github.com/heiervang-technologies)**, an open-source lab for AI agents, inference tooling, and forks of the libraries I use daily. MSc in Informatics (NLP) from the University of Oslo. I also stream the whole process on Twitch and YouTube.

My work spans the full model lifecycle: **data → training → quantization → serving → evaluation → agents**.

---

### 🌍 Open-source contributions

Getting brand-new models and fixes into the core ML stack:

- **GLM-4.7-Flash → vLLM**: Taught vLLM's MLA detection about `glm4_moe_lite` so the model runs on the engine · [vllm#32614](https://github.com/vllm-project/vllm/pull/32614)
- **Qwen3-TTS → vllm-omni**: Added speaker-embedding passthrough for the speech & voices APIs, a `speaker` alias, and a fix for the Qwen3-TTS-0.6B profile-run hang · [#1227](https://github.com/vllm-project/vllm-omni/pull/1227) · [#2424](https://github.com/vllm-project/vllm-omni/pull/2424) · [#1082](https://github.com/vllm-project/vllm-omni/pull/1082)
- **GPT-OSS MXFP4 quant → 🤗 transformers**: Fixed the MXFP4 quantizer to handle variable `num_local_experts`/`hidden_size`, so GPT-OSS models quantize correctly · [transformers#41795](https://github.com/huggingface/transformers/pull/41795)
- **OpenAI-compatible API eval → lm-evaluation-harness**: Fixed the assertion error that broke evaluation against OpenAI-compatible endpoints · [lm-eval#3356](https://github.com/EleutherAI/lm-evaluation-harness/pull/3356)

Plus smaller fixes to **[NVIDIA/Megatron-LM](https://github.com/NVIDIA/Megatron-LM/pull/1980)** (mcore example training loop), **[EuroEval](https://github.com/EuroEval/EuroEval/pull/865)** (fp16 loading for bf16 models on pre-Ampere GPUs), and **[ltgoslo/noreval](https://github.com/ltgoslo/noreval)**.

---

### 🎯 What I work on

I get **brand-new models running on open inference stacks**, then handle the lifecycle around them (quantize, serve, evaluate, and wrap in agents).

* 🚀 **Model enablement & inference:** Bringing new architectures (GLM-4.7, Qwen3-Omni/TTS, GPT-OSS) up in **vLLM**, **vllm-omni** & **🤗 transformers**.
* 🧮 **Quantization:** FP8, MXFP4 & GGUF to squeeze large models onto smaller and **non-NVIDIA GPUs** (Vulkan, ZLUDA).
* 🗣️ **Speech, voice & audio:** Speaker/voice embeddings, TTS, ASR, music generation.
* 🧠 **LLM training & fine-tuning:** Pre/post-training Norwegian LLMs, LoRA, prompt baking, synthetic data.
* 📊 **Evaluation & benchmarking:** EuroEval, lm-eval-harness, NorEval, MTEB.
* 🤖 **AI agents & dev tooling:** Agent orchestration, context compaction, CLI tools.

---

### 🚀 Featured projects

| Project | What it is | |
|---|---|---|
| **[sorting-hat](https://github.com/marksverdhei/sorting-hat)** | AI-powered file-naming CLI with animated ASCII art. Works with any OpenAI-compatible LLM. | ⭐ 16 |
| **[bakery](https://github.com/marksverdhei/bakery)** | Prompt baking & context distillation for LLMs. | ⭐ 5 |
| **[spritegrid](https://github.com/marksverdhei/spritegrid)** | Corrects AI-generated pixel art by applying grid sampling. | ⭐ 3 |
| **[chatfiles](https://github.com/marksverdhei/chatfiles)** | The dumbest *and* smartest way to make agents communicate. | ⭐ 2 |
| **[syntk](https://github.com/marksverdhei/syntk)** | Synthetic-data toolkit. | |
| **[semantic-sound-search](https://github.com/marksverdhei/semantic-sound-search)** | Semantic search over audio samples. | |
| **[autonomous-pokerogue](https://github.com/marksverdhei/autonomous-pokerogue)** | Turns PokéRogue into an idle clicker driven by vision-language models. | |
| **[localllama-with-vulkan](https://github.com/marksverdhei/localllama-with-vulkan)** | Run LLM inference on *any* GPU (tutorials & benchmarks). | |

---

### 🏢 Heiervang Technologies

Open-source software and hardened forks of the popular repos I run in production.

| Project | What it is | |
|---|---|---|
| **[am-i-openai-compatible](https://github.com/heiervang-technologies/am-i-openai-compatible)** | Probe any HTTP server for OpenAI-API compliance to get an honest matrix of how OSS implementations *actually* behave. | ⭐ 16 |
| **[unleash](https://github.com/heiervang-technologies/unleash)** | Unleash your agent (Rust). | ⭐ 14 |
| **[supercompact](https://github.com/heiervang-technologies/supercompact)** | Harder, better, faster, stronger context compaction for AI agents. | ⭐ 8 |
| **ht-\* forks** | Maintained forks of `vllm-omni`, `llama.cpp`, `pytorch`, `vllm`, `unsloth`, `mergekit`, `ACE-Step`, `codex`. | |

---

### 🤗 On the Hugging Face Hub

**31 models · 7 datasets · 6 spaces · 490 likes · ~21k downloads/month**

**Models**
- **[Qwen3-Voice-Embedding-12Hz](https://huggingface.co/marksverdhei/Qwen3-Voice-Embedding-12Hz-0.6B)** (0.6B & 1.7B) for speaker/voice embeddings · ~13k downloads, 48 ❤️
- **[GLM-4.7-Flash-FP8](https://huggingface.co/marksverdhei/GLM-4.7-Flash-FP8)** for FP8 quantization · 3.1k downloads, 19 ❤️
- **[Qwen3-Omni-30B-A3B-FP8](https://huggingface.co/marksverdhei/Qwen3-Omni-30B-A3B-FP8)** for FP8 any-to-any omni model · 3.3k downloads
- **[LCO-Embedding-Omni GGUF series](https://huggingface.co/marksverdhei)** for multimodal embeddings in GGUF
- **[modern-norbert3](https://huggingface.co/marksverdhei/modern-norbert3-base)** for Norwegian ModernBERT conversion
- **[t5-base-define](https://huggingface.co/marksverdhei/t5-base-define)** for definition generation

**Datasets** — [wordnet-definitions-en-2021](https://huggingface.co/datasets/marksverdhei/wordnet-definitions-en-2021) (11 ❤️) · [clickbait_title_classification](https://huggingface.co/datasets/marksverdhei/clickbait_title_classification) (6 ❤️)

**Spaces** — [transformer-training-visualized](https://huggingface.co/spaces/marksverdhei/transformer-training-visualized) · [explore-embedding-inversion](https://huggingface.co/spaces/marksverdhei/explore-embedding-inversion) · [saved-you-a-click](https://huggingface.co/spaces/marksverdhei/saved-you-a-click)

---

### 🔬 Research threads

- **Clickbait spoiling / "Saved You A Click":** Abstractive title-answering. Includes the [reddit-syac](https://huggingface.co/datasets/marksverdhei/reddit-syac-urls) dataset, pegasus/t5 spoiler models, a Gradio demo, and a browser extension from my MSc thesis.
- **Definition modeling:** Generating dictionary definitions with T5 + WordNet.
- **Norwegian NLP:** NorBERT/ModernBERT conversions and benchmark work.

---

<p align="center"><sub>📺 I build a lot of this live on <a href="https://www.twitch.tv/hyperplane_t">twitch.tv/hyperplane_t</a> — come say hi.</sub></p>
