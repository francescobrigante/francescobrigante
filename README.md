<div align="center">

# Francesco Brigante

**Applied AI Researcher @ [Translated](https://translated.com) · PhD Student @ [Sapienza University of Rome](https://www.uniroma1.it)**

Large-scale generative models · Representation learning · Audio & music ML

[![SAGE paper](https://img.shields.io/badge/SAGE-arXiv%3A2609.32755-b31b1b?style=flat-square&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2609.32755)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/francesco-brigante-666021215/)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:francescobrigantefb@gmail.com)

</div>

---

I train large generative models, at work and in my research.

At **Translated**, in the Foundation Models team, I work on pre-training, continued pre-training and distillation of large-scale multilingual language models.
At **Sapienza**, as a PhD student, I study generative models for audio and how to give their latent spaces semantic structure.
Before that I worked on production LLM systems, including a RAG assistant deployed for the Italian Ministry of Education.

I like owning the whole stack: data curation, model design, custom CUDA kernels, distributed training on HPC and careful evaluation.
I'm also a musician, which is where the audio obsession comes from.

---

### ⭐ Featured Research

#### [SAGE: Semantic Audio Generative Encoder](https://github.com/francescobrigante/SAGE)

[Paper](https://arxiv.org/abs/2609.32755) · [Project page](https://sage-music.pages.dev/) · [Weights](https://huggingface.co/francescobrigante/SAGE)

<table>
<tr>
<td width="50%" valign="middle">
<a href="https://github.com/francescobrigante/SAGE">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/francescobrigante/SAGE/main/docs/assets/efficiency_dark.png">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/francescobrigante/SAGE/main/docs/assets/efficiency.png">
  <img src="https://raw.githubusercontent.com/francescobrigante/SAGE/main/docs/assets/efficiency.png" width="100%" alt="SAGE: fidelity vs inference cost">
</picture>
</a>
</td>
<td width="50%" valign="middle">

A compact **105M-parameter VAE for 44.1 kHz stereo music**. A Swin Transformer V2 encoder and decoder work on the STFT, and LAION-CLAP semantic distillation shapes the latent space.

- **High fidelity, low cost:** matches an autoencoder 8× larger and 4× slower in listening tests
- **Semantic latent:** state of the art on all 19 latent-probing tasks
- **Open and reproducible:** trained only on public music
- **Built end to end:** data, fused CUDA kernels, DDP on 16×A100 (CINECA Leonardo), evaluation

<sub>Supported by an ISCRA allocation on Leonardo and a €5,000 Google Cloud Research Credits award.</sub>

</td>
</tr>
</table>

---

### 🎵 Selected Projects

| Project | What it is | Highlight |
|---|---|---|
| [**Audio2PianoRoll**](https://github.com/francescobrigante/Audio2PianoRoll) | Automatic music transcription with CQT and a custom U-Net | 83% F1 on GuitarSet |
| [**Real-Time AI Accompaniment**](https://www.youtube.com/watch?v=rMqet5fySLI) | Neural and symbolic system that accompanies a live musician | <10 ms end-to-end latency · [demo](https://www.youtube.com/watch?v=rMqet5fySLI) |
| [**Audio Style Transfer**](https://github.com/francescobrigante/Audio-Style-Transfer) | Piano ↔ violin transfer through latent disentanglement | Complex-valued representations |
| [**VectorRAG vs GraphRAG**](https://github.com/francescobrigante/VectorRAG-vs-GraphRAG) | Benchmark of vector, graph and hybrid RAG for enterprise retrieval | 10× fewer tokens at 0.84 faithfulness |

### 🔧 Open-Source Contributions

**[microsoft/Swin-Transformer #389](https://github.com/microsoft/Swin-Transformer/pull/389)** &nbsp;![stars](https://img.shields.io/github/stars/microsoft/Swin-Transformer?style=flat-square&label=%E2%98%85&color=555)  
Fused window CUDA kernels: fixed an out-of-bounds read that silently corrupts outputs on any non-square input, generalised the kernels to non-square windows, per-axis shifts and bfloat16, and ported them to ROCm, where they had never compiled. Bit-exact against eager on NVIDIA RTX 3080 and AMD MI300X, with a GPU-free test suite running in CI.

---

### 🛠️ Stack

**Large-scale training:** PyTorch (DDP) · Megatron Bridge · Lightning · Hydra · SLURM / HPC · Weights & Biases  
**Kernels & systems:** CUDA · ROCm · C++ · Python  
**LLMs:** Hugging Face Transformers · PEFT / QLoRA · distillation · LLM evaluation · RAG  
**Audio:** torchaudio · librosa · neural audio codecs · MIDI

---

<div align="center">

Happy to talk about audio generative models, large-scale training or music. The best way to reach me is [email](mailto:francescobrigantefb@gmail.com).

</div>
