# rvr_ros
ROS node for interacting with [Sphero RVR](https://www.sphero.com/rvr).

Requires a Python 3-based ROS installation.

## Current functionality:

- Stream sensor data (locator, quaternion, gyroscope, velocity) from RVR and publish it to /odom, plus publish a TF from /odom to /base_link.

## Planned functionality:

- A launch file
- Subscribe to /cmd_vel and control the RVR's motors

## Known bugs:

- Doesn't exit on ^C, needs a ^\
- dependency on [sphero-sdk](https://pypi.org/project/sphero-sdk/) python package not encoded