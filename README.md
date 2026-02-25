
# Neural Text-to-Speech (TTS) Evaluation

## Overview

This project evaluates the performance, latency, controllability, and audio quality of a neural Text-to-Speech system using structured engineering metrics.

The evaluation is conducted using the `gpt-4o-mini-tts` model and focuses on long-form input generation (600–800 words) to simulate realistic usage scenarios.

---

## Objectives

* Measure end-to-end latency
* Evaluate SSML-based controllability
* Assess speech naturalness and clarity
* Analyze system stability for long inputs
* Produce structured evaluation metrics

---

## Project Structure

```
.
├── TTS_Evaluation_Notebook_Generation.ipynb
├── generated_audio/
├── evaluation_reports/
└── README.md
```

* **TTS_Evaluation_Notebook_Generation.ipynb** – Main evaluation notebook
* **generated_audio/** – Output audio files
* **evaluation_reports/** – Structured evaluation results

---

## Evaluation Criteria

### 1. Latency

* API response time
* Audio generation time
* Total processing duration

### 2. Controllability

* Speech rate adjustments
* Pitch control
* Pause handling
* Emphasis via SSML

### 3. Audio Quality

* Naturalness
* Pronunciation clarity
* Prosody consistency
* Artifact detection

---

## Requirements

* Python 3.8+
* OpenAI-compatible API access
* Required libraries:

  ```
  pip install openai soundfile requests
  ```

---

## Usage

1. Configure your base URL and API key inside the notebook.
2. Run all cells in `TTS_Evaluation_Notebook_Generation.ipynb`.
3. Generated audio files and evaluation metrics will be saved automatically.

---

## Scope & Limitations

* Manual quality evaluation introduces subjectivity.
* Focused on a single TTS model.
* No automated MOS scoring integration.

---

## Future Work

* Multi-model benchmarking
* Automated speech quality metrics
* Real-time streaming evaluation
* Cross-lingual testing

---
