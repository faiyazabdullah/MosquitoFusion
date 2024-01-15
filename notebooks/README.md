<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
  <h1>MosquitoFusion_YOLOv8</h1>
  <p>This repository contains code for training and using YOLOv8 on the MosquitoFusion dataset.</p>
  <h2>GPU Information</h2>
  !nvidia-smi
  <h2>Installation</h2>
  !pip install ultralytics
  <h2>Train</h2>
  !yolo task=detect mode=train model=yolov8s.pt data=data.yaml epochs=25 imgsz=640 plots=True
  <h2>Validate</h2>
  !yolo task=detect mode=val model=runs/detect/train2/weights/best.pt data=data.yaml
  <h2>Predict</h2>
  !yolo task=detect mode=predict model=runs/detect/train2/weights/best.pt conf=0.25 source=data/test/images save=True
  <h2>Contributing</h2>
  <p>Feel free to contribute to this project by opening issues or submitting pull requests.</p>
</body>
</html>
