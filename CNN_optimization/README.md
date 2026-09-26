### Experiment 5 – CNN Training, Regularization, Optimization, Transfer Learning & Cross-Validation

Trained MobileNetV2 on the Oxford-IIIT Pet dataset, covering weight initialization, regularization (L2, Dropout, Batch Norm), optimizers (SGD, Momentum, RMSProp, Adam), hyperparameter tuning, transfer learning/fine-tuning, and 5-fold cross-validation for model selection.

**Result:** From-scratch training stalled at majority-class accuracy, while transfer learning reached 99.8% validation accuracy. Cross-validation selected a High-Dropout configuration, yielding 89.81% test accuracy.
