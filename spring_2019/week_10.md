## Last Week's Accomplishments
(1) Update Profile Image: 
- added bar button item to top right of profile page navbar to allow for editing the profile image chosen from photo library
- complication with saving and loading images locally (ultimately will go to the database). The issue was you cannot save image data to userdefaults so I had to convert the image to a file and have it get added to the defaults file library with its own string extension. Then this string could be used in another function called loadImageFromDisk to recover the image. 
- Also needed a function to make the image into a square and then back into a circle to fit the original design

(2) Profile Image Icon:
- Added a new class for the tabbarviewcontroller to allow for customization of icons. 
- In new class loaded profile image and made it into a resized and rounded image. The roaded image involved writing an extension to the UIImage base class to create a path and cut out the desired image. The resize did something similar by drawing a path and placing the image inside of it. 
- After that the image was made into a uiimageview and placed on the tabbar and will update immediately upon being changed.

## This Week's Plan
This is the final week of RCOS! As before I will try to finish up the skeleton to allow for future programmers to finish the app.

## Anything Blocking?
no

## Notes
nothing to report
