# Awesome-FullDuplexSDM [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/Ruiqi-Yan/Awesome-FullDuplexSDM)
A curated list of full-duplex spoken dialogue models.  
<img height=30 src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Hand%20gestures/Waving%20Hand.png"/> Welcome to PR if you want to add some resources.

### Legend

**Type** — what the entry actually gives you:

| Type | Meaning |
|:--|:--|
| **End-to-end** | A standalone full-duplex model: audio in, audio out, duplex behaviour learned inside the model. `(omni)` means it also takes vision. |
| **Cascaded** | A complete system assembled from separate parts (streaming ASR + LLM + TTS + a duplex controller). |
| **Component** | One piece of the puzzle — turn detection, semantic VAD, streaming TTS, retrieval, dialogue management. Needs a host system. |
| **Method** | A training recipe, reward model, or data scheme rather than a deployable system. |
| **Framework** | Engineering scaffolding for building/serving duplex systems. |

**Open** — what has been released:

| Open | Meaning |
|:--|:--|
| **Code + weights** | Public repo *and* released checkpoints. |
| **Code** | Public repo, no checkpoints released (or none linked). |
| **API / closed** | Usable as a product or API; nothing released. |
| **—** | Paper or tech report only. |
| **?** | Could not verify. |

**Year** is the year of first public release (arXiv v1, blog post, or repo). Entries without a dated paper are marked with the year they appeared publicly.


