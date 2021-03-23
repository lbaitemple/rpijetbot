# rpijetbot

```
sudo apt update && sudo apt upgrade -y
sudo apt-get install -y i2c-tools git
sudo raspi-config
```

setup I2C

```
sudo apt-get install build-essential cmake unzip pkg-config -y 
sudo apt-get install libjpeg-dev libpng-dev libtiff-dev -y
sudo apt-get install libavcodec-dev libavformat-dev libswscale-dev libv4l-dev -y
sudo apt-get install libxvidcore-dev libx264-dev -y
sudo apt-get install libgtk-3-dev -y
sudo apt-get install libcanberra-gtk* -y
sudo apt-get install libatlas-base-dev gfortran -y
sudo apt install python3-gst-1.0

```
Install OpenCV (https://github.com/ys7yoo/PiOpenCV)
```
https://gist.githubusercontent.com/sickate/062c7b236fc35915249b55bceb51e3a7/raw/0d13f297af6fa149b46f52b62c888701ab24000b/install_cv.sh
chmod +x install_cv.sh
./install_cv.sh
```
