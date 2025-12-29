# Cortex Compliance AI - Training Dataset

Fine-tuned LLM for Russian business document generation.

## Open in Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/maanisingh/cortex-compliance-ai/blob/main/cortex_compliance_finetuning.ipynb)

**Click the badge above to start training!**

## Dataset Statistics

| Metric | Value |
|--------|-------|
| **Total Training Examples** | 217 |
| **Source Templates** | 265 |
| **Categories** | 8 |
| **Language** | Russian |

### Categories Breakdown

| Category | Examples | Description |
|----------|----------|-------------|
| Contracts | 26 | Service, Sales, NDA, Partnership |
| Corporate | 12 | Charters, Protocols, Resolutions |
| Financial | 11 | Invoices, Acts, Reports |
| HR | 12 | Employment, Orders, Policies |
| Industry | 14 | Sector-specific documents |
| Legal | 10 | IP, Licensing, Claims |
| Specialized | 14 | Real Estate, Banking, Gov |
| Tax | 12 | Declarations, Reports |
| SME Templates | 98 | Small Business Documents |
| Compliance | 8 | 152-FZ, 187-FZ, GOST |

## Quick Start

1. Click "Open in Colab" badge above
2. Runtime → Change runtime type → **T4 GPU**
3. Runtime → Run all
4. Wait ~30-45 minutes for training
5. Model uploads to: `maaninder/cortex-compliance-ai`

## Files

- `combined_training_data.jsonl` - **Full dataset (217 examples)**
- `cortex_compliance_finetuning.ipynb` - Training notebook
- `sme_training_data.jsonl` - SME subset (98 examples)
- `compliance_training.jsonl` - Compliance subset (8 examples)

## Training Configuration

- **Base Model**: Mistral-7B-v0.1
- **Method**: QLoRA (4-bit quantization)
- **LoRA Rank**: 16
- **Epochs**: 3
- **GPU Required**: T4 or better

## Integration

Trained model is used by CORTEX AI platform:
- Live: https://cortex.alexandratechlab.com
- Model: https://huggingface.co/maaninder/cortex-compliance-ai

## License

MIT License - Cortex AI
