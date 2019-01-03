# mAP_eval (In progress)

Goals:
1. Convert Yolo Darknet Ground Truth Files to pycocotools json
2. Convert Yolo Darknet Detection Files to pycocotools json
3. Convert Yolo Darknet Ground Truth/Detection Files to */groundtruths /detections* folder usable by [rafaelpadilla/Object-Detection-Metrics](https://github.com/rafaelpadilla/Object-Detection-Metrics)
4. Customizable Ground Truth/Detection format for custom datasets

Current state:
Verifying mAP for the 5k validation dataset with results generated from [AlexeyAB/darknet](https://github.com/AlexeyAB/darknet) .  
`./darknet detector test cfg/coco.data cfg/yolov3.cfg yolov3.weights -thresh 0.005 -dont_show -ext_output < /home/dickson/data/coco/5k.txt > result.txt`  

Refer to demo.ipynb for details

![map_0 5iou_darknet](https://user-images.githubusercontent.com/22487836/50642471-3afa9800-0fa6-11e9-89da-bb8fb294b863.png)



# References

1. [AlexeyAB/darknet](https://github.com/AlexeyAB/darknet) 
2. [rafaelpadilla/Object-Detection-Metrics](https://github.com/rafaelpadilla/Object-Detection-Metrics)
3. [Cartucho/mAP](https://github.com/Cartucho/mAP)
4. [cocodataset/cocoapi](https://github.com/cocodataset/cocoapi)
