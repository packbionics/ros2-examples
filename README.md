# ros2-examples
Example packages for ROS2 on Nvidia Jetson Nano

## py_pubsub
Taken from official ROS2 [tutorial](https://docs.ros.org/en/foxy/Tutorials/Writing-A-Simple-Py-Publisher-And-Subscriber.html#), this package contains two Python Nodes - Talker and Listener. The talker publishes a String message `"Hello World"`, while the listener receives them.

## Running the packages
One easy way to run ROS2 Nodes is to run a docker-compose file. In the `docker/` directory, there are example `docker-compose` files used to run multiple Docker containers, and each container can launch its own Nodes. Docker compose can be advantageous when there are multiple versions of ROS needed (even ROS2 + ROS1), or when the packages have conflicting dependencies.

### Example

Startup py_pubsub talker and listener:  
```docker-compose -f docker-compose.py_pubsub.yml up```
