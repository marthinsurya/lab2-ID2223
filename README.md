#Improving Model Performance
1. Model-Centric Approach:
    - Tune training parameters especially Training parameters. Slow training is important to reach max peformance which was not done due to time constrain. One we focus on is warmup and learning rate among others
    - Model choice should try to avoid bnb-4bit due to incompatibility issue with many platform deployment, but this module is focussing on efficient training with 4bit. Hence, the choice of model
    - Depending on the purpose, choosing pre-trained instruct model can be counter productive. Especially for training purpose since the improvement could be negligible for short period
2. Data-Centric Approach:
    - Depending on the purpose, different data set can serve a better fine tuning dataset for the model. In our case, as example, we use FineTome-100k dataset which is focusing in educational content. Other data set can be proven to be more useful for specific purpose.
    - Data also was splitted to train, evaluation and testing dataset to measure training performance. Choosing dataset with pre-split definition can be helpful. We use evaluation and test set to measure performance
    
