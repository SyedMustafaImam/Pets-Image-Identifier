# Dogs-Image-Identifier
Classifies pet images using a pretrained CNN model, compares these
classifications to the true identity of the pets in the images, and
summarizes how well the CNN performed on the image classification task. 
Note that the true identity of the pet (or object) in the image is 
indicated by the filename of the image. Therefore, your program must
first extract the pet image label from the filename before
classifying the images using the pretrained CNN model. With this 
program we will be comparing the performance of 3 different CNN model
architectures to determine which provides the 'best' classification.



Use argparse Expected Call with <> indicating expected user input:
      python check_images.py --dir <directory with images> --arch <model>
             --dogfile <file that contains dognames>
                     also uses ResNet, AlexNet and VGG

# The objetives of this Proof of concept are:

1. Correctly identify which pet images are of dogs (even if breed is misclassified) and which pet images aren't of dogs.
2. Correctly classify the breed of dog, for the images that are of dogs.
3. Determine which CNN model architecture (ResNet, AlexNet, or VGG), "best" achieve the objectives 1 and 2.
4. Consider the time resources required to best achieve objectives 1 and 2, and determine if an alternative solution would have given a "good enough" result, given the amount of time each of the algorithms take to run.
