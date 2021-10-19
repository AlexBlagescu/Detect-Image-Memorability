# Detect Image Memorability

I used a pretrained ResNet-152 from where I eliminated the classification layer and considered the output of pool5 layer as features. With these features I trained a XGBoost regressor which predicts a real number between [0, 1].
Reproduction of the paper ["Is Image Memorability Prediction Solved?"](https://arxiv.org/abs/1901.11420)
