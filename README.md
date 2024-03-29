# rpijetbot
Jetbot https://developer.nvidia.com/embedded/jetpack

```
git clone https://github.com/lbaitemple/rpijetbot/
cd ~/rpijetbot
```

Image download at 

http://jetbot.org/v0.4.3/software_setup/sd_card.html

```
sudo apt update && sudo apt upgrade -y
sudo apt-get install -y i2c-tools git
sudo raspi-config
```
Pytorch Install
```
sudo apt install libopenblas-dev libblas-dev m4 cmake cython python3-dev python3-yaml python3-setuptools -y
mkdir pytorch_install && cd pytorch_install
git clone --recursive https://github.com/pytorch/pytorch
cd pytorch
pip3 install typing_extensions

export NO_CUDA=1
export NO_DISTRIBUTED=1
export NO_MKLDNN=1 
export NO_NNPACK=1
export NO_QNNPACK=1

python3 setup.py build
python3 setup.py sdist bdist_wheel
sudo -E python3 setup.py install
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

Pytorch
```
sudo apt install libopenblas-dev libblas-dev m4 cmake cython python3-dev python3-yaml python3-setuptools python3-wheel python3-pillow python3-numpy -y

wget https://raw.githubusercontent.com/nmilosev/pytorch-arm-builds/master/pytorch-arm64.sh
```

#### tensorflow light
```
pip3 install https://github.com/bitsy-ai/tensorflow-arm-bin/releases/download/v2.4.0/tensorflow-2.4.0-cp37-none-linux_armv7l.whl
```

### Install node-red
```
bash <(curl -sL https://raw.githubusercontent.com/node-red/linux-installers/master/deb/update-nodejs-and-nodered)
node-red-pi --max-old-space-size=256

```

```
sudo apt install libqtgui4   libilmbase-dev libopenexr-dev libgstreamer1.0-dev  -y
sudo apt-get install -y gstreamer1.0-plugins-bad gstreamer1.0-plugins-good python3-gst-1.0 python3-gi gobject-introspection gir1.2-gtk-3.0 python3-numpy
sudo  pip3 install opencv-contrib-python==4.1.0.25
```
ref

https://eide.ai/rpi4/pytorch/2020/06/30/pytorch-raspberry.html

https://qengineering.eu/install-tensorflow-2.2.0-on-raspberry-64-os.html

https://qengineering.eu/install-opencv-4.3-on-raspberry-64-os.html
