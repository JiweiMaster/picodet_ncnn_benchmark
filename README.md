# Mobile Detection Benchmark
This repo is used to test the speed of the mobile terminal models


# Benchmark Result
| Model                        | Input size | mAP<sup>val<br>0.5:0.95 | mAP<sup>val<br>0.5 | Params<br><sup>(M) | FLOPS<br><sup>(G) | Latency<sup>[1](#latency)<sup><br><sup>(ms) | Latency<sup>[2](#latency)<sup><br><sup>(ms) | Config                                                                                                                                                                                                                                            |
| :--------------------------- | :--------: | :---------------------: | :----------------: | :----------------: | :---------------: | :--------------------------------------------: | :--------------------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| YOLOv3-Tiny                  |    416     |          16.6           |        33.1        |        8.86        |       5.62        |                     25.42                      |                       -                        | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/yolov3-tiny.zip) </br> [link](https://github.com/ultralytics/yolov3#:~:text=YOLOv3-tiny,640)                                                                   |
| YOLOv4-Tiny                  |    416     |          21.7           |        40.2        |        6.06        |       6.96        |                     23.69                      |                       -                        | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/yolov4-tiny.zip) </br> [link](https://github.com/Tianxiaomo/pytorch-YOLOv4)                                                                                    |
| PP-YOLO-Tiny                 |    320     |          20.6           |         -          |        1.08        |       0.58        |                      6.75                      |                       -                        | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/ppyolo-tiny.zip) </br> [link](https://github.com/PaddlePaddle/PaddleDetection/tree/release/2.2/configs/ppyolo#:~:text=post%20quant%20model-,PP-YOLO%20tiny,-8) |
| PP-YOLO-Tiny                 |    416     |          22.7           |         -          |        1.08        |       1.02        |                     10.48                      |                       -                        | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/ppyolo-tiny.zip) </br> [link](https://github.com/PaddlePaddle/PaddleDetection/tree/release/2.2/configs/ppyolo#:~:text=post%20quant%20model-,PP-YOLO%20tiny,-8) |
| Nanodet-M                    |    320     |          20.6           |         -          |        0.95        |       0.72        |                      8.71                      |                       -                        | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/nanodet-m-320.zip) </br> [link](https://github.com/RangiLyu/nanodet#:~:text=Model%20Size-,NanoDet-m,-320*320)                                                  |  |
| Nanodet-M                    |    416     |          23.5           |         -          |        0.95        |        1.2        |                     13.35                      |                       -                        | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/nanodet-m-416.zip) </br> [link](https://github.com/RangiLyu/nanodet#:~:text=NanoDet-m-,416*416,-23.5)                                                          |  |
| Nanodet-M 1.5x               |    416     |          26.8           |         -          |        2.08        |       2.42        |                     15.83                      |                       -                        | [model](hhttps://raw.githubusercontent.com/JiweiMaster/lfs/master/nanodet-m-1_5-416.zip) </br> [link](https://github.com/RangiLyu/nanodet#:~:text=NanoDet-m-1.5x-,320*320,-23.5)                                                 |  |
| YOLOX-Nano                   |    416     |          25.8           |         -          |        0.91        |       1.08        |                     19.23                      |                       -                        | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/yolox-nano.zip) </br> [link](https://github.com/Megvii-BaseDetection/YOLOX#:~:text=YOLOX-Nano,416)                                                                                                                                                      |
| YOLOX-Tiny                   |    416     |          32.8           |         -          |        5.06        |       6.45        |                     32.77                      |                       -                        | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/yolox-tiny.zip) </br> [link](https://github.com/Megvii-BaseDetection/YOLOX#:~:text=YOLOX-Tiny,416)                                                                                                                                                      |
| YOLOv5n                      |    640     |          28.4           |        46.0        |        1.9         |        4.5        |                     40.35                      |                       -                        | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/yolov5n.zip) </br> [link](https://github.com/ultralytics/yolov5#:~:text=YOLOv5n,640)                                                                                                                                                                 |
| YOLOv5s                      |    640     |          37.2           |        56.0        |        7.2         |       16.5        |                     78.05                      |                       -                        | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/yolov5s.zip) </br> [link](https://github.com/ultralytics/yolov5#:~:text=4.5-,YOLOv5s,640,-37.2)                                                                                                                                                      |
| PicoDet-S                    |    320     |          27.1           |        41.4        |        0.99        |       0.73        |                      8.13                      |                    **6.65**                    | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/picodet-s-320.zip) </br> [link]()                                                                                                                              |
| PicoDet-S                    |    416     |          30.6           |        45.5        |        0.99        |       1.24        |                     12.37                      |                    **9.82**                    | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/picodet-s-416.zip) </br> [link]()                                                                                                                              |
| PicoDet-M                    |    320     |          30.9           |        45.7        |        2.15        |       1.48        |                     11.27                      |                    **9.61**                    | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/picodet-m-320.zip) </br> [link]()                                                                                                                                                                                                                          |
| PicoDet-M                    |    416     |          34.3           |        49.8        |        2.15        |       2.50        |                     17.39                      |                   **15.88**                    | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/picodet-s-416.zip) </br> [link]()                                                                                                                                                                                                                          |
| PicoDet-L                    |    320     |          32.6           |        47.9        |        3.24        |       2.18        |                     15.26                      |                   **13.42**                    | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/picodet-l-320.zip) </br> [link]()                                                                                                                                                                                                                          |
| PicoDet-L                    |    416     |          35.9           |        51.7        |        3.24        |       3.69        |                     23.36                      |                   **21.85**                    | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/picodet-l-416.zip) </br> [link]()                                                                                                                                                                                                                          |
| PicoDet-L                    |    640     |          40.3           |        57.1        |        3.24        |       8.74        |                     54.11                      |                   **50.55**                    | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/picodet-l-640.zip) </br> [link]()                                                                                                                                                                                                                          |
| PicoDet-Shufflenetv2 1x      |    416     |          30.0           |        44.6        |        1.17        |       1.53        |                     15.06                      |                   **10.63**                    | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/picodet-shufflenetv2.zip) </br> [link]()                                                                                                                                                                                                                          |
| PicoDet-MobileNetv3-large 1x |    416     |          35.6           |        52.0        |        3.55        |       2.80        |                     20.71                      |                   **17.88**                    | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/picodet-mobilenetv3.zip) </br> [link]()                                                                                                                                                                                                                          |
| PicoDet-LCNet 1.5x           |    416     |          36.3           |        52.2        |        3.10        |       3.85        |                     21.29                      |                    **20.8**                    | [model](https://raw.githubusercontent.com/JiweiMaster/lfs/master/picodet-lcnet.zip) </br> [link]()                                                                                                                                                                                                                          |

<details open>
<summary><b>Table Notes:</b></summary>

- <a name="latency">Latency:</a> All our models test on `Qualcomm Snapdragon 865(4\*A77+4\*A55)` with 4 threads by arm8 and with FP16. In the above table, test latency on `1` [NCNN](https://github.com/Tencent/ncnn) and `2` [Paddle-Lite](https://github.com/PaddlePaddle/Paddle-Lite).
- All model are trained on COCO train2017 dataset and evaluated on COCO val2017.


# Support Library
 - [Paddle-Lite](./paddlelite/README.md)
 - [NCNN](./ncnn/README.md)


# TODO
### TNN, MNN speed supplement, welcome to contribute!
