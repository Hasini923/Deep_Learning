# Experiments 8 & 9 – Attention Type in a Pretrained ResNet50

Studied how different attention mechanisms modify an ImageNet-pretrained ResNet50 and how they affect flower image classification. Six models were trained, each in its own notebook, under an identical protocol (same split, augmentation, seed and training schedule); only the attention type changed.

Topics covered:

* ResNet50 stage-wise architecture (conv2_x – conv5_x)
* Channel attention (SE-style)
* Spatial attention
* Sequential Channel → Spatial attention
* Self-attention
* Combined attention
* Two-phase transfer learning (frozen backbone, then fine-tuning)
* Grad-CAM and internal attention maps
* Accuracy–complexity trade-off

Dataset: TensorFlow Flowers (`flower_photos`)

* 5 classes: daisy, dandelion, roses, sunflowers, tulips
* 3,670 images, stratified 70:15:15 split (2,569 / 550 / 551)
* Input shape: 224 × 224 × 3

Models: attention inserted at P3 (after conv4_x, 14 × 14 × 1024)

* A0 Baseline, A1 Channel, A2 Spatial, A3 Channel+Spatial, A4 Self-Attention, A5 Combined
* Frozen backbone for 10 epochs (Adam 1e-3), then conv5_x unfrozen for 10 epochs (Adam 1e-4)
* Batch size 32, dropout 0.3, reduction ratio 16, spatial kernel 7 × 7, seed 42

Result: Compared the six models using accuracy, precision, recall, F1-score, parameter count, inference time and training time. Test accuracy ranged from 0.922 (A5) to 0.944 (A2) against 0.935 for the baseline; no difference was statistically significant. Attention shifted errors (mainly roses ↔ tulips) rather than removing them. Numerical results were obtained from the experimental execution.
