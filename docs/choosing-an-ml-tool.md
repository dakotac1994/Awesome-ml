# Choosing an ML Tool

How to evaluate ML tooling before depending on it — and per-category picks from the [catalog](../README.md).

## Maintenance signals (check before you adopt)

1. **Release cadence.** A healthy project ships regularly. No release in 2+ years is a yellow flag (exceptions: finished, stable tools in maintenance mode — stable is fine, abandoned is not).
2. **Commit activity.** Recent commits on the default branch mean someone is home. Archived repos are dead — don't build on them. This list excludes archived projects (see exclusions).
3. **Hardware support.** For frameworks and optimization tooling, check which accelerators are supported (CUDA, ROCm, TPU, Apple Silicon, NPUs). Vendor-neutral tooling (ONNX Runtime, TVM) hedges against lock-in.
4. **License.** This space relicenses often (Redis, ScyllaDB, and others changed terms in 2024–2025). Always read the LICENSE file; the catalog records licenses verbatim.
5. **SaaS vs. self-hosted.** Proprietary MLOps SaaS (Weights & Biases, Neptune, Comet) is labeled `proprietary` in the catalog. For regulated data, prefer self-hosted options (MLflow, ClearML, Aim).
6. **Ecosystem fit.** Pick the framework your team and hiring pool already know; switching costs in ML are high (data pipelines, model zoos, serving infra all couple to the choice).

## Per-category picks (opinionated starting points)

- **Deep learning:** PyTorch for research and most production DL; JAX for composable transforms and TPU work; TensorFlow where the TF ecosystem (TFX, TF Serving) is already entrenched; Keras 3 as the multi-backend high-level API.
- **Classical ML / tabular:** XGBoost or LightGBM first; CatBoost for categorical-heavy data; scikit-learn as the baseline everything compares against.
- **Distributed training:** PyTorch's native DDP/FSDP for most cases; DeepSpeed for very large models (ZeRO); Ray Train for heterogeneous, fault-tolerant jobs.
- **Experiment tracking:** MLflow for the self-hosted default; Aim for comparing thousands of runs cheaply; Weights & Biases if you want managed SaaS.
- **Model serving:** NVIDIA Triton for GPU inference at scale; BentoML for framework-agnostic packaging; KServe for Kubernetes-native serving.
- **Feature stores:** Feast for the open-source default.
- **AutoML:** AutoGluon for tabular + multimodal; FLAML for fast, lightweight tuning; Optuna for the search algorithm underneath everything.
- **Optimization:** ONNX Runtime for portable inference; TensorRT for NVIDIA GPUs; OpenVINO for Intel hardware; Apache TVM for cross-hardware compilation.