## Datasets
| Title | Year | Open | Relevant&nbsp;Resources |
|:--|:-:|:-:|:-:|
| **DuplexChat** | 2026 | Data + code | [Github](https://github.com/sarulab-speech/DuplexChat)/[Huggingface](https://huggingface.co/datasets/sarulab-speech/DuplexChat) |
| **SOMMELIER: Scalable Open Multi-turn Audio Pre-processing for Full-duplex Speech Language Models** | 2026 | Code (pipeline) | [arXiv](https://arxiv.org/abs/2603.25750)/[Demo](https://kyudan1.github.io/sommelier.github.io//)/[Github](https://github.com/naver-ai/sommelier)/[Blog](https://clova.ai/en/tech-blog/conversation-doesnt-wait-its-turn-sommelier-a-data-pipeline-for-real-time-conversational-voice-ai) |
| **SmoothConv & DuplexConv: Large-Scale Chinese Full-Duplex Speech Datasets for Conversational AI** | 2026 | Data + code | [Github](https://github.com/qualialabsAI/SmoothConv-DuplexConv)/[Demo](https://qualialabsai.github.io/SmoothConv-DuplexConv)/[Huggingface](https://huggingface.co/datasets/qualialabsAI) |



## Models
| Title | Year | Type | Open | Relevant&nbsp;Resources |
|:--|:-:|:--|:-:|:-:|
| **JoyAI-Talker: Full-Duplex Speech Interactive Large Model Built for Empathetic Voice Agents** | 2026 | Cascaded | — | [arXiv](https://arxiv.org/abs/2608.01119) |
| **Qwen Audio Agent** | 2026 | Cascaded | Code | [Github](https://github.com/QwenAudio/qwen-audio-agent) |
| **Dual-Axis Generative Reward Model Toward Semantic and Turn-taking Robustness in Interactive Spoken Dialogue Models** | 2026 | Method | Code | [arXiv](https://arxiv.org/abs/2604.14920)/[Github](https://github.com/MM-Speech/DualAxisRM) |
| **DuplexOmni: Real-Time Listening, Seeing, Thinking, and Speaking for Full-Duplex Interaction** | 2026 | End-to-end (omni) | Code | [arXiv](https://arxiv.org/abs/2606.09186)/[Github](https://github.com/MuyeHuang/DuplexOmni) |
| **Hierarchical Acoustic-Semantic Modeling: Modality Separation and Semantic Coherence for Full-Duplex SLMs** | 2026 | End-to-end | Code + weights | [arXiv](https://arxiv.org/abs/2607.06540)/[Github](https://github.com/HITsz-TMG/Lychee-FD)/[Huggingface](https://huggingface.co/HIT-TMG/Lychee-FD)/[Demo](https://hitsz-tmg.github.io/Lychee-FD/lychee-fd-showcase/) |
| **BayLing-Duplex: Native Full-Duplex Speech Dialogue with a Single Autoregressive LLM** | 2026 | End-to-end | Code + weights | [arXiv](https://arxiv.org/abs/2606.14528)/[Github](https://github.com/BayLing-Models/BayLing-Duplex)/[Huggingface](https://huggingface.co/BayLing-Models/BayLing-Duplex) |
| **TurnSense and TurnSense 1.1: Three-Class Semantic Turn Detection for Chinese and English Speech Interaction** | 2026 | Component — turn detection | Code + weights | [Github](https://github.com/Bairong-Xdynamics/TurnSense)/[Huggingface](https://huggingface.co/brgroup/TurnSense) |
| **DuplexSLA: A Full-Duplex Spoken Language Model with Synchronized Speech, Language, and Action** | 2026 | End-to-end | Code | [Github](https://github.com/hyzhang24/DuplexSLA)/[Demo](https://hyzhang24.github.io/DuplexSLA/) |
| **X-Talk: On the Underestimated Potential of Modular Speech-to-Speech Dialogue System** | 2025 | Cascaded | Code | [arXiv](https://arxiv.org/abs/2512.18706)/[Github](https://github.com/xcc-zach/xtalk)/[Demo](https://xtalk.sjtuxlance.com/) |
| **Unmute** | 2025 | Cascaded | Code + weights | [arXiv](https://arxiv.org/abs/2509.08753)/[Github](https://github.com/kyutai-labs/unmute)/[Demo](https://unmute.sh/) |
| **Reinforcement Learning Enhanced Full-Duplex Spoken Dialogue Language Models for Conversational Interactions** | 2026 | Method | — | [paper](https://openreview.net/pdf?id=QbLbXz8Idp) |
| **MoshiRAG: Asynchronous Knowledge Retrieval for Full-Duplex Speech Language Models** | 2026 | Component — retrieval | Code + weights | [arXiv](https://arxiv.org/abs/2604.12928)/[Github](https://github.com/kyutai-labs/moshi-rag)/[Huggingface](https://hf.co/collections/kyutai/moshirag-release) |
| **Seeduplex: Native Full-Duplex Speech LLM** | 2026 | End-to-end | API / closed | [Release](https://seed.bytedance.com/en/blog/introducing-seed-full-duplex-speech-llm-attentive-listening-robust-interference-suppression-enabling-more-natural-interaction)/[Blog](https://seed.bytedance.com/en/seeduplex) |
| **FastTurn: Unifying Acoustic and Streaming Semantic Cues for Low-Latency and Robust Turn Detection** | 2026 | Component — turn detection | — | [arXiv](https://arxiv.org/abs/2604.01897) |
| **JAL-Turn: Joint Acoustic-Linguistic Modeling for Real-Time and Robust Turn-Taking Detection in Full-Duplex Spoken Dialogue Systems** | 2026 | Component — turn detection | — | [arXiv](https://arxiv.org/abs/2603.26515) |
| **TurnGuide: Enhancing Meaningful Full Duplex Spoken Interactions via Dynamic Turn-Level Text-Speech Interleaving** | 2025 | Method | Code | [arXiv](https://arxiv.org/abs/2508.07375)/[Github](https://github.com/dreamtheater123/TurnGuide)/[Demo](https://dreamtheater123.github.io/TurnGuide-Demo/) |
| **Qwen3.5-Omni** | 2026 | End-to-end (omni) | API / closed | [Official Blog](https://qwen.ai/blog?id=qwen3.5-omni) |
| **Covo-Audio** | 2026 | End-to-end | Code + weights | [arXiv](https://arxiv.org/abs/2602.09823)/[Github](https://github.com/Tencent/Covo-Audio)/[Huggingface](https://huggingface.co/tencent/Covo-Audio-Chat) |
| **SoulX-Duplug: Plug-and-Play Streaming State Prediction Module for Realtime Full-Duplex Speech Conversation** | 2026 | Component — semantic VAD | Code + weights | [arXiv](https://arxiv.org/abs/2603.14877)/[Github](https://github.com/Soul-AILab/SoulX-Duplug)/[Huggingface](https://huggingface.co/Soul-AILab/SoulX-Duplug-0.6B)/[Demo](https://soulx-duplug.sjtuxlance.com/) |
| **PHOENIX-VAD: STREAMING SEMANTIC ENDPOINT DETECTION FOR FULL-DUPLEX SPEECH INTERACTION** | 2025 | Component — VAD/endpointing | — | [arXiv](https://arxiv.org/abs/2509.20410) |
| **EASY TURN: INTEGRATING ACOUSTIC AND LINGUISTIC MODALITIES FOR ROBUST TURN-TAKING IN FULL-DUPLEX SPOKEN DIALOGUE SYSTEMS** | 2025 | Component — turn detection | Code | [arXiv](https://arxiv.org/abs/2509.23938)/[Github](https://github.com/ASLP-lab/Easy-Turn)/[Demo](https://aslp-lab.github.io/Easy-Turn/) |
| **Fun-Audio-Chat** | 2025 | End-to-end | Code | [arXiv](https://arxiv.org/pdf/2512.20156)/[Github](https://github.com/FunAudioLLM/Fun-Audio-Chat)/[Demo](https://funaudiollm.github.io/funaudiochat) |
| **FireRedChat: A Pluggable, Full-Duplex Voice Interaction System with Cascaded and Semi-Cascaded Implementations** | 2025 | Cascaded | Code | [arXiv](https://arxiv.org/pdf/2509.06502)/[Github](https://github.com/FireRedTeam/FireRedChat)/[Demo](https://fireredteam.github.io/demos/firered_chat/) |
| **PERSONAPLEX: VOICE AND ROLE CONTROL FOR FULL DUPLEX CONVERSATIONAL SPEECH MODELS** | 2026 | End-to-end | Code | [arXiv](https://arxiv.org/abs/2602.06053)/[Github](https://github.com/NVIDIA/personaplex)/[Demo](https://research.nvidia.com/labs/adlr/personaplex/) |
| **VITA: Towards Open-Source Interactive Omni Multimodal LLM** | 2024 | End-to-end (omni) | Code + weights | [arXiv](https://arxiv.org/abs/2408.05211)/[Github](https://github.com/VITA-MLLM/VITA)/[Demo](https://vita-home.github.io/) |
| **A Full-duplex Speech Dialogue Scheme Based On Large Language Models** | 2024 | End-to-end | — | [arXiv](https://arxiv.org/abs/2405.19487) |
| **Freeze-Omni: A Smart and Low Latency Speech-to-speech Dialogue Model with Frozen LLM** | 2024 | End-to-end | Code + weights | [arXiv](https://arxiv.org/abs/2411.00774)/[Github](https://github.com/VITA-MLLM/Freeze-Omni) |
| **Moshi: a speech-text foundation model for real-time dialogue** | 2024 | End-to-end | Code + weights | [arXiv](https://arxiv.org/abs/2410.00037)/[Github](https://github.com/kyutai-labs/moshi) |
| **FlexDuo: A Pluggable System for Enabling Full-Duplex Capabilities in Speech Dialogue Systems** | 2025 | Component — duplex control | — | [arXiv](https://arxiv.org/abs/2502.13472) |
| **MinMo: A Multimodal Large Language Model for Seamless Voice Interaction** | 2025 | End-to-end | — | [arXiv](https://arxiv.org/abs/2501.06282)/[Demo](https://funaudiollm.github.io/minmo/) |
| **SoulX-DuoVoice** | 2025 | End-to-end | ? | [Unofficial Intro](https://zhuanlan.zhihu.com/p/1926352123244832218) |
| **SALMONN-omni: A Standalone Speech LLM without Codec Injection for Full-duplex Conversation** | 2025 | End-to-end | Code | [arXiv](https://arxiv.org/abs/2505.17060)/[Github](https://github.com/bytedance/SALMONN) |
| **CleanS2S: Single-file Framework for Proactive Speech-to-Speech Interaction** | 2025 | Framework | Code | [arXiv](https://arxiv.org/abs/2506.01268)/[Github](https://github.com/opendilab/CleanS2S) |
| **Mini-Omni2: Towards Open-source GPT-4o with Vision, Speech and Duplex Capabilities** | 2024 | End-to-end (omni) | Code + weights | [arXiv](https://arxiv.org/abs/2410.11190)/[Github](https://github.com/gpt-omni/mini-omni2) |
| **Real-Time Textless Dialogue Generation** | 2025 | End-to-end | Code | [arXiv](https://arxiv.org/abs/2501.04877)/[Github](https://github.com/mailong25/rts2s-dg)/[Demo](https://mailong25.github.io/rts2s-dg/) |
| **Language Model Can Listen While Speaking** | 2024 | End-to-end | — | [arXiv](https://arxiv.org/abs/2408.02622)/[Demo](https://ziyang.tech/LSLM/) |
| **Parrot: Seamless Spoken Dialogue Interaction with Double-Channel Large Language Models** | 2024 | End-to-end | — | [Paper](https://openreview.net/pdf?id=73EDGbG6mB) |
| **Beyond Turn-Based Interfaces: Synchronous LLMs as Full-Duplex Dialogue Agents** | 2024 | End-to-end | — | [arXiv](https://arxiv.org/abs/2409.15594)/[Demo](https://syncllm.cs.washington.edu/) |
| **LLM-Enhanced Dialogue Management for Full-Duplex Spoken Dialogue Systems** | 2025 | Component — dialogue mgmt | — | [arXiv](https://arxiv.org/abs/2502.14145) |
| **Duplex Conversation: Towards Human-like Interaction in Spoken Dialogue Systems** | 2022 | Cascaded | — | [arXiv](https://arxiv.org/abs/2205.15060) |
| **Generative Spoken Dialogue Language Modeling** | 2022 | End-to-end | Code + weights | [arXiv](https://arxiv.org/abs/2203.16502)/[Github](https://github.com/facebookresearch/fairseq/tree/main/examples/textless_nlp/dgslm)/[Demo](https://speechbot.github.io/dgslm/) |
| **Duplex Conversation in Outbound Agent System** | 2021 | Cascaded | — | [Paper](https://www.isca-archive.org/interspeech_2021/jin21b_interspeech.html) |
| **OmniFlatten: An End-to-end GPT Model for Seamless Voice Conversation** | 2024 | End-to-end | — | [arXiv](https://arxiv.org/abs/2410.17799)/[Demo](https://omniflatten.github.io/) |
| **DuplexMamba: Enhancing Real-time Speech Conversations with Duplex and Streaming Capabilities** | 2025 | End-to-end | Code | [arXiv](https://arxiv.org/abs/2502.11123)/[Github](https://github.com/khfs/DuplexMamba) |
| **Beyond the Turn-Based Game: Enabling Real-Time Conversations with Duplex Models** | 2024 | Method | Code + data | [arXiv](https://arxiv.org/abs/2406.15718)/[Github](https://github.com/thunlp/duplex-model)/[HuggingFace](https://huggingface.co/datasets/xinrongzhang2022/Duplex-UltraChat) |
| **KAME: Tandem Architecture for Enhancing Knowledge in Real-Time Speech-to-Speech Conversational AI** | 2025 | Component — retrieval | Code + weights | [arXiv](https://arxiv.org/abs/2510.02327)/[Github](https://github.com/SakanaAI/kame)/[HuggingFace](https://huggingface.co/SakanaAI/kame) |
| **VoXtream: Full-Stream Text-to-Speech with Extremely Low Latency** | 2025 | Component — streaming TTS | Code | [arXiv](https://arxiv.org/pdf/2509.15969)/[Github](https://github.com/herimor/voxtream)/[Demo](https://herimor.github.io/voxtream/) |
| **VoXtream2: Full-stream TTS with dynamic speaking rate control** | 2026 | Component — streaming TTS | Code | [arXiv](https://arxiv.org/abs/2603.13518)/[Github](https://github.com/herimor/voxtream)/[Demo](https://herimor.github.io/voxtream2/) |



## Benchmark
| Title | Year | Relevant&nbsp;Resources |
|:--|:-:|:-:|
| **Game-Time: Evaluating Temporal Dynamics in Spoken Language Models** | 2025 | [arXiv](https://arxiv.org/abs/2509.26388)/[Demo](https://ga642381.github.io/Game-Time)/[Dataset](https://huggingface.co/datasets/gametime-benchmark/gametime) |
| **Semantic-Aware Interruption Detection in Spoken Dialogue Systems: Benchmark, Metric, and Model** | 2026 | [arXiv](https://arxiv.org/abs/2603.24144)/[Github](https://github.com/xkx-hub/SID-bench) |
| **Full-Duplex Interaction in Spoken Dialogue Systems: A Comprehensive Study from the ICASSP 2026 HumDial Challenge** | 2026 | [arXiv](https://arxiv.org/abs/2604.21406)/[Github](https://github.com/ASLP-lab/HumDial-FDBench)/[Dataset](https://huggingface.co/datasets/ASLP-lab/HumDial-FDBench) |
| **Full-Duplex-Bench-v3: Benchmarking Tool Use for Full-Duplex Voice Agents Under Real-World Disfluency** | 2026 | [arXiv](https://arxiv.org/abs/2604.04847)/[Github](https://github.com/DanielLin94144/Full-Duplex-Bench)/[Demo](https://daniellin94144.github.io/FDB-v3-demo) |
| **Full-Duplex-Bench-v2: A Multi-Turn Evaluation Framework for Duplex Dialogue Systems with an Automated Examiner** | 2025 | [arXiv](https://arxiv.org/abs/2510.07838)/[Github](https://github.com/DanielLin94144/Full-Duplex-Bench) |
| **FULL-DUPLEX-BENCH V1.5: Evaluating Overlap Handling for Full-Duplex Speech Models** | 2025 | [arXiv](https://arxiv.org/abs/2507.23159)/[Github](https://github.com/DanielLin94144/Full-Duplex-Bench) |
| **Full-Duplex-Bench: A Benchmark to Evaluate Full-duplex Spoken Dialogue Models on Turn-taking Capabilities** | 2025 | [arXiv](https://arxiv.org/abs/2503.04721)/[Github](https://github.com/DanielLin94144/Full-Duplex-Bench) |
| **MTR-DuplexBench: Towards a Comprehensive Evaluation of Multi-Round Conversations for Full-Duplex Speech Language Models** | 2025 | [arXiv](https://arxiv.org/abs/2511.10262) |
| **FD-Bench: A Full-Duplex Benchmarking Pipeline Designed for Full Duplex Spoken Dialogue Systems** | 2025 | [arXiv](https://arxiv.org/abs/2507.19040)/[Github](https://github.com/pengyizhou/FD-Bench)/[Dataset](https://huggingface.co/collections/pengyizhou/fd-bench-audio-68674bd6de6feea91ba3ce37) |
| **Talking Turns: Benchmarking Audio Foundation Models on Turn-Taking Dynamics** | 2025 | [arXiv](https://arxiv.org/abs/2503.01174) |



## Survey
| Title | Year | Relevant&nbsp;Resources |
|:--|:-:|:-:|
| **A Survey of Full-Duplex Spoken Dialogue Systems: Architectural Hierarchy, Interaction Ontology, and Decision State Machine** | 2026 | [arXiv](https://arxiv.org/abs/2606.19453)/[Github](https://github.com/DuplexLM/DuplexSurvey) |
| **From Turn-Taking to Synchronous Dialogue: A Survey of Full-Duplex Spoken Language Models** | 2025 | [arXiv](https://arxiv.org/abs/2509.14515)/[Github](https://github.com/elpsykongloo/FD-SLMs) |


