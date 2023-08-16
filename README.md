# GeoPythonWorkshop2023_SSL
This repository contains the codes for the [GeoPython Workshop](https://2023.geopython.net/talks.html#workshops) held in Basel, Switzerland on March 2023.

With the help of current semi-supervised learning algorithms, we can classify aerial scenes using 4, 20, or 40 labeled examples per class and still obtain similar accuracies as training with numerous labeled examples. With this workshop, we want to show the semi-supervised learning algorithms currently available and how to use the repositories available for scene classification.

During the workshop, we’ll go through the strategic use of git to get the repository, an explanation of the usage of the code, setting up the environment, and the training of the algorithm. We’ll finalize the workshop with the implementation of the best model for scene classification with semi-supervised learning.

## Example
To check the training results using CoMatch on UCM with 4 labeled examples per class, download the compressed file "example_comatch_ucm_wrn_b1x8_l4". It contains the configuration file (.py), the log file of the training (.log), and the best model (.pth) for this model using a batch size of 8 on a single GPU.

To train the model, we executed the following command in the terminal:

```bash
CUDA_VISIBLE_DEVICES=0 python3 train_semi.py --cfg ./configs/4_perclass/comatch/comatch_ucm_wrn_b1x8_l4.py --out ./results/4_perclass/comatch/comatch_ucm_wrn_b1x8_l4 --seed 5




