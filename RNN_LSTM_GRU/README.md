### Experiment 6 – RNN, LSTM, GRU & Video Understanding

Studied recurrent neural network architectures and implemented sequence learning using Vanilla RNN, LSTM and GRU models. The experiment also explored CNN-based feature extraction for video understanding and encoder–decoder sequence-to-sequence learning.

**Topics covered:**

* Vanilla RNN
* Backpropagation Through Time (BPTT)
* Vanishing and exploding gradients
* LSTM
* GRU
* Sequence classification
* CNN + LSTM/GRU for video understanding
* Encoder–decoder architecture
* Sequence-to-sequence learning

**Dataset:** UCI Human Activity Recognition Using Smartphones

* 6 activity classes
* 128 temporal measurements per sequence
* 9 sensor channels
* Input shape: 128 × 9

**Video Task:** UCF101

* Used a small subset of action classes
* 10 frames sampled per video
* Pretrained MobileNetV2 used for feature extraction
* CNN features processed using LSTM/GRU

**Result:**
Compared RNN, LSTM and GRU models using accuracy, precision, recall, F1-score, parameter count and training time. The experiment also demonstrated CNN-based video understanding and sequence-to-sequence learning through an encoder–decoder architecture. Numerical results were obtained from the experimental execution.
