# Jetson-nano-benchmark

Model | GPU | Mode | Inference Time | Framework | Task
-- | -- | -- | -- | -- | --
[pelee-ssd-304](https://github.com/eric612/MobileNet-YOLO) |  Jetson nano | float32 | 53 ms | TensorRT-Pelee | Detection
[pelee-ssd-304](https://github.com/eric612/MobileNet-YOLO) |  Jetson nano | float32 | 89 ms | TensorRT-Pelee | [Detection + Segmentation](https://youtu.be/nndFtIPMy20)
[mobilenet-yolov3-lite-320](https://github.com/eric612/MobileNet-YOLO) |  Jetson nano | float32 | 66 ms | TensorRT-YOLOv3 | Detection

* pre/post process cosume 10 ms per frame 
* Framework link : [TensorRT-YOLOv3](https://github.com/eric612/TensorRT-Yolov3-models) , [ncnn](https://github.com/Tencent/ncnn) , [darknet](https://github.com/pjreddie/darknet), [TensorRT-Pelee](https://github.com/eric612/Pelee-Seg-TensorRT)
* The performance in jetson nano was not satisfactory , I will try to optimize it 
* Compare with yolov3-lite , the pelee network get 20% higher performance , it is because the upsample layer cosume 20% computiing time in yolov3-lite , which was not exist in pelee network , so the main difference was the upsample layer 
