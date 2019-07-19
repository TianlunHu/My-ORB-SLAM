# My-ORB-SLAM
ORB_SLAM is a widely used visual SLAM algorithm, whch could solve online or offline SLAM Problems:
link: https://github.com/raulmur/ORB_SLAM2.git

![imageofORBSLAM]()

This repository is built to save and analysis the data from Monucular ORB_SLAM for 3D environment reconstruction, motion recovery and frame correction.
After the running of ORB_SLAM, these data would be downloaded in several .TXT files. 

## Save data from ORB_SLAM:
I did some changes in source code to read and save the motion data like 3D position of Keyframes and Map-Points, Quaternion also 4*4 Camera Matrix for every frame to reover the orientations.

### KeyFrameTrajectory.txt :
this file save the motion data of every keyframe in sequence, the meaning of components in each line is:\
[TimeStamp, Coord.x, Coord.y, Coord.Z, Quater.x, Quater.y, Quater.z, Quater.w, [4*4 Camera Matrix]]

