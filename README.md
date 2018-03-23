# pix2code (PyTorch)

This repo holds a basic PyTorch implementation of [pix2code](https://github.com/tonybeltramelli/pix2code) — a deep learning model that transforms GUI screenshots into code (in this case, a DSL based on Bootstrap).

## Instructions

This isn't ready for general usage yet. However, look at `pix2code (alpha).ipynb` for the following:

- Custom PyTorch dataloader (based on [pix2code web dataset](https://github.com/tonybeltramelli/pix2code/tree/master/datasets))
- Encoder/Decoder models
- Testing Code (includes finding BLEU values for multiple pretrained models)

I've also included [pretrained weights after 100 and 1000 epochs of training](https://github.com/andrewsoohwanlee/pix2code-pytorch/releases/tag/v0.1-alpha).

## Results

Early results have been generally successful in terms of BLEU scores, with our max at ~0.92 after 100 epochs of training (the model started generally overfitting to the training data after that point).

| Epochs  | BLEU |
| ------------- | ------------- |
| 100 | 0.924819024813575 |
| 200 | 0.8959682936793072 |
| 300 | 0.920018035108614 |
| 400 | 0.9033686688876422 |
| 500 | 0.9191831702256483 |
| 600 | 0.8876589013117365 |
| 700 | 0.9098200684974314 |
| 800 | 0.9164715424716915 |
| 900 | 0.919587909269687 |
| 1000 | 0.8644991775415475 |

---

— [Andrew](https://andrewlee.design/)
