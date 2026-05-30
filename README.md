<h1 align="center">hei.</h1>

<p align="center">
  <img src="https://github.com/marksverdhei/marksverdhei/blob/main/3d.gif?raw=true" width="320" alt="Rotating dog.">
</p>

<p align="center">
  <em>Making clankers think and GPUs go BRRR</em>
</p>

<p align="center">
  <a href="https://huggingface.co/marksverdhei"><img src="https://img.shields.io/badge/Hugging%20Face-marksverdhei-FFD21E?logo=huggingface&logoColor=black"></a>
  <a href="https://www.twitch.tv/hyperplane_t"><img src="https://img.shields.io/badge/Twitch-hyperplane__t-9146FF?logo=twitch&logoColor=white"></a>
  <a href="https://www.youtube.com/@marksverdhei"><img src="https://img.shields.io/badge/YouTube-marksverdhei-FF0000?logo=youtube&logoColor=white"></a>
  <img src="https://img.shields.io/badge/Based%20in-Norway-2f6feb">
  <a href="https://marksverdhei.github.io/marksverdhei/github-wrapped-2025.html"><img src="https://img.shields.io/badge/2025-Wrapped-f107a3"></a>
</p>

---

### About

LLM engineer at the **[National Library of Norway](https://github.com/NationalLibraryOfNorway)**, where I help pretrain, post-train and evaluate Norwegian large language models, most recently the **Borealis** family. Off the clock I run **[Heiervang Technologies](https://github.com/heiervang-technologies)**, an open-source lab for AI agents, inference tooling, and forks of the libraries I use daily. MSc in Informatics (NLP) from the University of Oslo. I stream a lot of the process on Twitch and YouTube.

My work spans the full model lifecycle: data → training → quantization → serving → evaluation → agents.

---

### Featured

**[Borealis](https://huggingface.co/NbAiLab):** The National Library of Norway's newly released family of Norwegian language models. Built on Gemma 3, spanning 270M to 27B parameters, vision-language capable, fluent in Bokmål and Nynorsk, and shipped in open and full-data variants with GGUF and MLX builds. I'm part of the team behind it.

**[unleash](https://github.com/heiervang-technologies/unleash):** A Rust harness for running coding agents autonomously. (⭐ 14)

---

### What I work on

I get **brand-new models running on open inference stacks**, then handle the lifecycle around them: quantize, serve, evaluate, and wrap in agents.

- **Model enablement & inference:** New architectures (GLM-4.7, Qwen3-Omni/TTS, GPT-OSS) brought up in vLLM, vllm-omni, and Hugging Face Transformers.
- **Quantization:** FP8, MXFP4, and GGUF to squeeze large models onto smaller and non-NVIDIA GPUs (Vulkan, ZLUDA).
- **Speech, voice & audio:** Speaker/voice embeddings, TTS, ASR, music generation.
- **LLM training & fine-tuning:** Pre/post-training Norwegian LLMs, LoRA, prompt baking, synthetic data.
- **Evaluation & benchmarking:** EuroEval, lm-eval-harness, NorEval, MTEB.
- **AI agents & dev tooling:** Agent orchestration, context compaction, CLI tools.

---

### Open-source contributions

Getting brand-new models and fixes into the core ML stack:

- **GLM-4.7-Flash → vLLM:** Taught vLLM's MLA detection about `glm4_moe_lite` so the model runs on the engine. [vllm#32614](https://github.com/vllm-project/vllm/pull/32614)
- **Qwen3-TTS → vllm-omni:** Added speaker-embedding passthrough for the speech & voices APIs, a `speaker` alias, and a fix for the Qwen3-TTS-0.6B profile-run hang. [#1227](https://github.com/vllm-project/vllm-omni/pull/1227) · [#2424](https://github.com/vllm-project/vllm-omni/pull/2424) · [#1082](https://github.com/vllm-project/vllm-omni/pull/1082)
- **GPT-OSS MXFP4 quant → Transformers:** Fixed the MXFP4 quantizer to handle variable `num_local_experts`/`hidden_size`, so GPT-OSS models quantize correctly. [transformers#41795](https://github.com/huggingface/transformers/pull/41795)
- **OpenAI-compatible API eval → lm-evaluation-harness:** Fixed the assertion error that broke evaluation against OpenAI-compatible endpoints. [lm-eval#3356](https://github.com/EleutherAI/lm-evaluation-harness/pull/3356)

Plus smaller fixes to **[NVIDIA/Megatron-LM](https://github.com/NVIDIA/Megatron-LM/pull/1980)** (mcore example training loop), **[EuroEval](https://github.com/EuroEval/EuroEval/pull/865)** (fp16 loading for bf16 models on pre-Ampere GPUs), and **[ltgoslo/noreval](https://github.com/ltgoslo/noreval)**.

---

<details>
<summary><h3>📂 See all open projects</h3></summary>

A running index of my public work. (HT = under [Heiervang Technologies](https://github.com/heiervang-technologies).)

**Agents & LLM tooling**
- **[am-i-openai-compatible](https://github.com/heiervang-technologies/am-i-openai-compatible):** Probe any HTTP server for OpenAI-API compliance, with an honest matrix of how OSS implementations actually behave. HT · ⭐ 16
- **[supercompact](https://github.com/heiervang-technologies/supercompact):** Harder, better, faster, stronger context compaction for AI agents. HT · ⭐ 8
- **[sorting-hat](https://github.com/marksverdhei/sorting-hat):** AI file-naming CLI with animated ASCII art; works with any OpenAI-compatible LLM. ⭐ 16
- **[bakery](https://github.com/marksverdhei/bakery):** Prompt baking & context distillation for LLMs. ⭐ 5
- **[chatfiles](https://github.com/marksverdhei/chatfiles):** The dumbest and smartest way to make agents communicate. ⭐ 2
- **[syntk](https://github.com/marksverdhei/syntk):** Synthetic-data toolkit.
- **[exex](https://github.com/marksverdhei/exex):** Expert exchange.
- **[markutils](https://github.com/marksverdhei/markutils):** Python utilities I reach for constantly.

**Local inference & models**
- **[localllama-with-vulkan](https://github.com/marksverdhei/localllama-with-vulkan):** Run LLM inference on any GPU; tutorials and benchmarks.
- **[replications](https://github.com/marksverdhei/replications):** Install diaries, container images, and guides for running or training the model that just dropped.
- **[norbert3-modernbert-conversion](https://github.com/marksverdhei/norbert3-modernbert-conversion):** Convert NorBERT3 weights into a ModernBERT architecture.
- **[ollama-modelfiles](https://github.com/marksverdhei/ollama-modelfiles):** A collection of Ollama Modelfiles.
- **ht-\* forks:** Maintained forks of `vllm-omni`, `llama.cpp`, `pytorch`, `vllm`, `unsloth`, `mergekit`, `ACE-Step`, `codex`. HT

**Speech, audio & vision**
- **[semantic-sound-search](https://github.com/marksverdhei/semantic-sound-search):** Semantic search over audio samples.
- **[spritegrid](https://github.com/marksverdhei/spritegrid):** Corrects AI-generated pixel art by applying grid sampling. ⭐ 3
- **[autonomous-pokerogue](https://github.com/marksverdhei/autonomous-pokerogue):** Turns PokéRogue into an idle clicker driven by vision-language models.

**MCP & data**
- **[dhlab-mcp](https://github.com/marksverdhei/dhlab-mcp):** MCP server for the National Library's DH-lab.
- **[ssb_mcp](https://github.com/marksverdhei/ssb_mcp):** MCP server for Statistics Norway (SSB).

**Writing, web & meta**
- **[Advent-of-AI-papers](https://github.com/marksverdhei/Advent-of-AI-papers):** An advent calendar for AI and NLP research papers.
- **[opensourcefriendly.dev](https://github.com/marksverdhei/opensourcefriendly.dev):** An index of open-source-friendly companies and developer integrations.
- **[python-template](https://github.com/marksverdhei/python-template):** My Python project template.
- **[dotfiles-public](https://github.com/marksverdhei/dotfiles-public):** My dotfiles, with an optional private extension.
- **[studies-portfolio](https://github.com/marksverdhei/studies-portfolio):** Compiled programming work from my CS/NLP studies.

</details>

---

### On the Hugging Face Hub

**31 models · 7 datasets · 6 spaces · 490 likes · 220k+ all-time downloads**

Live all-time download counters (auto-updating):

<p>
  <img src="https://img.shields.io/badge/dynamic/json?url=https%3A//huggingface.co/api/models/marksverdhei/GLM-4.7-Flash-FP8%3Fexpand%3DdownloadsAllTime&query=%24.downloadsAllTime&label=GLM-4.7-Flash-FP8&color=FFD21E&logo=huggingface&logoColor=black">
  <img src="https://img.shields.io/badge/dynamic/json?url=https%3A//huggingface.co/api/models/marksverdhei/Qwen3-Omni-30B-A3B-FP8%3Fexpand%3DdownloadsAllTime&query=%24.downloadsAllTime&label=Qwen3-Omni-30B-FP8&color=FFD21E&logo=huggingface&logoColor=black">
  <img src="https://img.shields.io/badge/dynamic/json?url=https%3A//huggingface.co/api/models/marksverdhei/Qwen3-Voice-Embedding-12Hz-0.6B%3Fexpand%3DdownloadsAllTime&query=%24.downloadsAllTime&label=Qwen3-Voice-Embedding&color=FFD21E&logo=huggingface&logoColor=black">
</p>

**Models**
- **[GLM-4.7-Flash-FP8](https://huggingface.co/marksverdhei/GLM-4.7-Flash-FP8):** FP8 quantization · 140k downloads, 19 likes.
- **[Qwen3-Voice-Embedding-12Hz](https://huggingface.co/marksverdhei/Qwen3-Voice-Embedding-12Hz-0.6B)** (0.6B & 1.7B): Speaker/voice embeddings · ~34k downloads, 48 likes.
- **[Qwen3-Omni-30B-A3B-FP8](https://huggingface.co/marksverdhei/Qwen3-Omni-30B-A3B-FP8):** FP8 any-to-any omni model · 30k downloads.
- **[LCO-Embedding-Omni GGUF series](https://huggingface.co/marksverdhei):** Multimodal embeddings in GGUF.
- **[modern-norbert3](https://huggingface.co/marksverdhei/modern-norbert3-base):** Norwegian ModernBERT conversion.
- **[t5-base-define](https://huggingface.co/marksverdhei/t5-base-define):** Definition generation.

**Datasets:** [wordnet-definitions-en-2021](https://huggingface.co/datasets/marksverdhei/wordnet-definitions-en-2021) (11 likes) · [clickbait_title_classification](https://huggingface.co/datasets/marksverdhei/clickbait_title_classification) (6 likes)

**Spaces:** [transformer-training-visualized](https://huggingface.co/spaces/marksverdhei/transformer-training-visualized) · [explore-embedding-inversion](https://huggingface.co/spaces/marksverdhei/explore-embedding-inversion) · [saved-you-a-click](https://huggingface.co/spaces/marksverdhei/saved-you-a-click)

---

### Research threads

- **Clickbait spoiling / "Saved You A Click":** Abstractive title-answering. MSc thesis line: the [reddit-syac](https://huggingface.co/datasets/marksverdhei/reddit-syac-urls) dataset, pegasus/t5 spoiler models, a Gradio demo, and a browser extension.
- **Definition modeling:** Generating dictionary definitions with T5 + WordNet.
- **Norwegian NLP:** NorBERT/ModernBERT conversions and benchmark work.

---

<div align="center">

I build a lot of this live on **[twitch.tv/hyperplane_t](https://www.twitch.tv/hyperplane_t)**. Come say hi.

<a href="https://github.com/marksverdhei/marksverdhei/raw/main/interleaved.mp4"><img src="https://github.com/marksverdhei/marksverdhei/blob/main/interleaved.gif?raw=true" width="420" alt="Click to watch the full clip."></a>

</div>
