```bash
echo "deb [trusted=yes] https://raw.githubusercontent.com/isys-vision/ros-one-moveit-overlay/jammy-one/ ./" | sudo tee /etc/apt/sources.list.d/isys-vision_ros-one-moveit-overlay-jammy-one.list
sudo apt update
sudo apt install python3-rosdep2
echo "yaml https://raw.githubusercontent.com/isys-vision/ros-one-moveit-overlay/jammy-one/local.yaml debian" | sudo tee /etc/ros/rosdep/sources.list.d/1-isys-vision_ros-one-moveit-overlay-jammy-one.list
rosdep update
```
