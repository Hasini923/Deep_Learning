### Experiment 5 – CNN Training, Regularization, Optimization, Hyperparameter Tuning, Transfer Learning & Cross-Validation

Studied CNN training using MobileNetV2 on the Oxford-IIIT Pet dataset. Covered weight initialization, regularization (L2, Dropout, Batch Norm), optimizers (SGD, Momentum, RMSProp, Adam), hyperparameter tuning, transfer learning/fine-tuning, and 5-fold cross-validation for model selection.

**Dataset:** Oxford-IIIT Pet (37 breeds, 224x224x3 RGB images)

**Result:** From-scratch training plateaued at majority-class accuracy, while transfer learning reached 99.8% validation accuracy. Cross-validation selected a High-Dropout configuration, giving 89.81% test accuracy (F1 89.70%).
