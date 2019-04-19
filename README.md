# Jetson-nano-benchmark

Model | GPU | Mode | Inference Time | Framework
-- | -- | -- | -- | --
mobilenet-yolov3-608 |  GTX 1080 | float32 | 12.655ms | TensorRT-YOLOv3
mobilenet-yolov3-608 |  Jetson nano | float32 | 247.655ms | TensorRT-YOLOv3
mobilenet-yolov3-lite-320 |  Jetson nano | float32 | 114.055ms | TensorRT-YOLOv3
mobilenet-yolov3-lite-320 |  Jetson nano | float16 | 97.189 ms | TensorRT-YOLOv3
tiny-yolov3-416 |  Jetson nano | float32 | 142.60 ms | darknet
tiny-yolov3-320 |  Jetson nano | float32 | 101.26 ms | darknet
mobilenet-yolov3-lite-416 |  Jetson nano (cpu) | float32 | 241.44 ms | ncnn 
mobilenet-yolov3-lite-320 |  Jetson nano (cpu) | float32 | 156.77 ms | ncnn 
mobilenet-ssd-300 |  Jetson nano (cpu) | float32 | 113.59 ms | ncnn 
pelee-ssd-304 |  Jetson nano | float32 | 60~90 ms | TensorRT-Pelee 

* Framework link : [TensorRT-YOLOv3](https://github.com/eric612/TensorRT-Yolov3-models) , [ncnn](https://github.com/Tencent/ncnn) , [darknet](https://github.com/pjreddie/darknet), [TensorRT-Pelee](https://github.com/ginn24/Pelee-TensorRT)
* The performance in jetson nano was not satisfactory , I will try to optimize it 
