# EVO

Matlab/C++ implementation of Event-Based Multi-View Stereo (mapping half of Event-Based Visual Odometry, i.e. using ground truth poses for localization). 

<center>
<img src="doc/results/office_depth_map_kf1.png" width="400"/>
</center>

**Note**: After we worked on this project, the authors of the paper published [source code for EMVS](https://github.com/uzh-rpg/rpg_emvs). They have also compiled a helpful [list of resources for event-based vision](https://github.com/uzh-rpg/event-based_vision_resources).  

### Prerequisites

_Matlab_: standalone - just need to get data.

_ROS node_ (work in progress):

* OpenCV
* Eigen
* [rpg_dvs_ros](https://github.com/uzh-rpg/rpg_dvs_ros)

### Data

Get datasets from University of Zurich's [Event-Camera Dataset].

_Matlab_: download data in txt format, and run ExtractData on it to get a mat file.

_ROS node_: download rosbag to data folder and point emvs.launch to it.

### Running

_Matlab_: Run EMVS.m

_ROS node_: `roslaunch evo emvs.launch`

### Authors

* Max Hu
* Aum Jadhav
* Benjamin Kuo
* Cyrus Liu
* Maitreya Naik
* Kazu Otani

### References

* Rebecq, Henri, Guillermo Gallego, and Davide Scaramuzza. ”EMVS: Event-based Multi-View Stereo.” British Machine Vision Conference (BMVC). No. EPFL-CONF-221504. 2016.

* Henri Rebecq, Timo Horstschaefer, Guillermo Gallego, Davide Scaramuzza, "EVO: A Geometric Approach to Event-based 6-DOF Parallel Tracking and Mapping in Real-time," IEEE Robotics and Automation Letters (RA-L), 2016.

* Gallup, David, et al. ”Real-time plane-sweeping stereo with multiple sweeping directions.” Computer Vision and Pattern Recognition, 2007. CVPR’07. IEEE Conference on. IEEE, 2007

* [event-based_vision_resources](https://github.com/uzh-rpg/event-based_vision_resources) from UZH group
* [Image Reconstruction from an Event Camera](https://github.com/uzh-rpg/rpg_image_reconstruction_from_events) - also from UZH
