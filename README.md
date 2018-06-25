# EKF -Extended Kalman Filters in C++
Udacity CarND Term 2, Project 1 - Extended Kalman Filters

## Project Basics
The main goal of the project is to apply Extended Kalman Filter to fuse data from LIDAR and Radar sensors of a self driving car using C++. The code will make a prediction based on the sensor measurement and then update the expected position.

See the starter code from Udacity Project 
[Starter Code](https://github.com/udacity/CarND-Extended-Kalman-Filter-Project)

## Basic Build Instructions
1. Clone this repo.
2. Make a build directory: mkdir build && cd build
3. Compile: cmake .. && make
	On windows, you may need to run: cmake .. -G "Unix Makefiles" && make
4. Run it: ./ExtendedKF

## Contents of Repository
- src dir
	1. main.cpp - communicates with the Term 2 Simulator receiving data measurements, calls a function to run the Kalman filter, calls a function to calculate RMSE
	2. FusionEKF.cpp - initializes the filter, calls the predict function, calls the update function
	3. kalman_filter.cpp- defines the predict function, the update function for lidar and the update function for radar
	4. tools.cpp- function to calculate RMSE and the Jacobian matrix
- data - a directory with one input file, provided by Udacity
- results - a directory with output and log files
- Docs - a directory with files formats description

## Results
![Laser-Radar-Output-Dataset1](https://github.com/vikasmalik22/EKF/blob/master/results/ekf_output1.png)

![Laser-Radar-Output-Dataset2](https://github.com/vikasmalik22/EKF/blob/master/results/ekf_output2.png)