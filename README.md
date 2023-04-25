# Developed-an-improved-one-hot-encoding-method-for-bubbly-flow-image-prediction-generation-under-continuable velocities

In this paper, we proposed an improved one-hot method to achieve bubbly images generation at continuable superficial gas velocities.

## Resouces

The weight file of the pretrained prediction model and the detector can be found on [Google Drive](https://drive.google.com/drive/folders/1yabGWhDVhZF-wJRkcB1fvQlKVyysC5Vf?usp=sharing)

## System requirement
* Python 3.5.2 
* Keras 2.2.5 
* tensorflow 1.14.0 
* CUDA 10.0 toolkit and cuDNN 7.5.

## Predict bubbly flow images with continuable superficial gas velocities

**Using pretrained model to generate bubbly flow image**
```python
python run_generator.py generate-images  --seeds=seed_num --truncation-psi=1.0 --label 1.0 0.0 0.0 0.0 0.0 --network=path_to_pkl
```

## Detect the bubbly flow images
Don't forget to put the weights file into the “model_data” folder.

We have put the weights of the detector on Google Drive.

```
python yolo_video.py
```
The detection results and labels are saved in folders "results" and "output" respectively
