<div align="center">
    <h1>Simple Lidar Simulator</h1>
</div>

## :open_file_folder: What's in this repo

* Python launch file
* Yaml params file with all customisable parameters
* Models foulder for car and cones .stl models
* Track foulder with .csv file with the internal side of a test track (no mid-track)

## :package: Prerequisite packages
> What we need are ros2, gazebo fortress, pandas and numpy.

```commandline
sudo apt-get install python3-numpy python3-pandas -y
```
## :gear: How to build & Run
```commandline
mkdir ros2_ws/src
cd ros2_ws/src
git clone https://github.com/leonardonels/simulator_project
cd ..
colcon build --packages-select simulator_project --symlink-install
```
```commandline
ros2 launch simulator_project simulator_launch.py
```
![Screenshot from 2025-01-31 21-59-21](https://github.com/user-attachments/assets/343c7e04-40dd-4dab-8bff-37520b708268)

![Screenshot from 2025-01-31 22-01-26](https://github.com/user-attachments/assets/b83116c2-6654-4973-a4c8-35ecabcbc5de)

---

## Todo List
- [ ] Modify the lidar sensor to have a variable density of points
- [ ] Fine-Tuning lidar settings
- [ ] Apply the true model for the car
- [ ] Improve performance
