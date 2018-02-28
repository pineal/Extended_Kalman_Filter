# Extended Kalman Filter
## Compilling
Build successfully with cmake and make.
Usage: ./ExtendedEKF under build.

## Accuracy
From the observation, RMSE meets the requirement RMSE <= [.11, .11, 0.52, 0.52].

## Follows the Correct Algorithm
- Sensor fusion algorhithm followed the general processing flow, processMeasurment function in fussionEKF.cpp and KalmanFilter class. 
- First measurement is taken care of by processMeasurement function, where a flag to indicate the first measurement and do neccessary initialization. - In processMeasurment function, an if condition to choose the right method for two sensor types lidar and radar has been addressed. 

## Code Efficiency
- Tried to optimize the time complexity, nothing significant madatory improvement has been found.