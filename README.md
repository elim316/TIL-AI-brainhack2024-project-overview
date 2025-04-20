# Operation Guardian – DSTA BrainHack 2024 Case Study

![Challenge](https://img.shields.io/badge/Event-DSTA%20BrainHack%202024-red)
![Role](https://img.shields.io/badge/Role-NLP%20Engineer-green)
![Tech](https://img.shields.io/badge/Built%20With-Python-blue)
![NLP](https://img.shields.io/badge/NLP-spaCy%20%7C%20NLTK-lightgrey)
![System](https://img.shields.io/badge/System-Multimodal%20AI-purple)
![Tools](https://img.shields.io/badge/Tools-Docker%20%7C%20GitHub-brightgreen)


This repository documents my contributions to **Operation Guardian**, a challenge project for the DSTA BrainHack 2024. The task was to develop an intelligent system capable of interpreting spoken commands and identifying visual targets in a simulated defense scenario.

---

## Project Overview

Operation Guardian involved building a multi-stage AI pipeline to simulate an automated turret command system. The challenge was split into three key technical areas:

1. **ASR (Automatic Speech Recognition)** – Convert noisy audio to transcribed text  
2. **NLP (Natural Language Processing)** – Extract structured commands from speech  
3. **VLM (Vision-Language Model)** – Identify and localize targets within an image based on natural language descriptions

Our team collaborated using Git, Docker, and shared documentation, and we were evaluated on model accuracy, latency, and robustness to noise.

---

## My Role: Natural Language Processing (NLP)

As part of the NLP subteam, I was responsible for transforming raw transcribed speech into structured commands that could be used by the turret control system. This included:

- **Entity Extraction & Classification**  
  Used rule-based parsing and spaCy NLP pipelines to extract commands like `FIRE`, target descriptors, and action types.

- **Custom Intent Mapping**  
  Designed a lightweight command grammar to standardize variable input into structured JSON-like instructions (e.g., `{action: "fire", heading: 240, target: "drone"}`).

- **Noise Robustness**  
  Created fallback mechanisms and regex patterns to handle ASR transcription errors and ambiguity in command phrasing.

- **Model Integration**  
  Integrated the NLP module between the ASR and VLM layers, ensuring smooth data flow and compatibility across the pipeline.

- **Collaboration**  
  Worked closely with the ASR team to understand transcription patterns and with the VLM team to align semantic intent with target selection logic.

---

## Tech Stack

- Python, spaCy, NLTK, Regex
- JSON schema design
- Docker
- GitHub

---

## Team Contributions

| Task        | Contributors            |
|-------------|--------------------------|
| ASR         | Adrian, Peter            |
| NLP         | Elias *(my role)*        |
| VLM         | Aaron                    |
| Docker      | Everyone                 |

---

## Note

Due to the nature of the challenge and team agreement, source code cannot be made public. This case study is intended to summarize my contributions and technical approach.

---

## What I Learned

- Designing NLP pipelines for real-world command parsing
- Handling transcription noise in downstream tasks
- Working across a modular, multi-model AI pipeline
- Communicating and collaborating in a high-stakes, time-sensitive team project

---

## Challenge Details

- [View the Official Challenge Brief](https://tribegroup.notion.site/Project-Submission-74caa4421c5e42bc9bc044111b63025d)

---

