# Gait_Datasets
Part of the datasets of the  article ["Robust Gait Recognition by Integrating Inertial and RGBD Sensors"](http://ieeexplore.ieee.org/document/7888946/).  
## gait_mobile_Acc_data
Folder gait_mobile_Acc_data/fast(or nomal) contains the phone acceleration data when the user is walking at fast(or normal) speed.   
Subfolders ("aaa", "cxb", "lbr", ...) store data for ten different users, the folder name is the name of the tester's abbreviation.   
The file name of a single data subfile is named after the rule of "tester's abbreviation"_"attr""count".txt, where "attr" includes "fa, fb, na, nb", "f" and "n" for fast speed and normal speed, "a" and "b" on behalf of the phone on the left or right side of the pants pocket， "count" means that the file is simply counted
## 9_gestures_of_15_tester_data
### Acceleration data of 9 gestures
Folder 9_gestures_of_15 tester contains 5 subfolders that store walking data acceleration from 1 to 5 step-length.  
Subfolders store data for 15 different users, the file name of a single data subfile is named after the rule of "tester's abbreviation"_"m(1to9)""attr"_"count".txt, where "m(1to9)" for 9 different walking gestures. "attr" includes "fa, na", "f" and "n" for fast speed and normal speed, so the ratio of the two types of data is 1: 4.  
The total amount of data in a subfolder is: (1 + 4) x 9 x 15 = 675
### Kinect data of 9 gestures
The kinect of 9 gestures corresponding to the above acceleration data can be downloaded [**here**](https://pan.baidu.com/s/1hszgWJE). The data has been compressed twice,  you can run "Kinect_data_9gestures_15tester.part01.exe" to do the initial decompression.  
The file tree of this dataset is shown in "File Tree of "Kinect data of 9 gestures"". Subfolders named from 1 to 15 store data for 15 different users, and every subfolder has (1 + 4) x 9 = 45 groups of data, the ratio of data in fast speed and normal speed is also 1:4.  
 The person in the video data (Kinect data of 9 gestures) (numbers) correspond to the person in folder "Mobile_data_9gestures_of_15tester" in order of 'ls','zht','zq','lyb','nlh','lt','zm','wy','zy','lx','hss','wjj','zz','ywq','cxb'. Both types of data are recorded simultaneously 
The file structure of each video subfolder is as follows:
- **Video_subfolder**
  + **BodyIndexCalibrated**  
  This folder contains calibrated human body data which represented with txt file for each frame, named in time. For every txt file, there are lots of lines, each of which is  in the form of (x,y,z). x,y are coordinate of different pixle (frame size is 1920 * 1080)and z is pixle value(range from 0 to 255).
  + **OriginalCalibratedText**  
  This folder contains human body data without any calibration. Pixles are in the form of (x,y,z). z is the depth value of the pixle at (x,y).
  + **rgbClipped**  
  This folder contains rgb pictures of the tester. each of the picture is corresponding to the txt file in the BodyIndexCalibrated folder.
  + **rgbVideo**  
  This folder contains rgb pictures of the tester without clipping.
  + **SkeletonData**  
  This folder contains skeleton data of the tester for each frame, which is represented in the form of (x,y,z). x,y is coordinate of the skeleton point and z is the horizontal distance from the point to the kinect. each txt file contains 9 skeleton points, which represents head,.... respectively.

