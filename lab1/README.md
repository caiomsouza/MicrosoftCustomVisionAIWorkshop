# Microsoft Custom Vision AI Workshop
This workshop explains how to use Microsoft Custom Vision AI to detect images. 

## Use Case 1 - Lab 1 - Social Distance Image Detector
This lab 1 explains how to use Microsoft AI to detect Social Distance using Microsoft Customvision.ai (AI/ML) and Microsoft PowerApps. This is not production ready. <BR>

The goal of this Demo App is to identify Social Distance in an image. <BR>
This is a binary classification: Yes or No. <BR>
  
### Tools
1. Microsoft PowerApps (https://powerapps.microsoft.com/) <BR>
2. Microsoft CustomVision.ai (https://www.customvision.ai/) <BR>  

### How to identify Social Distance? 
If we have two or more people together without keeping the social distance guidelines, we classify Social Distance equals NO. <BR>

In the picture below we can see they are all following Social Distance guidelines. <BR>

![Social Distance](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/data/social-distance-images/funny-images/beatles-abbey-road-social-distancing%20(1).jpg)

### Keep Social Distance to save lives now

![Social Distance definition](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/data/social-distance-images/social-distance-definition/social-distancing-620.jpg)

### Social Distance equals YES 

![Social Distance equals YES](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/data/social-distance-images/yes/000_1PR2KI.width-800.jpg)

### Social Distance equals NO

![Social Distance equals NO](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/data/social-distance-images/no/0_EUV_pUXXQAA0cY_.jpg)

All images were collected using Google and Bing Search. They are all publicly available in the internet. <BR>

### Social Distance funny solutions

![Funny 1](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/data/social-distance-images/funny-images/25877132-8104031-image-a-28_1584009191615.jpg)

![Funny 2](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/data/social-distance-images/funny-images/_1_main_screengrab.jpg)


# Workshop Lab 1 - Step by Steps (NOT Completed)

1) Build the Power Apps 
First you need to have a PowerApps account. 
With your PowerApps account login in using the address https://powerapps.microsoft.com/en-us/

Use this link to build your new Power App: <BR>
https://preview.create.powerapps.com/studio <BR>


2) Build your Custom Vision AI Model

Call: <BR>
ClearCollect(imgcol,CustomVision.DetectImageV2("Your Custom Vision AI project ID","Your Iteration",Camera1.Photo).predictions) <BR>


Real example:<BR>
ClearCollect(imgcol,CustomVision.DetectImageV2("8c1fa230-043d-42ba-b284-e52653d873ef","Iteration1",Camera1.Photo).predictions)<BR>



### References

Use your model with the prediction API<BR>
https://docs.microsoft.com/en-us/azure/cognitive-services/custom-vision-service/use-prediction-api<BR>

PowerApps Pro Tips | How to Set Up Image Capture<BR>
http://powerappspros.com/2017/03/powerapps-pro-tips-how-to-set-up-image-capture/<BR>

How to upload images from the camera control to Azure blob storage<BR>
https://powerapps.microsoft.com/en-us/blog/custom-api-for-image-upload/<BR>

Quickstart: Create an image classification project with the Custom Vision Python SDK<BR>
https://docs.microsoft.com/en-us/azure/cognitive-services/custom-vision-service/python-tutorial<BR>

POWERAPPS TUTORIAL: HOW TO BUILD YOUR FIRST POWERAPP<BR>
https://jobs.collab365.community/powerapps-tutorial-how-to-build-your-first-powerapp/<BR>

Youtube videos:<BR>
https://www.youtube.com/watch?v=syt61L03dpc<BR>
https://www.youtube.com/watch?v=syt61L03dpc<BR>
https://www.youtube.com/watch?v=P5yKrEfKtEI<BR>
https://www.youtube.com/watch?v=KUtdnnYRpo4<BR>
https://www.youtube.com/watch?v=O0vstZ1EBaI<BR>
https://www.youtube.com/watch?v=wtTYSyBUpFc<BR>

Xamarin<BR>
https://docs.microsoft.com/en-us/xamarin/get-started/what-is-xamarin<BR>
