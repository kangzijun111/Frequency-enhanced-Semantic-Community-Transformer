# FreqCoT: Frequency-enhanced Semantic Community Modeling for Spatiotemporal Forecasting

[![Paper](https://img.shields.io/badge/Paper-Under--Review-orange.svg)]()
[![Code Status](https://img.shields.io/badge/Code-Coming--Soon-blue.svg)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

This repository is the official PyTorch implementation of **FreqCoT**, a frequency-enhanced semantic community transformer for traffic forecasting.

> **Frequency-enhanced Semantic Community Modeling for Spatiotemporal Forecasting**  
> *Under Review (2026)*

FreqCoT organizes traffic nodes into **semantic communities** using frequency-domain descriptors, and models global interactions through **hierarchical community tokens** (HD-CoTAR). By restricting global attention to a small set of community tokens, it captures long-range dependencies beyond spatial proximity while keeping inference latency competitive with lightweight GNN baselines.

---

## 📢 Release Status & Roadmap

The codebase is currently undergoing final cleanup, documentation, and licensing reviews. We are actively preparing the full repository for public release.

- [x] Paper submitted
- [ ] Environment setup & dependencies (`requirements.txt`)
- [ ] Data preprocessing scripts for 6 traffic benchmarks
- [ ] Core model architecture (`FreqCoT` & `HD-CoTAR`)
- [ ] Training configs & checkpoint release

> 💡 **Notice**: The complete training/evaluation code and configuration files will be released upon paper acceptance (or within the coming weeks). Please star or watch this repository to stay updated!

---


## 📊 Supported Datasets (Coming Soon)

We provide evaluation scripts and data preprocessing pipelines for 6 standard spatial-temporal benchmarks:

- **Traffic Flow**: PEMS03, PEMS04, PEMS07, PEMS08
- **Traffic Speed**: METR-LA, PEMS-BAY

Download links and processing instructions will be made available upon code release.

---

## 🛠️ Usage Preview

Once released, you will be able to run experiments via configuration files:

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Train model on a specific benchmark
python main.py --config config/PEMS04.conf
