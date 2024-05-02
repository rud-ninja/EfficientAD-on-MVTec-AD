# EfficientAD for anomaly detection in metal objects

*   Framework: Pytorch
*   Architecture: WideResNet101, CNN, AutoEncoder
*   Dataset: MVTec AD - Metal nut images


### Original images (left) and anomaly masks (right)

<p align="center">
  <img src="https://github.com/rud-ninja/EfficientAD-on-MVTec-AD/blob/main/images/images_and_anomaly_masks.PNG" alt="sample_images" width="40%">
</p>

*   Distillation training epochs - 5000
*   Teacher-student training epochs - 20000

### Results on object metal_nut only
[Student](https://github.com/rud-ninja/EfficientAD-on-MVTec-AD/blob/main/saved_models/student_model.pth)

[AutoEncoder](https://github.com/rud-ninja/EfficientAD-on-MVTec-AD/blob/main/saved_models/autoencoder_EAD.pth)
<p align="center">
  <img src="https://github.com/rud-ninja/EfficientAD-on-MVTec-AD/blob/main/images/results.PNG" alt="sample_images" width="100%">
</p>

### Results on all objects in the MVTec AD dataset
[Student](https://github.com/rud-ninja/EfficientAD-on-MVTec-AD/blob/main/saved_models/student_model_all.pth)

[AutoEncoder](https://github.com/rud-ninja/EfficientAD-on-MVTec-AD/blob/main/saved_models/autoencoder_EAD_all.pth)
<p align="center">
  <img src="https://github.com/rud-ninja/EfficientAD-on-MVTec-AD/blob/main/images/results_all.PNG" alt="sample_images" width="100%">
</p>


Remarks: Need to improve feature extraction by increasing distillation training epochs for better performance on multiple objects. 

### References
*   [EfficientAD: Accurate Visual Anomaly Detection at Millisecond-Level Latencies](https://arxiv.org/abs/2303.14535)
*   [Towards Total Recall in Industrial Anomaly Detection](https://arxiv.org/abs/2106.08265)
