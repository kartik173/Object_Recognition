# Identifying Vehicles from Video data

The code in this notebook performs the task of **taking a video file as input**, and creating **cropped images of the objects detected in the video**.

These cropped images are created as training data for a Deep Learning model. The images will be further labeled into 3 classes - 
1. 2 or 3 wheelers (motorbikes, rickshaws, etc.)
2. 4 wheelers (cars)
3. 4+ wheelers (buses, trucks, etc.)

The overall workflow of this demonstration is as follows:

- We first define some **global variables** that will be used through the entire demo
- Then, we **define functions** that will be used during execution.
- As soon as you run the **while loop** in the main function, the **first frame of the video is initialised**.
- Using your mouse, you will **draw a line across one side of the road**. This will appear as a yellow line.
- Once you draw the line, the video will start running.
- Then, the video will keep running, and **vehicle images will get cropped** and get saved on a specified path.
- When the **vehicle count reaches a certain threshold**, the video will stop.
- All the cropped images will get saved on your machine.
