# Darknet-YOLO

You only look once (YOLO) is a state-of-the-art, real-time object detection system.

Steps for object detection using a pre-trained model.

  - git clone https://github.com/pjreddie/darknet
    cd darknet
    make
   
  - Download pre-trained weights.
    - wget https://pjreddie.com/media/files/yolov3.weights
    
   - Run Dtetector
      ./darknet detect cfg/yolov3.cfg yolov3.weights data/dog.jpg
 
 You can change the detection threshold from the default value which is det to 0.25
 by passing the -thresh <val> flag to the yolo command.
    ./darknet detect cfg/yolov3.cfg yolov3.weights data/dog.jpg -thresh 0.7
  
