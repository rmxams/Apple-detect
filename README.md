# Apple-detect
 An apple ripeness detector built off the jetson-inference library 

## The Algorithm

ResNet is a deep learning architecture that uses shortcut connections to enable training of very deep neural networks. Its key innovation lies in residual blocks, allowing gradients to flow more efficiently and enabling the development of deeper models for improved performance in various computer vision tasks.
## Running this project

Before running this project install the following:
* NVIDIA Jetson Nano
* Python 3.6 or later
* CUDA toolkit
* PyTorch

1. Set up the NVIDIA NANO
2. Connect the NANO to your computer through SSH (Open PUTTY on your desktop and input your Nano's IP address)
3. Log in to the Linux terminal
4. Download the jetson-inference folder, the machine learning and the model will run inside this folder
5. OpenVSC on your desktop and connect the Nano
6. Go to the NVIDIA folder
7. Open up a new terminal with the task bar
8. Go inside the jetson-inference folder using cd jetson-inference/
9. THe docker command will be used to enter the the docker container [./docker/run.sh]
10. Download the ONNX model located in the repository
11. Enter navigate to python/training/classification and export the model
12. Set the lables to ripe and unripe
13. Then, run [imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/train/ripe/rp0.jpg apple.jpeg]
##
* https://github.com/dusty-nv/jetson-inference/blob/master/docs/pytorch-cat-dog.md#processing-all-the-test-images
REFER TO THIS LINK IF YOU ARE HAVING ANY ISSUES


##
[View a video explanation here](video link)
