# centenis-mobile
Centenis-mobile is the mobile equivalent of the web app that is  used to detect and diagnose early stage Alzheimer's disease and dementia, and in addition to being able to be used as a tool to treat victims of brain injury. It utilizes IBM Watson's Visual Recognition API and BigHugeLab's Thesaurus API to classify a standard set of images. The app presents the user with a series of images (currently web only) which they try to identify, and their answer is checked with the classifications generated by Watson's computer vision algorithms.

To run the app:

Run git clone https://github.com/calufornia/centenis-mobile.git in an appropriate directory.

Compile and build using gradle and Android Studio.
*There is a significant error with the android file storage that causes the application to crash on some phones. 
I am actively searching for a fix for this issue, but it will be fixed in the future in one way or another*

Steps:
1.) Press the "Select Gallery Image" button to pick and retrieve any picture of 100 square pixels or more (size is maxed to 4mb due to IBM watson API's)
*ERROR OCCURS HERE ON SOME PHONE*
2.) You should now see the image on the bottom half of your screen (give it a second)
3.) Enter a "Guess" of what you think the picture depicts
4.) On the terminal you should be able to see if your guess (and it's related synonyms) are similar to watson's categories
