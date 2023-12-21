# Aruco Models for Gazebo World

## Basic Information

Aruco Dictionary: cv2.aruco.DICT_6X6_100

Size: 2 meters X 2 meters

Aruco made from https://chev.me/arucogen/

## Use

Clone the repository:
```bash
git clone https://github.com/sacchinbhg/gazebo_aruco_models.git
```

We need to copy the marker to the gazebo model folder, I am going to be using marker 0 as an example please use whichever you are going to use:
```bash
sudo cp -r marker_0/ /usr/share/gazebo-11/models/
```

Now in any model file include the marker using:
```xml
<include>
  <uri>model://marker_0</uri>
  <pose>0 0 10 3.14 0 3.14</pose>
</include>
```
