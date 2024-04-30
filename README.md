This code is designed for the ECE 4180 GPS Car Project and uses the mbed platform to navigate a vehicle autonomously. It integrates various components such as a GPS module, a digital compass (LSM9DS1 IMU), and motor drivers. The software incorporates libraries for interfacing with the hardware and managing tasks within a real-time operating system (RTOS). It handles the asynchronous reading of GPS data, processes this data to pinpoint the vehicle's current location, and computes the direction in which the vehicle needs to move.

<img width="583" alt="image" src="https://github.com/cammarcil/4180-final-gps/assets/114452492/88aa3bb7-c26e-4458-a530-1d80365af382"># 4180-final-gps

The system calculates the vehicle's exact position by decoding GPS data and applies a moving average filter to smooth out location readings, enhancing accuracy. This processed data is used to continuously update the vehicle’s travel path towards designated waypoints. The navigation logic includes functions that calculate the direction and distance to these waypoints and adjust the vehicle’s trajectory accordingly.

In the navigation code, mathematical formulas are used to determine bearings and distances between coordinates, and to adjust the vehicle’s orientation based on the compass readings. The point() function is crucial here, managing the vehicle’s steering by adjusting motor speeds to align with the correct heading. This function checks and corrects the vehicle's heading dynamically, ensuring it stays on the planned route. The entire program demonstrates how geometric calculations and control mechanisms can be implemented in real-time systems for effective autonomous navigation.


<img width="648" alt="image" src="https://github.com/cammarcil/4180-final-gps/assets/114452492/daa2401c-d16a-45d8-aea0-1f539b825a38">


