# YoLo on Custom Dataset

## Description : Preprocessing step
This project implements the YOLO (You Only Look Once) algorithm for object detection on a custom dataset. 
1. Preprocessing of Data
   ```bash
   https://github.com/RajratanWankhade/YoLo_On_Custom_Dataset/blob/master/1_datapreparation/01_extract_object_info_xml.ipynb

We have a dataset labeled in XML format that needs to be converted into YOLO-compatible format, specifically with fields for class ID, center x, center y, width, and height. Before performing the conversion, we'll preprocess the XML data by loading it into a Pandas DataFrame to enable further analysis and gain deeper insights into the dataset.
            A. Get List of XML file in python
            B. Read and Extract label data from XML format
            C. Convert labels into Pandas
            D. Create Labels for YOLO model in Python using below formula 




   ![image](https://github.com/user-attachments/assets/8143a78f-678f-4e93-8e42-30ade68f0c44)


2. Split Images into Train and test

3. Label Encoding of Objects
   Its nothing but assigning the numbers into objects. car: 01, Bat: 02

   

5. Creating Train and Test Folder accodring to Yolo requirement



![1_XupA8TGTSGdZdjsrs16hkw](https://github.com/user-attachments/assets/37b423ab-fcbe-4888-ae95-6d925fdd0630)




## Description: YOLO Model Training 

1. Traing Yolo model on Google colab
   ```bash
   https://colab.research.google.com/drive/1ksBl-Br13-nBXkIpk_UnjNLgXo0bMIxA?usp=sharing

2. Saving Models weights into best.pt file in a yolo directory folder
         !python train.py --data data.yaml --weights yolov5s.pt --batch-size 8 --name Model --img 640 --epochs 150

   
4. Model retraining : If you are not satisfied with the model performance retrain it but insted of using yolov5s.pt use best.pt weights, which is saved in runs/model/train.

   !python export.py --weights runs/train/Model/weights/best.pt --include onnx --simplify --opset 12

   
5. Export Model into ONNX : best.onnx we will use it in prediction section to run inferences

   !python export.py --weights runs/train/Model/weights/best.pt --include onnx --simplify --opset 12



### description : Running Predictions on images or video file or live stream  from any IP cameras

1. Load YAML
2. Load YOLO
3. load the image
4. Get the YOLO prediction from images
5. Non- Maximum supression
6. Bounding Boxes
   

### Description : Running this yolo app on streamlit to get inferences( i plan to work on it in near future)   

   

       
   
            

 
 

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/RajratanWankhade/YoLo_On_Custom_Dataset.git

2. Enitre Project Link
```bash
https://drive.google.com/drive/folders/1fUHOf7SP5QpjpiuxO2jO8J6Pek2bmQxS?usp=sharing   



