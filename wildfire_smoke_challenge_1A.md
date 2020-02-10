# Challenge IA: Smoke vs No Smoke using Entire Image

In this challenge, your task is to build a wildfire smoke classifier using the full image. 
We provide the following HPWREN camera smoke vs no smoke images as training dataset. 
You can use your solution as the entry to the Let's Stop Wildfire Hackathon. 
The same hackathon rules apply to this challenge. See [rules](README.md)

#### Train Dataset
You can download the train dataset below. 
It consists of three folders, one contains smoke, the other contains no_smoke images, and
a reference folder. 
You can only use the smoke and no smoke images for training.
The accompanying reference folder contains multiple subfolders where 
each subfolder contains image sequences captured with a HPWREN camera.
This reference folder allows you to loop through image sequences and examine the progression of smoke. However, you cannot use the reference folder in training. 

Note: If you want to use temporal sequence to detect start of smoke ignition, please join [Challenge 2](wildfire_smoke_challenge_2.md).

You can find the train dataset from either the Google drive link or Dropbox link.

* [Google Drive: train dataset](https://tinyurl.com/roo8tas)

or

* [Dropbox: train dataset](https://www.dropbox.com/s/ghfhjtoh1z59xeb/wildfire_smoke_data.tar)
* [Dropbox: reference sequence dataset](https://www.dropbox.com/s/791wed3scimh6sq/sequence_reference.tar.gz)


#### Submission
You will have to create a new github repo for your codes with the MIT License. To allow us to evaluate your model against our test dataset, you can either 

1) Save your model in HDF5 format and share it in your repo. If the model size is over 100MB, please provide either Dropbox or Google Drive link to your model. We will load your model and evaluate it against our test dataset.

or

2) Provide a python program to read in a folder consists of multiple images and predict whether there is smoke or no smoke in each image and write the output in a CSV file with the following format.

##### Output File
image_name, smoke_detected(1 if smoke detected or 0 if no smoke)

Example:
```
image_name_a,1
image_name_b,0
```

#### Contact Us
Please feel free to reach out to us if you have any questions. Join AI For Mankind **Slack** [https://tinyurl.com/rrsflyv](https://tinyurl.com/rrsflyv) channel to ask question.
