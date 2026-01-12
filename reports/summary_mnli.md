# Task 1B — Fine-tuning BERT for MNLI (NLI)

Generated: 2026-01-10 11:20:49

## Setup
- Dataset: nyu-mll/glue (mnli)
- Model: bert-base-uncased
- Max length: 256
- Epochs: 3
- Learning rate: 2e-05
- Train batch size: 16
- Eval batch size: 32
- Weight decay: 0.01

## Data sizes used
- Train: 392702
- Validation (matched): 9815
- Validation (mismatched): 9832

## Results
| Split | Loss | Accuracy | Macro-F1 |
|------|------|----------|----------|
| Validation (matched) | 0.5737 | 0.8446 | 0.8443 |
| Validation (mismatched) | 0.5500 | 0.8487 | 0.8481 |
