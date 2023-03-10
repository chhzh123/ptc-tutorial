# PyTorch Compilation Tutorial

This tutorial is designed for ECE6980 Spring 2023 @ Cornell. It covers the basic compilation techniques in the PyTorch ecosystem.

1. Basic [PyTorch](https://pytorch.org/)
    * Hierarchical module construction
2. [TorchScript](https://pytorch.org/docs/stable/jit.html)
    * Tracing mode
    * Scripting mode
3. [torch.fx](https://pytorch.org/docs/stable/fx.html)
    * Symbolic trace
    * Intermediate representation (IR)
    * Graph traversal and manipulation
    * limitation
4. [slapo](https://github.com/awslabs/slapo)
    * Progressive optimization (manual + compiler optimization)
    * Subgraph matching
    * Operator fusion
    * Module replacement
    * Quantization (optional)
5. [PyTorch 2.0](https://pytorch.org/get-started/pytorch-2.0/) (optional)


## Set up environment
Please use a clean environment and install the following package.

```bash
pip3 install torch==1.13.0+cu117 torchvision==0.14.0+cu117 slapo
```


## Reading materials

### Paper
* Adam Paszke et al., [*PyTorch: An Imperative Style, High-Performance Deep Learning Library*](https://arxiv.org/abs/1912.01703), NeurIPS, 2019.
* James K. Reed et al., [*Torch.fx: Practical Program Capture and Transformation for Deep Learning in Python*](https://arxiv.org/abs/2112.08429), MLSys, 2022.
* Hongzheng Chen et al., [*Decoupled Model Schedule for Deep Learning Training*](https://arxiv.org/abs/2302.08005), arXiv:2302.08005, 2023.

### Blogs
* Yuxin Wu, [TorchScript: Tracing vs. Scripting](https://ppwwyyxx.com/blog/2022/TorchScript-Tracing-vs-Scripting/)
