# S-DPQ Reference Implementation

This repository contains the code to reproduce the results in the paper **"S-DPQ: Block-Level Angular and Norm Matching for Data-Free Ternary Quantization"**.

## How to Run (Google Colab)
1. Upload `main.ipynb` to Google Colab.
2. Select **T4 GPU** runtime (`Runtime` -> `Change runtime type`).
3. Click **Runtime** -> **Run All**.

## Licensing and Assets

This repository provides the reference implementation and does not redistribute any pretrained model checkpoints or raw benchmark datasets. The code in this repository is released under the license specified in the `LICENSE` file.

The `distilbert/distilbert-base-uncased-finetuned-sst-2-english` checkpoint explicitly declares the Apache-2.0 license in its model card. However, the `textattack/distilbert-base-uncased-MRPC` repository does not state an explicit license in its public model card; therefore, this repository does not independently characterize or redistribute that fine-tuned checkpoint as Apache-2.0.

The `roberta-large` architecture is originally MIT-licensed. However, the public pages reviewed for `siebert/sentiment-roberta-large-english` and `howey/roberta-large-mrpc` do not explicitly declare MIT for the fine-tuned checkpoints themselves. Accordingly, this repository does not redistribute those checkpoint files. Users who obtain them independently via the Hugging Face API are responsible for reviewing and complying with the licenses, attribution requirements, and any additional terms supplied by the respective maintainers.

The evaluation datasets are loaded via the Hugging Face `datasets` library using the `SetFit/sst2` and `SetFit/mrpc` distributions. These are derived from the original Stanford Sentiment Treebank and Microsoft Research Paraphrase Corpus, respectively, and are not redistributed with this repository. Users should use them in accordance with their original academic terms: the **Stanford NLP custom research license** for SST-2, and the **Microsoft Research Data License Agreement (MSR-DLA)** for MRPC. The Hugging Face `transformers` and `datasets` libraries are external dependencies distributed under the Apache-2.0 license.

### Asset references (As utilized in the code)

- DistilBERT SST-2 checkpoint: <https://huggingface.co/distilbert/distilbert-base-uncased-finetuned-sst-2-english>
- TextAttack DistilBERT MRPC checkpoint: <https://huggingface.co/textattack/distilbert-base-uncased-MRPC>
- SiEBERT sentiment checkpoint: <https://huggingface.co/siebert/sentiment-roberta-large-english>
- RoBERTa-large MRPC checkpoint: <https://huggingface.co/howey/roberta-large-mrpc>
- SST-2 Dataset (SetFit distribution): <https://huggingface.co/datasets/SetFit/sst2>
- MRPC Dataset (SetFit distribution): <https://huggingface.co/datasets/SetFit/mrpc>
- Hugging Face Transformers license: <https://github.com/huggingface/transformers/blob/main/LICENSE>
