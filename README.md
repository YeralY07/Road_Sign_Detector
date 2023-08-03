
# Road Signs Detector

My project detects road signs and tells what to to do when detecting them. It can detect stop, pedestrian and speed limit signs

## The Algorithm

My model uses imagenet with trained model that uses dataset. I changed imagenet to only show message related to road signs and give basic instruction what to do. 

## Running this project

1.Go to jetson-inference/python/training/classification by writing cd jetson-inference/python/training/classification in the terminal
2.Write /home/nvidia/jetson-inference/build/aarch64/bin/imagenet.py --model=models/RoadSign_Dataset/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=data/RoadSign_Dataset/labels.txt /dev/video0 in terminal and show road signs to camera and see i=messages in terminal 
3.Press Ctrl + C to escape


## Dataset Links
Speed Limit Sign: https://www.kaggle.com/datasets/andrewmvd/road-sign-detection
Stop Sign: https://images.cv/dataset/stop-sign-image-classification-dataset
Pedestrian sign: https://universe.roboflow.com/germantrafficsigns-zl3mn/pedestrian-crossing-sign-n7qju

## Project is in master branch
