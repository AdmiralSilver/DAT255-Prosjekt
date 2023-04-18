# DAT255-Prosjekt
Repo for prosjektoppgave vår 2023

##
We decided to choose an assignement which included the automatic tagging of noisy audio recordings. This because we saw this as a challenging and exiting assignement where we could really challenge ourselves and create something useful. 

We feel we have created a good model but if we had more time there is still more that could be accomplished with the model, there is still some things that could be done with our model. We were not able to use raw audio files to create a direct audio model, but rather our model used the MFCC's of the audio files to tag the recordings. 

We also used a lot of time to try and create an application where a user could upload files in the browser and get a somewhat accurate representation of what the audio was, but was not successful in our attempt. 

The problem seems to appear when a audio file is processed and when a prediction is run on the audio something happens and it always returns the same result : [['Hi-hat' 'Bus' 'Squeak']], but when the models are run on the test set we get a great accuracy with what the actual audio represents. 

If we were able to fix this problem, then in theory you could easily use the model on different datasets to automatically label the data in a accurate way. 
##

To be able to run our notebook you need the dataset which was used in the training of the models. The FSDKaggle2018 datasets can be downloaded from Zenodo at: https://zenodo.org/record/2552860#.XFD05fwo-V4 

You might need to change some of the paths in the notebook to represent your paths depending on if you use Kaggle like we did or not. If you use Kaggle to run the notebook it should be pretty straight forward to run the notebook, just change the paths to represent your setup and run. We would recomend using Kaggles GPU accelerators if you run this. The run time will be around 13 minutes if you use a similar setup as we did with GPU P100 as accelerator. 
