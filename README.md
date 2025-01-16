# Simplified_TAG_Embedding_LLMs

## 0. Python Environment Setup with Conda

```bash
# Create and activate environment
conda create --name TAPE python=3.8
conda activate TAPE

# Install faster environment solver
conda install -n base conda-libmamba-solver
conda config --set solver libmamba   # Use 'conda config --set solver classic' to revert

# Install PyTorch and related packages
conda install pytorch==1.12.1 torchvision==0.13.1 torchaudio==0.12.1 cudatoolkit=11.3 -c pytorch

# Install PyG (PyTorch Geometric) packages
conda install -c pyg pytorch-sparse
conda install -c pyg pytorch-scatter
conda install -c pyg pytorch-cluster

# Additional packages
pip install --upgrade accelerate