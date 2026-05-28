 # CogPortrait: Fine-Grained Eye-Region Control in Portrait Animation via Hierarchical Agent Planning

[![arXiv](https://img.shields.io/badge/arXiv-2605.28056-b31b1b.svg)](https://arxiv.org/abs/2605.28056)
[![Project Page](https://img.shields.io/badge/Project-Page-blue)](https://fenghe12.github.io/cogportrait-io/)

**He Feng**<sup>1</sup>, **Yongjia Ma**<sup>2</sup>, **Donglin Di**<sup>2</sup>, **Lei Fan**<sup>3,&dagger;</sup>, **Tonghua Su**<sup>1,&dagger;</sup>

<sup>1</sup> Harbin Institute of Technology &nbsp; <sup>2</sup> Li Auto &nbsp; <sup>3</sup> University of New South Wales  
<sup>&dagger;</sup> Corresponding authors

---

## Overview

CogPortrait is a two-stage framework that generates portrait animations with fine-grained eye-region control from high-level labels. In the first stage, three chain-of-thought MLLM agents compile labels into facial keypoints through temporal event planning, prototype retrieval from a real-behavior library, and semantic-physiological constraint enforcement. In the second stage, a DiT-based video generation backbone synthesizes the final animation conditioned on the keypoints, reference portrait, audio, and text prompt, enhanced by dynamic CFG with eye-region-aware reweighting and KTO-based refinement for boundary cases.

## Key Contributions

- **Hierarchical Agent Planning**: Three CoT MLLM agents (planning, composition, critic) translate abstract labels into physiologically plausible facial keypoints
- **Dynamic CFG & KTO Refinement**: Eye-region-aware reweighting eliminates global color shift; KTO handles long-tail boundary cases (asymmetric eyebrows, large-angle head poses)
- **EMH Benchmark**: 12 categories (6 core emotions + 6 beyond-emotion states) with AU-F1 and AU-Temp metrics for evaluating fine-grained eye-region and head-motion control

## Project Page

Visit **[https://fenghe12.github.io/cogportrait-io/](https://fenghe12.github.io/cogportrait-io/)** for demos, results, and more details.

## Citation

```bibtex
@misc{feng2026cogportrait,
    title={CogPortrait: Fine-Grained Eye-Region Control in Portrait Animation via Hierarchical Agent Planning},
    author={He Feng and Yongjia Ma and Donglin Di and Lei Fan and Tonghua Su},
    year={2026},
    eprint={2605.28056},
    archivePrefix={arXiv},
    primaryClass={cs.CV}
}
```

## License

Code will be released upon publication.
