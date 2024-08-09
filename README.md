# YoLo on Custom Dataset

## Description
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

4. Creating Train and Test Folder accodring to Yolo requirement
![1_XupA8TGTSGdZdjsrs16hkw](https://github.com/user-attachments/assets/37b423ab-fcbe-4888-ae95-6d925fdd0630)



   
            

 
 

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/RajratanWankhade/YoLo_On_Custom_Dataset.git

2.    



## Navigate to the project directory
cd YoLo_On_Custom_Dataset

## Create a virtual environment and activate it:


## Install the required packages:
