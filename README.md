# 易收纳 (Good Idea) – Optional ASR Models

This public repository distributes optional offline speech-recognition model
assets used by the 易收纳 (Good Idea) app during development.

## Current model

- Model: Qwen3-ASR-0.6B
- Runtime format: sherpa-onnx ONNX INT8
- Model version: 2026-03-25
- License: Apache License 2.0
- Original model: https://huggingface.co/Qwen/Qwen3-ASR-0.6B
- ONNX conversion and upstream package:
  https://github.com/k2-fsa/sherpa-onnx/releases/tag/asr-models
- sherpa-onnx export documentation:
  https://k2-fsa.github.io/sherpa/onnx/qwen3-asr/export.html

The model files are published as GitHub Release assets instead of Git objects,
so the app source repository stays small. The app downloads the selected model
on demand and verifies every file with its size and SHA-256 digest.

See the `LICENSE-QWEN-APACHE-2.0.txt` and `NOTICE.txt` assets in each release.

This repository contains model distribution metadata only. It does not contain
app source code, user audio, transcripts, account data, or other user data.
