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
## Making A Custom Aruco Model

Making a custom model is a little hard but using the files available in this repo might make it easier for you.

First download and install Blender https://www.blender.org/

Next open the sample.blend file available at the repo using blender blender

Now go to the material property of the aruco model and select the aruco image you want:
![blender_info](https://github.com/sacchinbhg/gazebo_aruco_models/assets/61612220/5c4ef22b-4046-4284-b04b-7d0fb771d99f)
