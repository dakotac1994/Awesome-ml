# Glossary

Terms you'll meet across the [Awesome-ml](../README.md) catalog.

- **Autograd** — automatic differentiation: the engine (PyTorch, JAX, TensorFlow) that computes gradients for backpropagation.
- **DDP (DistributedDataParallel)** — PyTorch's data-parallel training: each GPU holds a full model replica and gradients are averaged across workers.
- **FSDP (Fully Sharded Data Parallel)** — shards model parameters, gradients, and optimizer state across GPUs so models larger than one GPU's memory can train.
- **ZeRO** — DeepSpeed's memory-optimization stages that progressively shard optimizer state, gradients, and parameters.
- **Quantization** — reducing numeric precision (e.g. FP32 → INT8) to shrink models and speed inference, with small accuracy trade-offs.
- **Pruning** — removing unimportant weights or neurons to compress a model.
- **Knowledge distillation** — training a small "student" model to mimic a large "teacher" model.
- **ONNX (Open Neural Network Exchange)** — an open format for representing ML models so they can move between frameworks and runtimes.
- **Inference server** — a service that loads a trained model and serves predictions over an API (Triton, BentoML, KServe).
- **Feature store** — a system that serves consistent feature values for both training and inference, avoiding train/serve skew.
- **Experiment tracking** — logging hyperparameters, metrics, and artifacts per training run so runs are comparable and reproducible (MLflow, Aim, W&B).
- **MLOps** — the practices and tooling for deploying, monitoring, and maintaining ML models in production.
- **AutoML** — automating model selection, hyperparameter tuning, and sometimes feature engineering.
- **NAS (Neural Architecture Search)** — automatically discovering neural network architectures rather than hand-designing them.
- **Model registry** — a versioned store of trained models with metadata, lineage, and stage transitions (staging → production).
- **Data labeling / annotation** — producing ground-truth labels for training data (bounding boxes, segmentations, text spans) via tools like CVAT or Label Studio.
- **Train/serve skew** — when the features or data distribution at serving time differ from training time, silently degrading model quality.
- **Drift** — change over time in input data (data drift) or in the input→output relationship (concept drift) that erodes a deployed model's accuracy.
