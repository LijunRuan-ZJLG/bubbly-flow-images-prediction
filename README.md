# Developed-an-improved-one-hot-encoding-method-for-bubbly-flow-image-prediction-generation-under-cont

In this paper, we proposed an improved one-hot method to achieve bubbly images generation at continuable superficial gas velocities.

## predict bubbly flow images with continuable superficial gas velocities
**1. download the pickle file**
```
https://drive.google.com/drive/
```
**2. generate bubbly flow image**
```python
python run_generator.py generate-images  --seeds=6600-6609 --truncation-psi=1.0 --label=0 --network=xxx/xxxx
```
If you want to train the network on your own dataset,you can do as follow:
```
python train.py
```

## detect
Don't forget to put the weights file into the “model_data” folder.
We have put the weights of the detector to the url mentioned above.
```
python yolo_video.py
```
The detection results and labels are saved in folders "results" and "output" respectively
