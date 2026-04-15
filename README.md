# Application of Multi-speaker Dialogue Content Recognition Technology in Open Scenarios

[![Project Status: Phase 2 Active](https://img.shields.io/badge/Project%20Status-Phase%202%20Active-orange)](#)

> **An end-to-end multi-speaker dialogue recognition system designed for unconstrained environments.**
> This project tackles the core challenge of "Who Spoke What and When" in open scenarios (e.g., smart meetings, remote work) by integrating Voice Activity Detection (VAD), Context-Aware Masking (CAM++), and Automatic Speech Recognition (ASR).

🌐 **Project Website & Progress Tracker:** [https://wuzhiyun112.github.io/speakerRecognition/](https://wuzhiyun112.github.io/speakerRecognition/)

---

## 🎯 Project Abstract
Traditional single-speaker speech recognition systems struggle to accurately distinguish and transcribe dialogue content in real-world scenarios due to alternating speakers, overlapping speech, and complex background noise. This project introduces a robust, modular pipeline designed for practical application:

1. **Speech Preprocessing:** The system resamples raw audio and applies a fine-tuned Voice Activity Detection (VAD) module to effectively remove silent segments and background noise, ensuring high-quality input data.
2. **Speaker Diarization & Verification:** Utilizing a Densely Connected Time Delay Neural Network (D-TDNN) combined with the **CAM++** architecture. It incorporates a Squeeze-and-Excitation (SE) Block to dynamically focus on the target speaker while suppressing irrelevant environmental noise.
3. **Automatic Speech Recognition (ASR):** Pre-trained models are deployed to convert the enhanced speech into text.
4. **Dialogue Structuring:** The output from the diarization and ASR modules are fused to generate structured, chronologically sorted transcripts in the format of *"Speaker ID + Timestamp + Text"*.

## 🚀 Key Technologies
* **CAM++ (Context-Aware Masking):** Captures multi-granularity contextual information to generate precise masks for target speakers.
* **SE-Block:** Adaptive calibration of global contextual information in the acoustic frontend.
* **Depthwise Separable Convolutions:** Replaces standard convolutions in the backbone to reduce computational complexity and inference latency, meeting the demands of edge-device deployment.

---
*Developed by YE Zixin, CAO Kainan, and WU Zhiyun.*
