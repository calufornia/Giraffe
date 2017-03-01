# Centenis
Centenis (the mobile equivalent of the web app) is an app used to detect and diagnose early stage Alzheimer's disease and dementia, which is in addition to it being a tool to treat victims of brain injury. It utilizes IBM Watson's Visual Recognition API, BigHugeLab's Thesaurus API to classify a standard set of images and Google's speech to text functionality. The app presents the user with a series of images (currently web only) which they try to identify, and their answer is checked with the classifications generated by Watson's computer vision algorithms. To account for the enourmous diversity of the human language, this string is then run through another api via HTTP GET requests that find synonyms for the string (this allows the user to see if they were in the general vacinity of what Watson thought the image represented).

To run the app:

Run git clone https://github.com/Karsten12/Centenis.git in an appropriate directory.

Compile and build using gradle and Android Studio.
*There is a significant error with the android file storage that causes the application to crash on some phones. 
I am actively searching for a fix for this issue, but it will be fixed in the future in one way or another*

Steps:
1.) Press the "Select Gallery Image" button to pick and retrieve any picture of 100 square pixels or more (size is maxed to 4mb due to IBM watson API's)
*ERROR OCCURS HERE ON SOME PHONE*
2.) You should now see the image on the bottom half of your screen (give it a second)
3.) Enter a "Guess" of what you think the picture depicts
4.) On the terminal you should be able to see if your guess (and it's related synonyms) are similar to watson's categories


Future features:
1.) Ability to upload and categorize up to 20 images at any given time
2.) Machine learning so that the user can pinpoint exactly what categories they are missing (SUPER USEFULL TO DOCTORS)
3.) Possibilty of using cloud based photos from popular vendors like Google Photos etc..
