# Project Name: Familiar Faces

My idea was to sort of create code for a doorbell camera that can identify specific people (family/close friends), so I retrained network to identify my face and my brother's face.

![A Ring doorbell camera, which is similar to the nature of this project, because the project is meant to be a doorbell camera that recognizes sprecific faces](https://ecobestreviews.com/wp-content/uploads/2020/06/Doorbell.jpg)

## The Algorithm

Add an explanation of the algorithm and how it works > The algorithm was re-trained on resnet18 by using about 33 training images and 7-8 val immages for each familiar face (both mine and my brother's). After running 35 epochs, the model was exported as am onnx file and used along with a webcam. For this project to be successful, the re-trained model is neccesary, and must be a onnx file, or elsethe jetson will not be able to use it. 

## Running this project

1.) set up jetson nano

2.) scp the files into jetson (Location is /home/jetson-inference/python/training/classification/data)

3.) ssh into the jetson nano

4.) cd into jetson-inference/python/training/classification/data

5.) plug in webcam

6.) run the re-trained network with imageNet on the webcam.

7.) See the results!



[View a video explanation here](https://youtu.be/wSnLIc7GWAE)
