# Cortex Compliance AI

Fine-tuned LLM for Russian compliance document generation (152-ФЗ, 187-ФЗ, ГОСТ 57580, ФСТЭК).

## Open in Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/maanisingh/cortex-compliance-ai/blob/main/cortex_compliance_finetuning.ipynb)

**Click the badge above to start training!**

## What This Does

1. Fine-tunes Mistral-7B on Russian compliance documents
2. Uses LoRA for efficient training (works on free GPU)
3. Uploads trained model to HuggingFace

## Quick Start

1. Click "Open in Colab" badge above
2. Runtime → Change runtime type → **T4 GPU**
3. Runtime → Run all
4. Wait ~30 minutes for training
5. Model available at: `cortexgrc/cortex-compliance-ai`

## Training Data

8 Russian compliance document templates:
- Personal Data Policy (Политика обработки ПДн)
- Consent Form (Согласие на обработку)
- ISPDN Description (Описание ИСПДн)
- Roskomnadzor Notification (Уведомление в РКН)
- DPO Appointment Order (Приказ о назначении)
- KII Categorization Act (Акт категорирования КИИ)
- Bank Security Policy (Политика ИБ банка)
- УЗ-3 Protection Level Explanation

## Files

- `cortex_compliance_finetuning.ipynb` - Training notebook
- `compliance_training.jsonl` - Training data

## License

Proprietary - Cortex GRC
