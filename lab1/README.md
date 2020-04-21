# Microsoft Custom Vision AI Workshop
This workshop explains how to use Microsoft Custom Vision AI to detect images. 

## Use Case 1 - Lab 1 - Social Distance Image Detector
This lab 1 explains how to use Microsoft AI to detect Social Distance using Microsoft Customvision.ai (AI/ML) and Microsoft PowerApps. This is not production ready. <BR>

The goal of this Demo App is to identify Social Distance in an image. <BR>
  
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

### Build the Power Apps 
First you need to have a PowerApps account. 
With your PowerApps account login in using the address https://powerapps.microsoft.com/en-us/

Use this link to build your new Power App: <BR>
https://preview.create.powerapps.com/studio <BR>

<b>Social Distance Detector Demo Power Apps</b><BR>
If you do not want to build your own Power Apps you can import this Power Apps.<BR>
https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/tree/master/lab1/src/PowerApp<BR>


### Build your Custom Vision AI Model

<b>Create a new Custom Vision Project</b>
![Create a new Custom Vision Project](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/tutorial/create-custom-vision-project.PNG)

<b>Add and label images</b>
![Train Images](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/tutorial/images-tagged.PNG)

<b>Train Images</b>
![Train Images](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/tutorial/train-images.PNG)

<b>Test with a new image</b>
![Test](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/tutorial/quick-test-model.PNG)

<b>Publish the Model</b>
![Quick test in the Model](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/tutorial/publish-model.PNG)

<b>Use the Prediction API to predict new images</b>
![Prediction API](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/tutorial/prediction-api.PNG
)

Call: <BR>
```javascript  
ClearCollect(imgcol,CustomVision.DetectImageV2("Your Custom Vision AI project ID","Your Iteration",Camera1.Photo).predictions)
```

Real example:<BR>
```javascript
ClearCollect(imgcol,CustomVision.DetectImageV2("8c1fa230-043d-42ba-b284-e52653d873ef","Iteration1",Camera1.Photo).predictions)
```

![Calling the Custom Vision API in the Power Apps](https://github.com/caiomsouza/MicrosoftCustomVisionAIWorkshop/blob/master/lab1/tutorial/power-app-call-customvisionapi2.PNG)


