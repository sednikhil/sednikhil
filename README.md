# Nikhil Gupta

I'm a computer vision engineer in New Delhi. I work on video understanding, ML infrastructure and applied research.

## What I work on

Founding engineer at AlliumIQ (Gurgaon) since March 2025. I built our video-intelligence platform from the first commit: detection, multi-object tracking and person re-ID that keeps identities across non-overlapping cameras. It's in field pilots with law-enforcement and defence agencies (300+ cameras, 10,000+ hours of footage), with airport pilots in progress, and cuts manual footage review by roughly 98%.

## Selected work

- Re-ID on CLIP and ViT/Swin backbones, fine-tuned on identity- and camera-disjoint splits, with Milvus (DiskANN, HNSW) for sub-second identity search.
- Cross-domain re-ID: reproduced baselines (89.64 mAP on Market-1501, 73.38 on MSMT17), wrote a GPU evaluator about 1000x faster than the NumPy reference, ran a 17-experiment ablation. Per-camera feature standardisation gave +4.87 mAP on unseen cameras without retraining.
- Canonicalising video at ingest (HEVC, closed GOP, CFR, pinned colour space) cut frame lookup from 432 ms to 15 ms.
- A 1.4/255 per-pixel difference between decoders was enough to push embeddings below a 0.999 cosine threshold, so decoder and colour space are pinned and parity-checked in CI.
- Inference on TensorRT FP16, NVDEC, cross-source frame batching and multi-GPU sharding, shipped as a five-service appliance (FastAPI, Redis, Milvus, PostgreSQL, Docker) on a single RTX 5090, installed on-site in air-gapped environments.

Before that I was an SDE intern at Midheaven Technologies (Aug 2024 to Mar 2025): 40+ Spring Boot APIs, and Redis session caching that cut auth latency 40% at 2,000+ RPS. B.Tech in Software Engineering, Delhi Technological University, 2025.

## Publication

*A Lightweight, Real-Time Fall Detection System for Edge Devices*, ICDAM 2025 (accepted). Detection, contextual filtering and tracking on a Raspberry Pi, 90.9% accuracy in real time.

## Skills

- ML and CV: PyTorch, person re-ID (CLIP, ViT, Swin), foundation-model fine-tuning, detection, multi-object tracking, Milvus (DiskANN/HNSW), OpenCV, MLflow
- Inference and video: TensorRT, ONNX Runtime, CUDA, NVENC/NVDEC, multi-GPU sharding, FFmpeg, HEVC/H.264, PyAV, PyNvVideoCodec, RTSP/MediaMTX
- Backend and infra: FastAPI, Node.js, Spring Boot, PostgreSQL, Redis, React, Docker Compose, AWS (EC2, S3, SageMaker), GitLab CI/CD, Prometheus, Nginx
- Languages: Python, C++, TypeScript, SQL, Bash

## Contact

[LinkedIn](https://www.linkedin.com/in/sednikhil) or [nikhilgupta1118@gmail.com](mailto:nikhilgupta1118@gmail.com)
