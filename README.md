# NeuroEdge-Medical-SLM
Offline-First Medical AI for Android

![License](https://img.shields.io/badge/license-MIT-blue) ![Platform](https://img.shields.io/badge/platform-Android%20(Offline)-green) ![Model](https://img.shields.io/badge/model-Qwen2.5--1.5B-orange)

**NeuroEdge** is a privacy-first, offline-native Small Language Model (SLM) designed to provide medical guidance in connectivity-constrained environments. Built as a Final Year Project (FYP).

## Key Features
* **100% Offline:** Runs entirely on-device using the CPU (ARM64).
* **Privacy Focused:** No patient data leaves the phone.
* **Optimized:** 1.5B Parameters quantized to 4-bit (q4_k_m) for speed.
* **Medical Domain:** Fine-tuned on PubMedQA for accurate diagnostic support.

##  Downloads
* **[Download the App (APK)](https://github.com/ALLEE16481/NeuroEdge-Medical-SLM/releases/download/v1.0.0/ChatterUI_v0.8.9-beta7.apk)**
* **[Download the Model (GGUF)](https://github.com/ALLEE16481/NeuroEdge-Medical-SLM/releases/download/v1.0.0/neuroedge-medical-q4_k_m.gguf)**

##  Tech Stack
* **Base Model:** Qwen2.5-1.5B-Instruct
* **Fine-Tuning:** QLoRA (Peft + BitsAndBytes) on Tesla T4 GPU.
* **Quantization:** `llama.cpp` (GGUF Format).
* **Inference Engine:** Llama.cpp Android / ChatterUI.

##  How to Run
1.  Download and install the **APK** from the `app/` folder.
2.  Download the **Model file (.gguf)** from the link above.
3.  Open the App $\rightarrow$ **Load Model** $\rightarrow$ Select `neuroedge-medical-q4_k_m.gguf`.
4.  **Settings:** Set `Temperature: 0.6` and `Repetition Penalty: 1.15`.
5.  Ask a medical question!

##  Performance
| Metric | Value |
| :--- | :--- |
| **Model Size** | 935 MB |
| **Inference Speed** | ~5.2 tokens/sec (Snapdragon/Pixel) |
| **RAM Usage** | ~1.2 GB |
| **Precision** | 4-bit (Q4_K_M) |

##  Author
**Ali Muttahar**
