# Methodology and limitations

## Review design

This project is a critical review of the deep-learning NIDS survey by Anis et al. (2025), supplemented by six related surveys and selected foundational references. The review organizes the surveyed systems into four broad families:

1. reconstructive and generative models;
2. Transformer-based models;
3. convolutional and feed-forward models; and
4. hybrid and federated models.

The analysis compares the assumptions, datasets, reported metrics, deployment constraints, and evidence gaps associated with these families. Dataset-use counts and model results are taken from the source survey and from the course report's synthesis of that survey.

## Evidence boundaries

- The project did not rerun the 31 primary studies.
- It did not conduct an independent database search or PRISMA screening process.
- Reported accuracy, F1, AUC, latency, and transfer results should be read as literature-reported values, not independently reproduced measurements.
- The representative evidence matrix is a structured selection of systems discussed in the report. It is not a complete extraction of every paper in the survey.
- The proposed two-tier SOC architecture is a reasoned deployment interpretation. It was not implemented, load-tested, or validated against live enterprise traffic.

## Critical interpretation rules

The review applies four checks to prominent claims:

1. **Evaluation context:** distinguish within-dataset scores from cross-dataset evidence.
2. **Operational context:** look for latency, throughput, memory, hardware, false-positive, and encrypted-traffic measurements.
3. **Security context:** identify adversarial evaluation, privacy leakage, and model-update risks.
4. **Methodological context:** separate findings supported by explicit search and selection methods from narrative coverage.

## Corrections in the public edition

The public portfolio edition qualifies several statements from the original course files:

- Federated learning is described as reducing raw-data centralization, not as proof of GDPR or HIPAA compliance.
- Federated learning is presented as one architectural option where traffic centralization is restricted, rather than the only viable option.
- The adversarial-robustness finding acknowledges isolated adversarial studies while retaining the broader criticism that no unified benchmark or systematic defense comparison is available.
- Student registration numbers and personal authoring metadata were removed.

## Reproducibility status

The repository is reproducible as a literature-analysis artifact: the report, slides, selected evidence matrix, references, and explicit limitations are included. Reproducing the underlying model results would require the primary papers, datasets, preprocessing pipelines, training code, hardware details, and random seeds, which are outside this repository's scope.

