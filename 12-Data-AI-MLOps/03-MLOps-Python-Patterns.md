# 03 — Python Patterns for MLOps / AI Platforms

MLOps me sirf model training nahi; reliable software practices bhi important hain.

## 1. Config Outside Code
```python
import os
MODEL_PATH = os.getenv("MODEL_PATH", "models/model.pkl")
```

## 2. Typed Input
```python
def predict(features: list[float]) -> float:
    ...
```

## 3. Separate Responsibilities
```text
data loading
feature transform
model loading
prediction
API serving
logging/metrics
```

## 4. Model Load Once
Long-running service me har request par model reload avoid karo unless design requires it.

```python
class ModelService:
    def __init__(self, model):
        self.model = model

    def predict(self, features):
        return self.model.predict([features])[0]
```

## 5. Validate Inputs
Missing/wrong feature types handle karo before model call.

## 6. Observability
Log:
- request/result metadata (non-sensitive)
- latency
- errors
- model version

## 7. Reproducibility
Dependency versions, model version, config, code revision track karo.

## 8. Tests
Test preprocessing, edge cases, API behavior, model wrapper.

## AI Platform Mindset
Model ko production service ki tarah treat karo: secure, observable, testable, repeatable.
