# Drone_texture_workbooks
Jupyter notebooks for processing the big data workload I implemented for my master's thesis in big data analytics

## Background

### Project Overview
I tackled this project to achieve my master's degree in big data analytics from the Letterkenny Institute of Technology. The project concept was to compare two methods for classifying terrain as seen from a drone's camera, to determine what the terrain is that the drone can see. The first approach to be followed was to use classic computer vision techniques, while the second approach was to use a Convolutional Neural Network to perform the same classification. 

### Source data and classification
Source data was gathered from a DJI Mavic Air drone, flown over various bits of rural County Donegal in Ireland. The videos were pre-processed by a python script that dumped the image of ever 100 frames to file. 

One thousand images were taken from this process, and uploaded into an S3 bucket where the custom app in https://github.com/Joon/Image_Tagger was used to classify the images into 30 pixel square tiles of terrain classification, i.e. each tile was marked up as being foliage, water, road or building.

## Implementation
These notebooks show the process of inspecting the classification data, preparing training data for the CNN and comparing ther esulting Ilastik and CNN Predictions to measure the accuracy of the approaches as compared to the ground truth data available

## Link to the source data
The imagery data for this project was too large to place into Github. Instead, it's been uploaded to a Harvard Dataverse storage project at https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi%3A10.7910%2FDVN%2FCFZWVN
