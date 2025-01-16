# Simplified_TAG_Embedding_LLMs
## 0. Python environment setup with Conda
```
```bash
conda create --name TAPE python=3.8
conda activate TAPE
# install faster env solver
conda install -n base conda-libmamba-solver
conda config --set solver libmamba   # `conda config --set solver classic` to revert

conda install pytorch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.3 -c pytorch
conda install pytorch==1.12.1 -y
conda install torchvision==0.13.1 -y
conda install torchaudio==0.12.1 -y
# conda install cudatoolkit=11.3 -c pytorch
conda install cudatoolkit=11.3 -c pytorch
conda install -c pyg pytorch-sparse
conda install -c pyg pytorch-scatter
conda install -c pyg pytorch-cluster
@@ -39,6 +32,14 @@ pip install --upgrade accelerate

## 1. Download TAG datasets

Get (A) and (B) by running script:
- ogbn-arxiv  | `bash ogbn_arxiv_orig_download_data.sh`
- ogbn-products (subset) | NA
- arxiv_2023 | NA
- Cora | NA
- PubMed | NA
### A. Original text attributes

| Dataset | Description |