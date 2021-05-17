# Line-Following-Robot
The line follower is a self-operating robot that detects and follows a line that is drawn on the floor. The path consists of a black line on a white surface (or it may be reverse of that. The control system used must sense a line and maneuver the robot to stay on course, while constantly correcting the wrong moves using feedback mechanism, thus forming a simple yet effective closed loop System. The robot is designed to follow very tight curves. 

The basic operations of the line follower are as follows:
1-Capture line position with optical sensors mounted at front end of the robot. For this a combination of IR LED’s and Photo Transistor called an opto- coupler is used. The line sensing process requires high resolution and high robustness.
2-Steer robot to track the line with any steering mechanism. To achieve this we use two motors governing wheels motion.
