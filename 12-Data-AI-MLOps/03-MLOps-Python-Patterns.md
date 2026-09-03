# MLOps-Oriented Python Patterns

MLOps code should be reproducible, configurable, testable, and observable.

## Configuration-Driven Code
```python
from dataclasses import dataclass

@dataclass
class TrainConfig:
    learning_rate: float
    epochs: int
    model_name: str
```

Avoid scattering constants across files.

## Separate Pipeline Stages
```text
data ingestion
→ validation
→ preprocessing
→ training
→ evaluation
→ packaging
→ deployment
→ monitoring
```

## Reproducibility
Record:
- package versions
- dataset/version identifiers
- model parameters
- metrics
- code commit

## Logging and Errors
Use structured logs and fail clearly when data is invalid.

## Cloud Pattern
Keep AWS-specific code behind small functions or service classes so business logic remains testable.

## Company Use
Training pipelines, model serving, batch inference, feature workflows, platform automation.

## Interview Questions
1. What makes an ML workflow reproducible?
2. Why separate configuration from code?
3. Why track model and data versions?