# Awesome ML

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Entries](https://img.shields.io/badge/entries-83-blue)](data/ml.json)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

A curated list of the **machine learning ecosystem**: deep learning frameworks, classical ML, distributed training, MLOps and experiment tracking, model serving, feature stores, AutoML, model hubs, datasets and labeling, and model optimization.

> **Scope:** this list covers *general-purpose machine learning* tooling — frameworks, libraries, platforms, and infrastructure. LLM-agent-specific tooling (LangChain, LlamaIndex, vLLM, TRL, PEFT, Diffusers, Haystack, Sentence Transformers…) is out of scope; it lives with the [Awesome-llms-labs](https://github.com/Awesome-llms-labs) family.
> **Honesty policy:** every entry was checked against an official source (project repo, LICENSE file, or official site) as of 2026-10-01 — **83/83 verified**. Unverified entries carry a stated reason. Licenses are copied from each project's actual LICENSE file — never softened, never guessed. Proprietary SaaS products are labeled `proprietary`. Machine-readable data lives in [`data/ml.json`](data/ml.json).

## Contents

- [Deep Learning Frameworks](#deep-learning-frameworks) — 13 entries
- [Classical ML](#classical-ml) — 9 entries
- [Training & Distributed Training](#training--distributed-training) — 7 entries
- [MLOps & Experiment Tracking](#mlops--experiment-tracking) — 12 entries
- [Model Serving & Inference](#model-serving--inference) — 8 entries
- [Feature Stores](#feature-stores) — 3 entries
- [AutoML](#automl) — 5 entries
- [Model Hubs & Registries](#model-hubs--registries) — 6 entries
- [Datasets & Labeling](#datasets--labeling) — 10 entries
- [Model Optimization](#model-optimization) — 10 entries

## Choosing the right ML tool

New here? Start with the [choosing-an-ml-tool](docs/choosing-an-ml-tool.md) guide (framework picks, maintenance signals, build-vs-buy for MLOps), the [glossary](docs/glossary.md), and [status-changes](docs/status-changes.md) (renames, archival notices, license gotchas).

## Deep Learning Frameworks

Neural network libraries and autograd engines — the foundation everything else trains on. (13 entries)

- [Burn](https://burn.dev) — Deep learning framework in Rust with a JIT compiler for training and inference on any device. *(Apache-2.0 OR MIT · ⭐ 16,011)*
- [Candle](https://github.com/huggingface/candle) — Minimalist machine learning framework for Rust with a PyTorch-like API. *(Apache-2.0 OR MIT · ⭐ 21,130)*
- [Flax](https://flax.readthedocs.io) — Neural network library for JAX with composable modules and first-class pytrees. *(Apache-2.0 · ⭐ 7,334)*
- [JAX](https://docs.jax.dev) — NumPy-compatible library for accelerator-oriented array computation with composable function transformations. *(Apache-2.0 · ⭐ 36,370)*
- [Keras](https://keras.io) — Multi-backend deep learning API (JAX, TensorFlow, PyTorch) for building and training neural networks. *(Apache-2.0 · ⭐ 64,344)*
- [Ludwig](https://ludwig.ai) — Declarative deep learning framework: define models in YAML config, train on any backend. *(Apache-2.0 · ⭐ 11,772)*
- [MindSpore](https://www.mindspore.cn/en) — Huawei's all-scenario AI framework with native distributed training, optimized for Ascend processors. *(Apache-2.0)*
- [MLX](https://ml-explore.github.io/mlx/) — Apple's NumPy-like array framework for efficient machine learning on Apple silicon. *(MIT · ⭐ 28,619)*
- [ONNX](https://onnx.ai/) — Open standard for representing machine learning models, enabling framework interoperability. *(Apache-2.0 · ⭐ 21,551)*
- [PaddlePaddle](https://www.paddlepaddle.org.cn) — Baidu's open-source deep learning platform for industry-scale AI development. *(Apache-2.0 · ⭐ 24,114)*
- [PyTorch](https://pytorch.org) — The dominant open-source deep learning framework for research and production. *(BSD-3-Clause · ⭐ 103,596)*
- [TensorFlow](https://www.tensorflow.org) — End-to-end open-source platform for machine learning, from research to production. *(Apache-2.0 · ⭐ 200,650)*
- [tinygrad](https://tinygrad.org) — Minimalist deep learning framework built on a lazy tensor, with a tiny and hackable codebase. *(MIT · ⭐ 33,686)*

## Classical ML

Gradient boosting, forests, and linear models — the workhorses that still win tabular competitions. (9 entries)

- [CatBoost](https://catboost.ai) — Gradient boosting library that handles categorical features natively with strong defaults. *(Apache-2.0 · ⭐ 9,129)*
- [H2O-3](https://h2o.ai) — Open-source distributed machine learning platform for big data with AutoML. *(Apache-2.0 · ⭐ 7,509)*
- [LightGBM](https://lightgbm.readthedocs.io/en/latest/) — Gradient boosting framework designed for speed, efficiency, and distributed learning. *(MIT · ⭐ 18,825)*
- [mlpack](https://www.mlpack.org/) — Fast, header-only C++ machine learning library with an open-governance community model. *(BSD-3-Clause · ⭐ 5,712)*
- [River](https://riverml.xyz) — Online machine learning library: incremental learning on streaming data, one sample at a time. *(BSD-3-Clause · ⭐ 6,117)*
- [scikit-learn](https://scikit-learn.org) — Python library of classical machine learning algorithms with a consistent, composable API. *(BSD-3-Clause · ⭐ 67,441)*
- [statsmodels](https://www.statsmodels.org/devel/) — Python module for statistical modeling, hypothesis tests, and data exploration. *(BSD-3-Clause · ⭐ 11,668)*
- [Vowpal Wabbit](https://vowpalwabbit.org) — Fast online machine learning system for large-scale learning and reinforcement learning problems. *(BSD-3-Clause · ⭐ 8,726)*
- [XGBoost](https://xgboost.readthedocs.io/) — Optimized distributed gradient boosting library for fast, accurate tabular modeling. *(Apache-2.0 · ⭐ 28,809)*

## Training & Distributed Training

Scaling training across GPUs and nodes: parallelism strategies, orchestration, and fault tolerance. (7 entries)

- [Accelerate](https://huggingface.co/docs/accelerate) — Library that runs the same PyTorch code across any distributed configuration with minimal changes. *(Apache-2.0 · ⭐ 9,899)*
- [Colossal-AI](https://www.colossalai.org) — System for large-scale AI model training with composable parallelism strategies. *(Apache-2.0 · ⭐ 41,442)*
- [Composer](https://docs.mosaicml.com) — Library of efficient training methods and recipes for distributed deep learning. *(Apache-2.0 · ⭐ 5,505)*
- [DeepSpeed](https://www.deepspeed.ai/) — Deep learning optimization library for distributed training of very large models. *(Apache-2.0 · ⭐ 43,173)*
- [Megatron-LM](https://docs.nvidia.com/megatron-core/developer-guide/latest/get-started/quickstart.html) — NVIDIA's framework for training large transformer language models at scale. *(Apache-2.0 · ⭐ 18,048)*
- [PyTorch Lightning](https://lightning.ai) — High-level PyTorch wrapper that organizes training code and scales to distributed hardware. *(Apache-2.0 · ⭐ 31,371)*
- [Ray Train](https://www.ray.io) — Distributed deep learning library for scaling model training on the Ray compute engine. *(Apache-2.0 · ⭐ 43,959)*

## MLOps & Experiment Tracking

Experiment tracking, pipelines, and model lifecycle management — from laptop to production. (12 entries)

- [Aim](https://aimstack.io) — Open-source, self-hosted experiment tracker built to compare thousands of training runs. *(Apache-2.0 · ⭐ 6,272)*
- [ClearML](https://clear.ml) — Open-source MLOps platform for experiment tracking, orchestration, and model management. *(Apache-2.0 · ⭐ 6,897)*
- [Comet ML](https://www.comet.com) — Commercial SaaS platform for ML experiment tracking, model evaluation, and observability. *(proprietary)*
- [DVC](https://dvc.org) — Git-based version control for datasets, models, and ML experiments. *(Apache-2.0 · ⭐ 15,897)*
- [Flyte](https://flyte.org) — Workflow orchestration platform for data and ML pipelines at scale. *(Apache-2.0 · ⭐ 7,611)*
- [Kedro](https://kedro.org) — Python framework for building reproducible, maintainable data engineering and ML pipelines. *(Apache-2.0 · ⭐ 11,014)*
- [Kubeflow](https://kubeflow.org) — Kubernetes-native open-source platform for deploying and orchestrating ML workflows. *(Apache-2.0 · ⭐ 15,892)*
- [Metaflow](https://metaflow.org) — Python framework for building, scaling, and deploying real-life ML and data science workflows. *(Apache-2.0 · ⭐ 10,286)*
- [MLflow](https://mlflow.org) — Open-source platform for ML experiment tracking, model registry, and lifecycle management. *(Apache-2.0 · ⭐ 28,215)*
- [Neptune.ai](https://neptune.ai) — Commercial experiment tracker for logging and visualizing ML training metadata at scale. *(proprietary)*
- [Weights & Biases](https://wandb.ai) — Commercial SaaS platform for experiment tracking, model management, and ML observability. *(proprietary)*
- [ZenML](https://zenml.io) — Extensible MLOps framework for building reproducible, production-ready ML pipelines. *(Apache-2.0 · ⭐ 5,600)*

## Model Serving & Inference

Serving trained models behind low-latency APIs: inference servers and deployment runtimes. (8 entries)

- [BentoML](https://www.bentoml.com) — Open-source framework for building and deploying ML model inference APIs. *(Apache-2.0 · ⭐ 8,869)*
- [KServe](https://kserve.github.io/website/) — Kubernetes-native platform for serving predictive and generative ML models. *(Apache-2.0 · ⭐ 6,056)*
- [NVIDIA NIM](https://docs.nvidia.com/nim/) — Commercial containerized inference microservices packaging optimized model engines behind standard APIs. *(proprietary)*
- [NVIDIA Triton Inference Server](https://developer.nvidia.com/triton-inference-server) — High-performance inference server for deploying models from TensorFlow, PyTorch, ONNX, and more. *(BSD-3-Clause · ⭐ 11,033)*
- [OpenVINO Model Server](https://docs.openvino.ai/2026/model-server/ovms_what_is_openvino_model_server.html) — High-performance C++ inference server for models optimized with Intel OpenVINO. *(Apache-2.0 · ⭐ 940)*
- [Ray Serve](https://www.ray.io) — Scalable model-serving library for deploying online inference APIs on Ray. *(Apache-2.0 · ⭐ 43,959)*
- [Seldon Core](https://www.seldon.io) — Kubernetes-native platform for deploying, scaling, and monitoring ML models in production (v2 is source-available under BSL-1.1). *(BSL-1.1 · ⭐ 4,782)*
- [TensorFlow Serving](https://www.tensorflow.org/tfx/guide/serving) — Flexible, high-performance serving system for TensorFlow models in production. *(Apache-2.0 · ⭐ 6,364)*

## Feature Stores

Serving consistent features for training and inference — the bridge between data pipelines and models. (3 entries)

- [Feast](https://feast.dev) — Open-source feature store for serving features to ML models during training and inference. *(Apache-2.0 · ⭐ 7,319)*
- [Featureform](https://www.featureform.com) — Open-source virtual feature store for defining, managing, and serving ML features. *(MPL-2.0 · ⭐ 1,991)*
- [Hopsworks](https://www.hopsworks.ai) — Feature store and ML platform with online/offline feature serving and model management. *(AGPL-3.0 · ⭐ 1,306)*

## AutoML

Automated model selection, hyperparameter tuning, and neural architecture search. (5 entries)

- [Auto-Sklearn](https://automl.github.io/auto-sklearn/master/) — Automated ML toolkit and drop-in scikit-learn estimator using Bayesian optimization and meta-learning. *(BSD-3-Clause · ⭐ 8,134)*
- [AutoGluon](https://auto.gluon.ai) — AutoML toolkit that trains and tunes high-quality models on raw data with minimal code. *(Apache-2.0 · ⭐ 10,758)*
- [FLAML](https://microsoft.github.io/FLAML/) — Lightweight AutoML and tuning library for finding accurate models with low compute. *(MIT · ⭐ 4,400)*
- [Optuna](https://optuna.org) — Hyperparameter optimization framework with define-by-run search spaces and pruning. *(MIT · ⭐ 14,867)*
- [TPOT](https://epistasislab.github.io/tpot/) — Genetic-programming AutoML tool that optimizes ML pipelines for classification and regression. *(LGPL-3.0 · ⭐ 10,054)*

## Model Hubs & Registries

Sharing, versioning, and discovering pretrained models and model cards. (6 entries)

- [Hugging Face Hub](https://huggingface.co) — The central hub for hosting, sharing, and discovering pre-trained ML models, datasets, and demos. *(Apache-2.0 · ⭐ 3,949)*
- [ONNX Model Zoo](https://github.com/onnx/models) — A collection of pre-trained models in the ONNX format, contributed by the community. *(Apache-2.0 · ⭐ 9,814)*
- [OpenML](https://openml.org) — An open platform for sharing ML datasets, tasks, and reproducible experiment results. *(BSD-3-Clause · ⭐ 757)*
- [Papers with Code](https://paperswithcode.com) — Proprietary index owned by Hugging Face that links ML papers with their code, datasets, and benchmark results. *(proprietary)*
- [PyTorch Hub](https://pytorch.org/hub) — PyTorch's directory of published pre-trained models for research, loadable with torch.hub. *(No license file · ⭐ 1,437)*
- [Replicate](https://replicate.com) — Commercial SaaS platform for running, fine-tuning, and deploying open-source ML models via API. *(proprietary)*

## Datasets & Labeling

Dataset management, annotation tooling, and efficient data loading for training at scale. (10 entries)

- [Argilla](https://argilla.io) — Open-source collaboration tool for building and curating high-quality datasets with human feedback. *(Apache-2.0 · ⭐ 5,132)*
- [CVAT](https://www.cvat.ai) — Open-source annotation platform for images, video, 3D, and audio with model-assisted labeling. *(MIT · ⭐ 16,843)*
- [FiftyOne](https://voxel51.com) — Open-source toolkit for visualizing, curating, and evaluating computer vision datasets. *(Apache-2.0 · ⭐ 11,135)*
- [Hugging Face Datasets](https://huggingface.co/datasets) — A library and hub for accessing and sharing ready-to-use ML datasets. *(Apache-2.0 · ⭐ 22,022)*
- [Label Studio](https://labelstud.io) — Open-source multi-modal data labeling tool for images, text, audio, video, and time series. *(Apache-2.0 · ⭐ 28,388)*
- [Labelbox](https://labelbox.com) — Commercial platform for data labeling, curation, and model evaluation, widely used for frontier-model training data. *(proprietary)*
- [Roboflow](https://roboflow.com) — Commercial SaaS platform for dataset management, annotation, training, and deployment of computer vision models. *(proprietary)*
- [Supervisely](https://supervisely.com) — Commercial platform for data labeling, curation, and model training across computer vision modalities. *(proprietary)*
- [TensorFlow Datasets](https://www.tensorflow.org/datasets) — A collection of ready-to-use datasets exposed as tf.data pipelines for TensorFlow and JAX. *(Apache-2.0 · ⭐ 4,595)*
- [WebDataset](https://github.com/webdataset/webdataset) — Efficient PyTorch-style dataset loader for large-scale training from POSIX tar archives. *(BSD-3-Clause · ⭐ 3,204)*

## Model Optimization

Making models smaller and faster: quantization, pruning, compilation, and hardware-specific runtimes. (10 entries)

- [AIMET](https://qualcomm.github.io/aimet-pages/index.html) — Qualcomm's library of quantization and compression techniques for efficient on-device inference. *(BSD-3-Clause · ⭐ 2,720)*
- [Apache TVM](https://tvm.apache.org) — An open-source ML compiler framework that optimizes models for diverse hardware backends. *(Apache-2.0 · ⭐ 13,792)*
- [Brevitas](https://github.com/Xilinx/brevitas) — PyTorch library for quantization-aware training of neural networks, maintained by AMD. *(BSD-3-Clause · ⭐ 1,582)*
- [Core ML Tools](https://github.com/apple/coremltools) — Apple's toolkit for converting ML models to Core ML format for on-device inference on Apple platforms. *(BSD-3-Clause · ⭐ 5,437)*
- [ExecuTorch](https://pytorch.org/executorch) — PyTorch's on-device inference framework for deploying models on mobile and edge hardware. *(BSD-3-Clause · ⭐ 5,071)*
- [NNCF](https://github.com/openvinotoolkit/nncf) — Intel's toolkit for neural network compression via quantization, pruning, and distillation. *(Apache-2.0 · ⭐ 1,204)*
- [Olive](https://microsoft.github.io/Olive/) — Microsoft's toolkit orchestrating model optimization workflows (quantization, conversion, tuning) for ONNX Runtime. *(MIT · ⭐ 2,397)*
- [ONNX Runtime](https://onnxruntime.ai) — Cross-platform inference engine that accelerates ONNX models across CPU, GPU, and edge devices. *(MIT · ⭐ 21,976)*
- [OpenVINO](https://openvino.ai) — Intel's open-source toolkit for optimizing and deploying AI inference across Intel hardware. *(Apache-2.0 · ⭐ 10,939)*
- [TensorRT](https://developer.nvidia.com/tensorrt) — NVIDIA's SDK for high-performance deep learning inference with quantization, fusion, and kernel tuning. *(Apache-2.0 · ⭐ 13,375)*

## Notable exclusions

Candidates that were researched and deliberately left out:

| Excluded | Reason |
| --- | --- |
| MXNet | Archived by the Apache Software Foundation; last commit 2023-10-25. |
| Caffe2 | Merged into PyTorch in 2018; the standalone repo no longer exists. |
| Horovod | Archived by the maintainers (Sept 2026). |
| Shogun | Dormant — last release 2019-07-05; no active development. |
| FairScale | Dormant; its flagship feature (FSDP) was absorbed into PyTorch core. |
| Determined AI | Dormant — zero commits since 2025-03-20; OSS development stalled under HPE. |
| TorchServe | Archived by AWS (repo pytorch/serve, last push 2025-08-06). |
| Microsoft NNI | Archived 2024; Neural Network Intelligence discontinued. |
| Pachyderm | Acquired by HPE (2023), then EOLed Nov 2024. |
| Tecton | Acquired by Databricks; standalone product folded into the Databricks platform. |
| TensorFlow Hub | Discontinued as a standalone offering; tfhub.dev redirects to Kaggle Models. |
| Kaggle Datasets | A section of the Kaggle platform, not standalone ML tooling. |
| Hugging Face Optimum | Too LLM-specific; belongs to the LLM tooling family. |
| torch.compile / TorchDynamo | Covered by the PyTorch framework entry, not standalone tooling. |
| LangChain / LlamaIndex / Haystack | LLM-specific frameworks — out of scope; see the Awesome-llms-labs org. |
| vLLM / TRL / PEFT / Diffusers / Sentence Transformers | LLM-specific tooling — out of scope; see the Awesome-llms-labs org. |
| llama.cpp | LLM-specific inference tooling — out of scope. |
| Ollama | LLM-specific local inference — out of scope for general ML serving. |

## Related

More curated lists by the same author:

- [Awesome-terminal](https://github.com/dakotac1994/Awesome-terminal) — terminal emulators and the terminal stack..
- [Awesome-diagram-tool](https://github.com/dakotac1994/Awesome-diagram-tool) — diagramming and visualization tools..
- [Awesome-chrome-extension](https://github.com/dakotac1994/Awesome-chrome-extension) — Chrome/Chromium browser extensions..
- [Awesome-db](https://github.com/dakotac1994/Awesome-db) — database engines by data model..
- [Awesome-python](https://github.com/dakotac1994/Awesome-python) — the general Python ecosystem..
- [Awesome-rust](https://github.com/dakotac1994/Awesome-rust) — the Rust language ecosystem..
- [awesome-cli](https://github.com/dakotac1994/awesome-cli) — the broad CLI/TUI tools list..
- [awesome-oss-cli](https://github.com/dakotac1994/awesome-oss-cli) — the OSS-only CLI/TUI list..
- [awesome-oss-macos](https://github.com/Awesome-llms-labs/awesome-oss-macos) — open-source macOS apps..

LLM-specific ML tooling lives with the [Awesome-llms-labs](https://github.com/Awesome-llms-labs) organization.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). PRs welcome — every entry must be verified against an official source, with the license copied from the project's actual LICENSE file.
