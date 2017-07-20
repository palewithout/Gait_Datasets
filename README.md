# Gait_Datasets
Part of the datasets of the  article " Robust Gait Recognition by Integrating Inertial and RGBD Sensors".  
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
