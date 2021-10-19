# Detect Image Memorability

I used a pretrained ResNet-152 from where I eliminated the classification layer and considered the output of **pool5 layer** as features. With these features I trained a **XGBoost regressor** which predicts a real number between [0, 1]. This number represents the memorability score for an image, the most memorable images having a score close to 1 and the least memorable close to 0. To measure the performance of the model I used the **Spearman correlation** which explains how two variables being compared are monotonically related.<br/><br/>
Reproduction of the paper: ["Is Image Memorability Prediction Solved?"](https://arxiv.org/abs/1901.11420)
