# **Simple Localization based on Extended Kalman Filter**
---

## Introduction

_**Note:** This project makes use of  [Udacity Extended Kalman Filter Starter Code](https://github.com/udacity/CarND-Extended-Kalman-Filter-Project) and Udacity Workspace. The simulator and data are not included in this repository and can be found in the link above._
In this project, a simple extended Kalman filter(EKF) is implemented to acquire position of a moving vehicle in the simulator provided by Udacity with C++. Noisy LIDAR and RADAR is provided in the form of x and y position measurements in the simulator. By fusing the LIDAR and RADAR  data, the estimated position is obtained and compared to the actual ground truth to calculate the final RMSE.

## Compiling and running simulator

1. Clone the repository and change directory into the repository folder
2. Create new folder, build `mkdir build`
3. Change directory into the newly built folder, build `cd build`
4. Compile `cmake ..`
5. `make`
6. Execute the generated file `./ExtendedKF`


**INPUT**: values provided by the simulator to the c++ program

["sensor_measurement"] => the measurement that the simulator observed (either lidar or radar)


**OUTPUT**: values provided by the c++ program to the simulator

["estimate_x"] <= kalman filter estimated position x

["estimate_y"] <= kalman filter estimated position y

["rmse_x"]

["rmse_y"]

["rmse_vx"]

["rmse_vy"]

---

## Dependencies

* cmake >= 3.5
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)
