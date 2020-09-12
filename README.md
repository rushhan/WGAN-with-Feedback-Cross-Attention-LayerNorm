# WGAN-with-Feedback-Cross-Attention-LayerNorm
WGAN with feedback from discriminator&amp; LayerNorm instead of BatchNorm


## Modifications to the original WGAN implementation:
1. Added feedback from the discriminator in the form of attention
2.Modified BN to LayerNorm as BatchNorm creates correlation between the examples.
Note that the results from LayerNorm were not promising

## Execute
python main.py --dataset lsun --dataroot /workspace/lsun --cuda --clamp --fdbac--save_dir sample

## Notes
Need the lsun data.
Follow the instruction in original implementation [link](https://github.com/martinarjovsky/WassersteinGAN)

## Sources
WGAN Model based on original paper [link](https://arxiv.org/abs/1701.07875).

Cross Attention is my own implementation


## To-Do
Rerun and recheck the results
