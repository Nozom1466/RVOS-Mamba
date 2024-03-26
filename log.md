`2024-3-13`
- [Mamba: Linear-Time Sequence Modeling with Selective State Spaces](https://arxiv.org/abs/2312.00752) Reading finished. Notes at [LINK](https://www.notion.so/ryan-ming/Mamba-Linear-Time-Sequence-Modeling-with-Selective-State-Spaces-e7b242b01ab145a0add7ff1a0c9796c9?pvs=4)



`2024-3-18`
- [Spectrum-guided Multi-granularity Referring Video Object Segmentation](https://arxiv.org/abs/2307.13537) Reading finished. Notes at [LINK](https://www.notion.so/ryan-ming/Spectrum-guided-Multi-granularity-Referring-Video-Object-Segmentation-4344952ce4794c68aa783b5d319da438?pvs=4)



`2024-3-24`
- Create repository
- Add README.md server_info.md
- Download RVOS-SgMg Dataset
  - `coco`: Converting file failed due to limited CPU Memory
  - `refer_youtube_vos`: Weblink expired
  - `refer_davis`: OK
  - `a2d_sentences`: Annotation file google drive link expired
  - `jhmdb_sentences`: Annotation file google drive link expired




`2024-3-26`
- New ideas:
  - Deformable Transformer Module cannot by simply replaced by Mamba because the long-range modeling ability cannot be leveraged well.
  - Inspired by [OnlineRefer: A Simple Online Baseline for Referring Video Object Segmentation](https://arxiv.org/abs/2307.09356) and [VMRNN: Integrating Vision Mamba and LSTM for Efficient and Accurate Spatiotemporal Forecasting](https://arxiv.org/abs/2403.16536), several ideas in `RVOS`:
    - Reccurent along time (frames)
    - Structure improvement: Stacked Mamba
    - Multi-modal fusion: SCF (FT)
    - Improve Mamba cell with LSTM cell mechanism (Gates)
  - Inspired by [VideoMamba: State Space Model for Efficient Video Understanding](https://arxiv.org/abs/2403.06977), ideas in `RVOS`:
    - Patch clustering
    - SCF (FT) multi-modal fusion
    - Multi-headed S6 cell
