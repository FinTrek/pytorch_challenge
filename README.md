# pytorch_challenge
This repository contains the models that I built for the flower classification challenge in the Pytorch Challenge.

## model_initial
Built a Resnet152 model which showed average performance. (Approx 30% validation accuracy)

## model_final
Improved the Resnet152 model by making changes in -
1. Parameters in hidden layer (reduced 1024 to 512)
2. Increased batch_size from 32 to 64
3. Changed the final accuracy calculation method. 
(Insted of calculating the max value, used the topk method in torch along with finding exponential of the final value)
This model had validation accuracy of over 95%.

Other parameters such as the Optimiser(Adam), Criterion(NLLLoss), Scheduler(StepLR), were kept same for both.
