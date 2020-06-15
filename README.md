# EyeTracking
This project aims at locating the pixels/area on the device screen on which the user is gazing at via the on-device webcam.

HOW TO RUN:
src & out directories are the code directories
In the recent push I have also uploaded pic_ip and pic_op directories along with compile.bat and run.bat these

pic_ip and pic_op directories should be one level above the repo directory... that means if the .git folder is in C:/Desktop/EyeTracking directory then the pic_ip and pic_op must be in C:/Desktop directory
see the contents of compile.bat and run.bat you will understand what it is...

#BEFORE YOU COMPILE
You need to set path with this value
set path=%path%;<absolute path including the .dll file in src folder>

You need to set classpath with this value
set classpath=.;<absolute path including the .jar file in the src folder>

#UPDATE THE ABSOLUTE PATHS IN SOURCE CODE TO THE ONES FOR YOUR PC
ctrl+shift+f and find Imgproc.imwrite, calls to this function accept the save path (make it point to the pic_op folder on your pc)
