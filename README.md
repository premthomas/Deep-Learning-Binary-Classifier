# Deep Learning (Binary Classifier) 
## With custom data (Kevin and Stuart from 'The Minions')
### Objective
You want to understand 'Deep learning'. Your search will almost always take you to the famous dataset: 'Dogs vs. Cats'. One of the better tutorials can be found [here](https://www.tensorflow.org/tutorials/images/classification). You implement the example and the results match the documentation. Very rarely, does a well documented example like 'Dogs vs. Cats go wrong. The data was collected and cleaned perfectly to get you similar results all the time. 

If you replace this dataset with one of your own, what would it look like? How much more effort would you have to put in? Would changing this example tutorial to use your dataset be extremely difficult? 

In this repository, I have created 5 programs. Each program explains one step of the process and ends with predicting for your data and checking the accuracies. 
<br><br>
### The environment
Assumption: Anaconda has been installed.
Executing a project inside an environment is not only a best practice but safe as upgrades do not hinder the execution in the future. The following commands are to be executed from the Anaconda command prompt.

Create the environment by using the command:`conda create --name <name of the environment> tensorflow-gpu`
  
Activate the environment by using the command:`conda activate <name of the environment>`

Install the following libraries using the `pip install`command
 - os
 - cv2
 - shutil
 - glob
 - pillow
 - random
 - matplotlib
 - sklearn
 - jupyter
 
Now your environment is complete to execute the programs found in this repository.
<br><br> 
### How to execute
 - Create a folder (e.g. Minion Recognition) on your drive for the project. 
 - Copy the code files from this repository into 'Minion Recognition'.
 - Create a sub folder called 'Data'.
 - Open the jupyter notebook with the title 'Step 1' and follow the instructions mentioned.
<br><br>
### About the data
The data has been collected with video display settings set to SD i.e. 720 x 480. Each video is about 10 seconds long and with an approximate FPS of 30, this should give us about 300 images per video. This is in no way sufficient. We need about 1000-1500 images per class to create an accurate model. 60 seconds of data capture should be good. 
 
 - Video files containing the string 'INP_VID' should be put in the correct class subfolders in the manually created 'Input Videos' folder. Follow the instructions and folder structure shown in the program 'Step 1'.
 - Video files containing the string 'TEST_VID' should be put in the correct class subfolders in the manually created 'Testing Videos' folder. Follow the instructions and folder structure shown in the program 'Step 6'. 
<br><br> 
### Results (as seen in the outputs of the programs)
Here are some of the more important variables used in the programs. 
 |Attributes|Value|
 |----------|-----|
 |Data split ratios (Train:Validate:Test)|60:30:10|
 |Training images (per class)|334|
 |Validation images (per class)|167|
 |Testing images (per class)|57|
 | | |
 |Epochs|Increments of 10|
 |Image height|200 px|
 |Image width|300 px|
 |Required validation accuracy|>90% (0.9)|
 |Required difference between training and validation accuracies|<5% (0.05)|
 
<br>

Program results
 |Attributes|Value|
 |----------|-----|
 |Training accuracy|94.16%|
 |Validation accuracy|93.71%|
 |Training loss|0.5660|
 |Validation loss|0.5589|
 |Testing accuracy|92.98%|
 |Testing accuracy (custom set with 222 images)|96.39%|
<br>
### Source
1. [Image classification tutorial](https://www.tensorflow.org/tutorials/images/classification) by Tensorflow.
