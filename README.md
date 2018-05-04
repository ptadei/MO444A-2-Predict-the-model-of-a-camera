# MO444A-Assignment-2

## Objective
Predict the model of a camera based on the content of their photographs. In other words, given an image, from which camera model did it come from? 

## Activities
Engineer your features. Here you do not have them for free. You need to think of possible ways for transforming the collected data into meaningful features. For some ideas, read attached papers.<p>
If you cannot think of anything, talk to the professor for some ideas. 

Propose classification techniques to solve the problem. Try first with Logistic Regression than move on to other models (e.g., K-NN, Neural Networks, etc). <p>

Is it possible to predict the model of a camera based on their noise signature? <p>

## Some ideas for your features 
Local Binary Patterns (LBPs)<p>
Wavelet features (DWT)<p>
Sensor Pattern Noise (SPN)<p>

Observation: You can use an already implemented feature extractor in this part that receives an image and gives you the feature vector<p>

Report all of your results comparing them to the real ground-truth provided in the dataset (real answers for each testing example). <p>
What are the reliable / easy camera for model identification? What’s the most difficult? Any ideas as for why this happens? <p>

## Dataset
Images in the training set were captured with 10 different camera models, a single device per model, with 275 full images from each device.<p>
### The list of camera models is as follows:
Sony NEX-7 <p>
Motorola Moto X<p>
Motorola Nexus 6<p>
Motorola DROID MAXX<p>
LG Nexus 5x<p>
Apple iPhone 6<p>
Apple iPhone 4s<p>
HTC One M7<p>
Samsung Galaxy S4<p>
Samsung Galaxy Note 3<p>

Images in the test set were captured with the same 10 camera models, but using a second device. For example, if the images in the train data for the iPhone 6 were taken with Ben Hamner's device (Camera 1), the images in the test data were taken with Ben Hamner's second device (Camera 2), since he lost the first device in the Bay while kite-surfing.<p>
None of the images in the test data were taken with the same device as in the train data.<p>
While the train data includes full images, the test data contains only single 512 x 512 pixel blocks cropped from the center of a single image taken with the device. No two image blocks come from the same original image.<p>
Half of the images in the test set have been altered. The image names indicate whether or not they were manipulated (_manip) from the original or unaltered (_unalt). While you are not explicitly told how each individual image was altered, the set of possible processing operations that were performed are as follows:<p>
JPEG compression with quality factor = 70<p>
JPEG compression with quality factor = 90<p>
resizing (via bicubic interpolation) by a factor of 0.5<p>
resizing (via bicubic interpolation) by a factor of 0.8<p>
resizing (via bicubic interpolation) by a factor of 1.5<p>
resizing (via bicubic interpolation) by a factor of 2.0<p>
gamma correction using gamma = 0.8<p>
gamma correction using gamma = 1.2<p>

### Dataset
MD5 (train.zip) = f3f8f3cd9fef8da6076f6b65b9b470f8<p>
MD5 (test.zip) = dddf8bb41b21906cefe40d079d6656ff

Download this dataset from https://www.kaggle.com/c/sp-society-camera-model-identification

### Submission
Bring your 4-page printed report and submit during class on the deadline day. This activity is INDIVIDUAL and not in teams. 
