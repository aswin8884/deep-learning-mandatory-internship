# Deep Learning Research Internship — University of Koblenz (SS 2026)

Coursework and exercise solutions from a graded research internship 
(Forschungspraktikum) at the Institute for Computer Science, 
University of Koblenz, supervised by Jennifer Wendland and 
Prof. Dr. Maik Kschischo. **Final grade: 1.0.**

The internship followed the "Dive into Deep Learning" (Zhang et al.) 
curriculum across five architecture families. This repo contains my 
worked exercise solutions, experiments, and analysis.

> Base notebooks are adapted from D2L (Zhang et al., 2023). 
> My contributions are the exercise solutions, ablation experiments, 
> and written analysis in each notebook.

## My worked solutions & experiments

**Linear/Softmax Regression**
- Zero-initialization symmetry problem analysis
- Numerical stability of softmax (exp overflow) and cross-entropy (log domain)
- Replaced MSE with Huber loss; gradient access in PyTorch

**Multilayer Perceptrons**
- Added hidden layers with tanh activation; observed effects
- Dropout at test time, dropout + weight decay interaction analysis

**Convolutional Neural Networks**
- Edge detection with custom kernels + Sobel operator
- Output-shape math for padding/strides; max vs average pooling in LeNet
- Batch norm: bias removal, per-layer necessity, dropout+BN combination

**Recurrent Neural Networks**
- Tokenization methods and vocab-size effects
- Gradient clipping ablation (what happens without it)
- Empirical runtime/perplexity comparison: RNN vs GRU vs LSTM (hidden dim 256)
