# vahan-ai-asr-benchmark

# ASR Evaluation for Bangalore Locality Recognition in Conversational Speech

This project benchmarks Automatic Speech Recognition (ASR) systems on conversational Hinglish speech containing Bangalore locality names under noisy real-world conditions.

## Models Evaluated

* Deepgram Nova-2 (baseline)
* Faster-Whisper Small

## Evaluation Metrics

* Word Error Rate (WER)
* Character Error Rate (CER)
* Entity Accuracy
* Latency

## Dataset

Custom dataset of 20 conversational audio recordings collected under:

* Quiet indoor conditions
* Fan noise
* Fast/whisper speech
* Traffic noise

## Runtime Configuration

The benchmarking pipeline was developed and executed using Google Colab.

Recommended runtime:

* GPU: T4 GPU
* Runtime Type: Python 3

Whisper benchmarking was executed using CPU inference due to CUDA compatibility issues encountered during Colab GPU execution.

## Key Findings

* Deepgram achieved lower latency and lower WER
* Whisper demonstrated better multilingual robustness in some conversational samples
* Both systems struggled with Bangalore locality recognition under noisy Hinglish speech

## Repository Structure

```text id="pk62p4"
vahan-ai-asr-benchmark/
│
├── audio/
├── results/
├── report/
└── vahan_asr_assignment.ipynb
```

## Files

* `audio/` → locality audio recordings
* `results/` → benchmark outputs and metrics
* `report/` → final benchmark report
* `vahan_asr_assignment.ipynb` → reproducible ASR benchmarking pipeline

## Report

Detailed benchmark analysis and findings are available in:
`report/final_report.pdf`
Also uploaded at Github

## Google Drive Link:
https://drive.google.com/drive/folders/1BvBVgpDM0PGPaO8jiCnPv7UgtvXieu4e?usp=sharing

## Audio and result Dataset

*Due to GitHub file upload limitations, the audio recordings are hosted on Google Drive.
*The folder contains all 20 conversational locality recordings used for benchmarking.
*Due to GitHub file upload limitations, the results are hosted on Google Drive.
*The folder contains all 5 CSV files.
