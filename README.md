# Hi, I'm Pierre-Antoine 👋

Machine learning for biology. Currently interested in virtual tissue models and perturbation modelling from spatial omics. Previously Senior Data Scientist at [Owkin](https://www.owkin.com) (2022–2026), where I shipped deep-learning models for pathology into pharma-facing studies and first-authored papers in *Nature Communications* and *Histopathology*. Before that, sparse optimization research at Inria.

I like writing fast, portable code for ML and biology: C/C++ inference engines, Rust servers for gigapixel images, and GPU kernels.

🌐 [pab.me](https://pab.me) · 🎓 [Google Scholar](https://scholar.google.com/citations?user=77JN6OcAAAAJ) · 🐦 [@el_pa_b](https://x.com/el_pa_b)

## Things I built

### Portable ML inference (C/C++, ggml)
| Repo | What it does |
|---|---|
| [bark.cpp](https://github.com/PABannier/bark.cpp) ⭐ 870+ | Suno's Bark text-to-speech in plain C/C++ with CUDA and Metal kernels. ~10× faster than the reference implementation. |
| [sam3.cpp](https://github.com/PABannier/sam3.cpp) ⭐ 370+ | State-of-the-art image and video segmentation (SAM 3) in portable C/C++. |
| [encodec.cpp](https://github.com/PABannier/encodec.cpp) ⭐ 230+ | Meta's EnCodec neural audio codec, compression and generation, without Python. |
| [biogpt.cpp](https://github.com/PABannier/biogpt.cpp) ⭐ 85+ | Microsoft's BioGPT running on ggml. |
| [rust-ggml](https://github.com/PABannier/rust-ggml) | Rust bindings for ggml. |

### Digital pathology & spatial omics infrastructure (Rust, C++)
| Repo | What it does |
|---|---|
| [WSIStreamer](https://github.com/PABannier/WSIStreamer) ⭐ 180+ | Tile server for whole-slide images stored in S3-compatible object storage. |
| [PathCollab](https://github.com/PABannier/PathCollab) ⭐ 30+ | Self-hosted collaborative slide viewer with real-time cursor presence and overlays. |
| [fovea](https://github.com/PABannier/fovea) | Streams only the slide tiles, cell chunks and heatmap tiles the viewport needs, for smooth pan/zoom over millions of cells. |
| [PathView](https://github.com/PABannier/PathView) | GPU-accelerated whole-slide viewer with polygon overlays and an MCP server so AI agents can drive it. |
| [spacexrfast](https://github.com/PABannier/spacexrfast) | Parallel R/C++ backend for RCTD spatial cell typing. Up to 15× faster on Xenium, identical calls. |
| [HistoAtlas](https://github.com/HistoAtlas/HistoAtlas) | Pan-cancer morphology atlas linking histomics to molecular programs and clinical outcomes ([preprint](https://arxiv.org/abs/2603.16587)). |
| [fgfr3mut](https://github.com/PABannier/fgfr3mut) | Code for the *Nature Communications* FGFR3 pre-screening paper. |

### Optimization & systems
| Repo | What it does |
|---|---|
| [sparseglm](https://github.com/PABannier/sparseglm) | Fast, modular sparse GLM solver in Rust. |
| [nanograd](https://github.com/PABannier/nanograd) ⭐ 35 | Torch-like autograd framework on NumPy arrays. |
| [nanokv](https://github.com/PABannier/nanokv) ⭐ 27 | Distributed key-value store in ~1,000 lines of Rust. |
| [sinkhorn-swift](https://github.com/PABannier/sinkhorn-swift) | 11 mask-interpolation methods (optical flow, Sinkhorn OT, Metal shaders) benchmarked for on-device video segmentation on Apple Silicon. |
| [simdcsv](https://github.com/PABannier/simdcsv) | Parsing gigabytes of CSV per second. |

## Open-source contributions

- **[skglm](https://github.com/scikit-learn-contrib/skglm)** — core developer. FISTA, non-convex penalties, Poisson/Gamma datafits, working-set improvements. Co-author of the [NeurIPS 2022](https://proceedings.neurips.cc/paper_files/paper/2022/hash/fe5c31e525e9a26a1426ab0b589f42fe-Abstract-Conference.html) and [JMLR](https://www.jmlr.org/papers/v26/24-0008.html) papers.
- **[HistoPLUS](https://github.com/owkin/histoplus)** — technical lead. Cell detection, segmentation and classification on H&E, scaled to 1B+ cells ([paper](https://doi.org/10.1016/j.jpi.2026.100696)).
- **[ggml](https://github.com/ggml-org/ggml)** — tensor operations and CPU/Metal kernels.
- **[MNE-Python](https://github.com/mne-tools/mne-python)** — SURE-based regularization selection for M/EEG source imaging, faster block-coordinate descent, source visualization.
- **[Benchopt](https://github.com/benchopt/benchopt)** — Lasso and L1 logistic regression benchmarks ([NeurIPS 2022](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a30769d9b62c9b94b72e21e0ca73f338-Abstract-Conference.html)).
- Smaller patches to [scikit-learn](https://github.com/scikit-learn/scikit-learn/pull/24843), [Numba](https://github.com/numba/numba/pull/7976) and [linfa](https://github.com/rust-ml/linfa/pull/194).

## Selected publications

- **AI allows pre-screening of FGFR3 mutational status using routine histology slides of muscle-invasive bladder cancer.** *Nature Communications*, 2024. First author. [doi](https://doi.org/10.1038/s41467-024-55331-6)
- **Development of a deep-learning model tailored for HER2 detection in breast cancer.** *Histopathology*, 2024. First author. [doi](https://doi.org/10.1111/his.15274)
- **Beyond L1: Faster and Better Sparse Models with skglm.** *NeurIPS*, 2022. [link](https://proceedings.neurips.cc/paper_files/paper/2022/hash/fe5c31e525e9a26a1426ab0b589f42fe-Abstract-Conference.html)
- **Toward comprehensive cellular characterization of H&E slides.** *Journal of Pathology Informatics*, 2026. [doi](https://doi.org/10.1016/j.jpi.2026.100696)

## What I'm interested in

- Virtual tissue models and perturbation modelling from spatial omics
- Computational pathology and foundation models for histology
- Optimal transport and sparse optimization
- Making ML models run fast on whatever hardware is in front of me: C/C++, Rust, CUDA, Metal
