# Jetson-nano-benchmark

Model | GPU | Mode | Inference Time | Framework
-- | -- | -- | -- | --
mobilenet-yolov3-608 |  GTX 1080 | float32 | 12.655ms | TensorRT
mobilenet-yolov3-608 |  Jetson nano | float32 | 247.655ms | TensorRT
mobilenet-yolov3-lite-320 |  Jetson nano | float32 | 114.055ms | TensorRT
mobilenet-yolov3-lite-320 |  Jetson nano | float16 | 97.189 ms | TensorRT
tiny-yolov3-416 |  Jetson nano | float32 | 142.60 ms | darknet
tiny-yolov3-320 |  Jetson nano | float32 | 101.26 ms | darknet
mobilenet-yolov3-lite-416 |  Jetson nano (cpu) | float32 | 241.44 ms | ncnn 
mobilenet-ssd-300 |  Jetson nano (cpu) | float32 | 113.59 ms | ncnn 

* The performance in jetson nano was not satisfactory , I will try to optimize it 
