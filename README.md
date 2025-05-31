# <!-- README.md  (English version) -->
<p align="center">
  <a href="README_zh_CN.md">👉 中文版</a>
</p>

<p align="center">
  <img src="https://img.shields.io/github/actions/workflow/status/SmartifCane/SmartifCane/build.yml?branch=main&label=build" alt="Build Status">
  <img src="https://img.shields.io/github/v/release/SmartifCane/SmartifCane" alt="Latest Release">
  <img src="https://img.shields.io/github/license/SmartifCane/SmartifCane" alt="License">
  <img src="https://img.shields.io/github/downloads/SmartifCane/SmartifCane/total" alt="Downloads">
</p>

# SmartifCane

> **An open-source AI-powered smart cane that fuses multi-modal perception with graph-gated agents to assist the visually impaired.**

## Table of Contents
1. [Project Overview](#project-overview)  
2. [Key Features](#key-features)  
3. [System Architecture](#system-architecture)  
4. [Hardware Components](#hardware-components)  
5. [Quick Start](#quick-start)  
6. [Directory Layout](#directory-layout)  
7. [Models & Data](#models--data)  
8. [Demo](#demo)  
9. [Performance Benchmarks](#performance-benchmarks)  
10. [Roadmap](#roadmap)  
11. [Contributing](#contributing)  
12. [Community & Support](#community--support)  
13. [License](#license)  
14. [Acknowledgements](#acknowledgements)  

---

## Project Overview
SmartifCane combines a lightweight visual-detection engine, graph-neural gates, and large-language-model prompts to deliver fine-grained spatial awareness and natural language feedback for outdoor and indoor navigation.

## Key Features
| Module          | Keywords                 | Description                               |
|-----------------|--------------------------|-------------------------------------------|
| Visual Detection| Lightweight OD engine    | Real-time obstacle & signage recognition  |
| Semantic Voice  | MoE Prompts ＋ LLM       | Personalized, multi-lingual scene speech  |
| Emotional Aid   | Emotion + Memory Bank    | Tone adaption & long-term user memory     |
| Offline Mode    | On-device tiny models    | Core functions without Internet access    |

## System Architecture
```text
Camera → Detection Engine → MSDN ROI → GNN Gate → Prompt Template
                ↘               ↘
       Mic/Audio → ASR  →  LLM (DeepSeek)
