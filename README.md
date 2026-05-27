# stPMVG
Code for A Pseudo-Label Multi-View Graph Contrastive Learning Framework for Identifying Spatial Domains 
<p align="center">
  <img src="model.png" width="85%" alt="stPMVG Framework"/>
</p>



## Requirements

- Python 3.10
- CUDA 12.1 (recommended for GPU acceleration)

### Environment Setup

We recommend using [Anaconda](https://www.anaconda.com/) to manage the environment.

**Step 1: Create and activate a conda environment**

```bash
conda create -n stpmvg python=3.10
conda activate stpmvg
```

**Step 2: Install PyTorch with CUDA support**

```bash
conda install pytorch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 pytorch-cuda=12.1 -c pytorch -c nvidia
```

> If you do not have a GPU, install the CPU-only version:
> ```bash
> conda install pytorch==2.2.2 torchvision==0.17.2 torchaudio==2.2.2 cpuonly -c pytorch
> ```

**Step 3: Install PyTorch Geometric (PyG)**

```bash
pip install torch_geometric
pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.2.0+cu121.html
```

**Step 4: Install remaining dependencies**

```bash
pip install anndata==0.9.1 \
            byol-pytorch==0.6.0 \
            matplotlib==3.7.1 \
            opencv-python==4.7.0.72 \
            pandas==2.0.1 \
            pot==0.9.0 \
            pyyaml==6.0 \
            rpy2==3.5.11 \
            scanpy==1.9.3 \
            scikit-misc==0.2.0 \
            seaborn==0.12.2 \
            umap-learn==0.5.3 \
            numpy==1.24.3 \
            scikit-learn==1.2.2 \
            scipy==1.10.1 \
            h5py==3.8.0 \
            tqdm==4.65.0 \
            threadpoolctl==3.4.0 \
            harmonypy \
            anndata2ri \
            PyWGCNA \
            spatialde \
            notebook
```
## Data Preparation

Place the raw spatial transcriptomics data (e.g., DLPFC) in the folder Dataset.


---

## Usage

**Model Training and Testing**

```bash
Run stPMVG/example/run_DLPFC.ipynb to train and test the stPMVG model:
```
