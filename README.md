# Deadlock Players Detector

#### Supported Labels
['deny', 'enemy', 'hit', 'minions']

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
![confusion_matrix_normalized.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/FIZ5RQWnc61uzl7CNBOkq.png)
#### Labels
![labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/ESwV9FZEdDZOSCSIQto3N.jpeg)
#### Results
![results.png](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/k5XlHxnTNEFWM0_RVjDbK.png)
#### Predict
![val_batch1_labels.jpg](https://cdn-uploads.huggingface.co/production/uploads/62e1c9b42e4cab6e39dafc97/MWBpq382VcQfXOdXZS2N-.jpeg)
```
YOLO11l summary (fused): 464 layers, 25,282,396 parameters, 0 gradients, 86.6 GFLOPs
                 Class     Images  Instances      Box(P          R      mAP50  mAP50-95): 100%|██████████| 8/8 [00:03<00:00,  2.37it/s]
                   all        551        661      0.874      0.798      0.856      0.486
                  deny         13         14      0.748      0.857      0.819       0.48
                 enemy        197        228      0.942      0.785      0.883      0.508
                   hit         40         53      0.861      0.704      0.787      0.409
               minions        222        366      0.945      0.847      0.933      0.546
```

#### Others models Counter Strike 2 YOLOv10m Object Detection
https://huggingface.co/jparedesDS/valorant-yolov10b
