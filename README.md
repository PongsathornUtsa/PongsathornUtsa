<div align="center">

# Pongsathorn Utsahawattanasuk

### AI Engineer · RAG & LLM Systems · Thai–English NLP

**Senior Associate, Automation at True Digital Group** · Bangkok, Thailand 🇹🇭

[![LinkedIn](https://img.shields.io/badge/LinkedIn-peachutsa-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/peachutsa)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-Pongsathorn-FFD21E?logo=huggingface&logoColor=black)](https://huggingface.co/Pongsathorn)
[![Kaggle](https://img.shields.io/badge/Kaggle-pongsathorn789-20BEFF?logo=kaggle&logoColor=white)](https://www.kaggle.com/pongsathorn789)
[![Email](https://img.shields.io/badge/Email-peachutsa%40gmail.com-D14836?logo=gmail&logoColor=white)](mailto:peachutsa@gmail.com)

</div>

## 👋 About me

I'm **Pongsathorn (Peach)**, an AI engineer who builds **retrieval-augmented generation (RAG)** and **large language model (LLM)** systems for **Thai and English** documents that mix text, tables and figures.

My rule is simple: **a default changes only after a measured gain, and every change is measured per language.**

- 🔭 **Now:** building **TDG-RAG**, a production multilingual RAG service at True Digital Group
- 🔬 **Research interests:** multimodal and cross-lingual RAG and how to evaluate it, grounding LLMs in documents, efficient training and serving on GPU / HPC
- 📄 **Published:** ITC-CSCC 2024 (IEEE)
- 🏅 **Certified:** NVIDIA Generative AI LLMs (NCA-GENL) · NVIDIA AI Infrastructure and Operations (NCA-AIIO)

## 📈 Highlights

| Metric | Result |
|---|---|
| Text retrieval MRR (dense → hybrid → reranked) | **0.766 → 0.863 → 0.940** |
| Top-10 answer recall (1,081 questions, 7 datasets) | **97.5%** |
| Cross-lingual retrieval MRR (adaptive translation routing) | **0.983** |
| Multimodal figure QA on MMLongBench-Doc (80 questions) | **36 → 44 correct** |
| Thai far-field speech recognition (wav2vec 2.0) | **WER 13.59% · CER 4.60%** |

## 💼 Experience

### Senior Associate, Automation · True Digital Group
*Dec 2025 – present*

I designed and built **TDG-RAG**, a production **Thai–English RAG service** on **PostgreSQL + pgvector** and **Gemini**. It runs as web, queue and worker services on **Google Cloud Run and Cloud SQL**, with an **MCP server** for AI agents.

- **Hybrid retrieval:** dense pgvector search plus **BM25 in plain SQL** with Thai word segmentation, convex score fusion and a multilingual **cross-encoder reranker**
- **Cross-lingual retrieval:** a router adds translated query legs (LLM or local **NLLB-200**) only when native-language search is weak. It reached an MRR of 0.983, compared with 0.970 for never translating and 0.940 for always translating
- **Multimodal RAG:** a vision model describes figures and a text model describes tables, and both descriptions are tied to the page and caption structure
- **Document parsing:** **Docling** layout and **TableFormer** produce structure-aware chunks. A font-table repair cut broken Thai characters from 35,328 to 115

### Senior Associate, True Next Gen · True Corporation
*Jun 2024 – Nov 2025*: tech talent programme with rotations in data, sales and network operations

- **Churn prediction** for postpaid customers, plus **sentiment analysis with locally hosted LLMs**
- Real-time **Grafana** monitoring for the **5G core** (Huawei / ZTE), with Python and Bash ETL into **TimescaleDB**
- **Robocorp** RPA bots for social-media analytics, and incentive-plan design for regional sales

<details>
<summary><b>Earlier roles: AIS · NECTEC · Super AI Engineer</b></summary>

### Network Engineer, IP Core · AIS
*Aug 2023 – May 2024*. I operated BNG, CGN, RADIUS and VMware vSphere, and wrote **Python (Netmiko)** automation for multi-vendor config backups, reachability checks and SNMP reports.

### Research Assistant · NECTEC Speech and Text Understanding Lab
*May – Jul 2023*. I fine-tuned **wav2vec 2.0** for far-field **Thai speech recognition** on the **LANTA supercomputer** and served the model with Docker and FastAPI.

### AI Engineer Apprentice · Super AI Engineer Season 3
*Oct 2022 – Aug 2023*. An eleven-month national programme solving real-world AI problems in vision, signal processing, NLP, big data and robotics.

</details>

## 🔬 Projects & publication

- 📄 **[NFT-Based Verification of Academic Credentials](https://doi.org/10.1109/ITC-CSCC62988.2024.10628144)**, *ITC-CSCC 2024*, Okinawa, Japan. A blockchain credential system for the Kasetsart University Graduate School. Code: [kucertV2](https://github.com/PongsathornUtsa/kucertV2) (Solidity + React)
- 🤖 **Name That LLM (Kaggle)** identifies which of 18 LLMs wrote a text. It is an explainable two-tier hierarchy (source family → model) with **Qwen2.5 LoRA** fine-tunes, and it scores **0.609** on the public leaderboard
- 🌫️ **[IoT air-quality monitor](https://github.com/PongsathornUtsa/IOT_project)** runs on ESP32 / ESP8266 with **FreeRTOS** multitasking, PM2.5 and weather sensors, and **MQTT** to the NETPIE cloud

## 🎓 Education & certifications

- **B.Eng. Electrical Engineering**, Kasetsart University (2019–2023): **First Class Honours**, GPA 3.65, top 5.7% of 1,122 students
- **NVIDIA-Certified Associate:** Generative AI LLMs (NCA-GENL), AI Infrastructure and Operations (NCA-AIIO), 2026
- **Cisco** CCNA Automation · CCST Networking · AI Technical Practitioner
- **Microsoft** Azure Fundamentals (AZ-900) · **Huawei** HCCDA Tech Essentials

## 🛠️ Tech stack

- **AI / ML:** PyTorch, Hugging Face Transformers, LoRA / PEFT, Gemini, RAG, embeddings, rerankers, speech recognition
- **Backend & data:** Python, SQL, PostgreSQL / pgvector, TimescaleDB, FastAPI, Bash
- **Cloud & infra:** Google Cloud (Cloud Run, Cloud SQL), Docker, Terraform, HPC clusters, Grafana
- **Other:** C / C++, JavaScript / React, Solidity, Cisco networking, ESP32 / Arduino

<p>
<img alt="Python" src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white">
<img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white">
<img alt="Hugging Face" src="https://img.shields.io/badge/Hugging%20Face-FFD21E?logo=huggingface&logoColor=black">
<img alt="Google Gemini" src="https://img.shields.io/badge/Gemini-8E75B2?logo=googlegemini&logoColor=white">
<img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white">
<img alt="FastAPI" src="https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white">
<img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white">
<img alt="Google Cloud" src="https://img.shields.io/badge/Google%20Cloud-4285F4?logo=googlecloud&logoColor=white">
<img alt="Terraform" src="https://img.shields.io/badge/Terraform-844FBA?logo=terraform&logoColor=white">
<img alt="Grafana" src="https://img.shields.io/badge/Grafana-F46800?logo=grafana&logoColor=white">
<img alt="React" src="https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB">
<img alt="Cisco" src="https://img.shields.io/badge/Cisco-1BA0D7?logo=cisco&logoColor=white">
</p>

---

<div align="center">

📫 Open to conversations about **RAG, LLM evaluation, Thai NLP** and ML research.<br>
Reach me on [LinkedIn](https://www.linkedin.com/in/peachutsa) or at **peachutsa@gmail.com**.

</div>
