# Status Changes

Notable renames, archival notices, dormancy, and license gotchas affecting entries in this list. Last reviewed 2026-10-01.

## Archival notices (excluded from the catalog)

- **MXNet** — archived by the Apache Software Foundation; last commit 2023-10-25.
- **Horovod** — archived by the maintainers (Sept 2026).
- **Caffe2** — merged into PyTorch in 2018; the standalone repo no longer exists.
- **TorchServe** — archived by AWS (repo `pytorch/serve`, last push 2025-08-06).
- **Microsoft NNI** — archived 2024; Neural Network Intelligence discontinued.
- **Pachyderm** — acquired by HPE (2023), EOLed Nov 2024.

## Dormant (not archived, but effectively unmaintained — excluded)

- **Shogun** — last release 2019-07-05.
- **FairScale** — dormant; its flagship feature (FSDP) was absorbed into PyTorch core.
- **Determined AI** — zero commits since 2025-03-20; OSS development stalled under HPE.

## Discontinued as standalone offerings (excluded)

- **TensorFlow Hub** — tfhub.dev now redirects to Kaggle Models ("integrated with Kaggle Models").
- **Tecton** — acquired by Databricks; tecton.ai redirects to databricks.com.

## Renames / moves

- **Burn: `tracetechnical/burn` → `tracel-ai/burn`** — the repo moved orgs; entries use the canonical new path.
- **Featureform** — acquired by Redis (Oct 2025); the OSS repo remains active and the entry is kept.

## License gotchas recorded at verification (2026-10-01)

- **Hopsworks is AGPL-3.0**, not Apache-2.0 as commonly assumed.
- **Seldon Core v2 is BSL-1.1** (source-available); labeled BSL-1.1 in the catalog.
- **PyTorch Hub's repo has no license file** — recorded verbatim as "No license file".
- **CVAT is MIT**, with copyright handed off from Intel to CVAT.ai.
- **mlpack's LICENSE.txt** carries a custom preamble but grants BSD-3-Clause; labeled BSD-3-Clause.
- **scikit-learn's license** lives in `COPYING`, not `LICENSE`; it is BSD-3-Clause.
- **Proprietary SaaS in the catalog** (labeled `proprietary`): Weights & Biases, Neptune.ai, Comet ML, Replicate, Papers with Code, Roboflow, Supervisely, Labelbox, NVIDIA NIM.
