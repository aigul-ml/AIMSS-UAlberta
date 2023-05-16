# Medical Tool Detection
AIMSS Community Project 2021 -- Medical tool object detection with deep learning

![website](https://user-images.githubusercontent.com/64624048/128646725-67b67a45-0bf4-4fc1-9cbb-ebb28f7be66c.PNG)
## Surgical Object Detection and Counting Model
### Overview
During surgeries, a significant number of surgical tools are used, typically ranging from 250 to 300, and this number can increase depending on the complexity of the procedure. Unfortunately, a small percentage of abdominal operations, roughly 1/1000 to 1/3000, result in the unintentional retention of surgical objects within patients after surgery. These objects can include tweezers, scalpels, needles, sponges, towels, and more. Although surgical staff follow strict counting procedures to prevent such incidents, mistakes can still occur in the fast-paced and high-pressure environment of the operating room.

This project aims to address this issue by developing a machine learning model capable of detecting, classifying, and counting surgical objects in an image. By leveraging the power of machine learning, we aim to create a prototype that can act as an additional tool for counting surgical objects, providing an extra layer of assurance in the operating room.

### Features
* Detect and identify surgical tools in images.
* Classify different types of surgical objects.
* Count the number of surgical objects present in an image.
* Enhance the existing tool-counting process in the operating room.

The objective of this project was to create a working ML application with the help of the interdisciplinary AIMSS team in 2021. The team consisted of various undergraduates and graduate students in computing science, biological sciences, and various other disciplines. Despite the project being a simple image recognition application taking in data via files, it serves as a viable prototype that satisfies the primary goals of the project. With Harish Prabhakar as the team lead for the group that are beginners with programming and Sacha Davis as the team lead for the backend with more experienced developers in ML and AI, a full stack application was created.

## Prerequisites
1. python
2. pip

## Windows Instructions
### init (only needs to be done once) :frog:
1. pip install streamlit
2. pip install tensorflow --upgrade
3. pip install Cython pandas tf-slim lvis
4. pip install pyyaml
5. git clone https://github.com/tensorflow/models.git
6. set PATH=%PATH%;C:\path\to\protoc\bin	<-- You have to change this.
7. cd models/research
8. protoc object_detection/protos/*.proto --python_out=.
9. python setup.py install

### Running the website locally (make sure you are in the object_detection folder) :chicken:
1. streamlit run master_app.py
