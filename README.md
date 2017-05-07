# Image classifier
Image classifier is a Udacity capstone project.


## Getting Started

The project consists of 2 parts:
1) GetFiles.ipynb - data collection. Use this file to collect the data in case you want to do it manually. You can also download the dataset from this link. 
2) ClassifyImages.ipynb - main project. 


### Prerequisites

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
- random
- json
- urllib
- requests
- codecs
- cv2
- pytube


### Setting up

We used OpenCV and Pytube for data collection and preparation (see GetFiles.ipynb). The libraries are optional, all files you can find [here](https://drive.google.com/open?id=0B_MIut4tVCU4cFh0Z19hWmJWMDA). In case you want to gather your own data, use the libs on your local machine. 

Install the labraries:
```
!pip install pytube
!pip install opencv-python
```

To make the project running in Google Cloud, follow the instruction below.
1) set up your account and project in [Google Cloud.](https://cloud.google.com/)
2) create and connect to a [Cloud Datalab instance](https://cloud.google.com/datalab/docs/quickstarts#create_and_connect_to_a_cloud_datalab_instance)
3) copy [files and notebooks](https://drive.google.com/open?id=0B_MIut4tVCU4cFh0Z19hWmJWMDA) in your core folder which has url similar to this - (https://XXXX-dot-XXXXXXX-dot-devshell.appspot.com/tree)

Finally your folder should contain these files and folders: 
```
ad_test/
excel-word-classifier-tt/
ClassifyImages.ipynb
GetFiles.ipynb
```
now you can reference the folder with path "/content/", so for example GetFiles.ipynb has a path "/content/GetFiles.ipynb"
