# Deadlock Players Detector

#### Supported Labels
['allie', 'ennemi', 'mob', 'orbe']

#### ALL my models YOLO11, YOLOv10 & YOLOv9
- Yolov9c: https://huggingface.co/jparedesDS/cs2-yolov9c
- Yolov10s: https://huggingface.co/jparedesDS/cs2-yolov10s
- Yolov10m: https://huggingface.co/jparedesDS/cs2-yolov10m
- Yolov10b: https://huggingface.co/jparedesDS/cs2-yolov10b
- Yolov10b: https://huggingface.co/jparedesDS/valorant-yolov10b
- Yolo11m: https://huggingface.co/jparedesDS/valorant-yolo11m
- Yolo11l: https://huggingface.co/jparedesDS/deadlock-yolo11l

#### How to use
```
from ultralytics import YOLO

# Load a pretrained YOLO model
model = YOLO(r'weights\yolo11l_deadlock.pt')

# Run inference on 'image.png' with arguments
model.predict(
    'image.png',
    save=True,
    device=0
    )
```
#### Confusion matrix normalized
![confusion_matrix_normalized.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/MDMOTxs4G4qNBQFJcDU3l.png)
#### Labels
![labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/YTdoZBR1OWMyBkkJ9Q0ft.jpeg)
#### Results
![results.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/Yt-rYobyjz4t5O8WiapwS.png)
#### Predict
![val_batch0_labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/szWzcf3WFuhjVFyb4RwtE.jpeg)
![val_batch0_pred.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/MrKln2QfKXgEd4m_eBj5d.jpeg)
```
YOLO11l summary (fused): 464 layers, 25,282,396 parameters, 0 gradients, 86.6 GFLOPs
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 3/3 [00:01<00:00,  2.81it/s]
                   all        138        230      0.801      0.647      0.723      0.382
                 allie         12         15      0.662      0.733      0.714      0.419
                ennemi         85         97      0.889      0.743      0.852      0.522
                   mob         40         92      0.822      0.651      0.733      0.353
                  orbe         20         26      0.832      0.462      0.592      0.234
```

#### Others models Counter Strike 2 YOLOv10m Object Detection
https://huggingface.co/jparedesDS/valorant-yolov10b
