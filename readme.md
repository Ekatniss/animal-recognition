# Animal Recognition

 Add short description of project here > 
This project can recognize 38 different animals. You just need to give it an image and it will recognize what animal is in the image.
![Image of a rabbit](https://upload.wikimedia.org/wikipedia/commons/d/df/Eastern_Cottontail.JPG)

## The Algorithm

This project uses a retrained Resnet-18 model trained on images of 38 different wild animals. The program takes an input image and feeds it to the retrained model; the model then uses its training to deduce what animal it believes to be in the image and the result is printed out.

## Running this project

1. ssh into your jetson-nano and make sure you have jetson-inference installed
2. download this git repositoy and put it into your jetson-nano (do not put it under the jetson-inference folder)
3. go into the terminal and cd into the folder containing the files from the git repository
4. Run this command: imagenet.py --model=resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=labels.txt $IMAGE_NAME.jpg output.jpg
5. replace the $IMAGE_NAME with the file name of the image
6. you can also replace the output.jpg with your desired name of the output image

[View a video explanation here](video link)
