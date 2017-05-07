# Image classifier
Image classifier is a Udacity capstone project.


## Getting Started

The project consists of 2 parts:
1) GetFiles.ipynb - data collection. Use this file to collect the data in case you want to do it manually. You can also download the dataset from this link. 
2) ClassifyImages.ipynb - main project. 



## Prerequisites

The project was build on Python 2.7 and Google Cloud Platform using:
- Google VM instance
- Google Datalab
- Google BigQuery
- Google Storage (optional)

To run the analysis please upload the files in your Google Cloud workspace. See "Setting up" section below. 

Libraries and modules we used:
- google.datalab
- pandas
- numpy
- logging
- pillow
- os
- random (optional)
- json (optional)
- urllib (optional)
- requests (optional)
- codecs (optional)
- cv2 (optional)
- pytube (optional)



## Setting up

To make the project running in Google Cloud, follow the instruction below.
1) set up your account and project in [Google Cloud.](https://cloud.google.com/)
2) create and connect to a [Cloud Datalab instance](https://cloud.google.com/datalab/docs/quickstarts#create_and_connect_to_a_cloud_datalab_instance)
3) go to /content/ directory by clicking Home icon (see 1). Create a notebook in home directory by clicking Notebook (see 2) 

<a><img src="http://image.prntscr.com/image/5ff4430c4e7b4bf7bedbb942c5d92a1c.png" height="200"></a>

4) insert code cell in your new notebook and run
```
!git clone https://github.com/mzhigarev/Udaticy_MLE_Capstone
```
to copy GitHub repo to your Google Datalab folder. This command will move the files into home directory ('/content/')

```
!gsutil mv /content/Udaticy_MLE_Capstone/* /content/
```
And lastly, remove unnecessary folders
```
import shutil
shutil.rmtree("/content/Udaticy_MLE_Capstone/")
shutil.rmtree("/content/datalab/")
```
5) Due to GitHub limit for file size, not all files will be copied. You need manually upload files from [Google Drive repository](https://drive.google.com/open?id=0B_MIut4tVCU4Z2JyQzN5cGZ5ejQ) into your directory on Google Cloud.
6) Finally your directory should contain these files and folders: 
```
ad_test/
excel-word-classifier-tt/
ClassifyImages.ipynb
GetFiles.ipynb
```
now you can reference the folder with path "/content/", so for example GetFiles.ipynb has a path "/content/GetFiles.ipynb"



## Optional
We pre-collected files for testing/training. If you want to collect your own set, please run GetFiles.ipynb on local machine. 


We used OpenCV and Pytube for data collection and preparation (see GetFiles.ipynb). The libraries are optional, all files you can find [here](https://github.com/mzhigarev/Udaticy_MLE_Capstone/excel-word-classifier-tt/). In case you want to gather your own data, use the libs on your local machine. 

Install the labraries:
```
!pip install pytube
!pip install opencv-python
```

