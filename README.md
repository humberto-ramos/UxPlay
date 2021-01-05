This project is an early stage prototype of unix AirPlay server.
Work is based on https://github.com/FD-/RPiPlay.
Tested on Ubuntu 19.10 desktop.
5G Wifi connection is the must.

Features:
1. Based on Gstreamer.
1. Video and audio are supported out of the box.
3. Gstreamer decoding is plugin agnostic. Uses accelerated decoders if availible. VAAPI is preferable.
4. Automatic screen orientation.

Building:
1. sudo apt-get install cmake
2. sudo apt-get install libssl-dev libavahi-compat-libdnssd-dev libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev gstreamer1.0-libav
3. sudo apt-get install gstreamer1.0-vaapi (For Intel graphics)
4. mkdir build
5. cd build
6. cmake ..
7. make

Also install the following packages

sudo apt install git cmake libssl-dev libplist-dev libavahi-compat-libdnssd-dev libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev gstreamer1.0-plugins-base gstreamer1.0-plugins-good gstreamer1.0-plugins-bad gstreamer1.0-plugins-ugly gstreamer1.0-libav gstreamer1.0-vaapi

Try it out and see if it runs. If not, try installing these 

sudo apt install gstreamer1.0-doc gstreamer1.0-tools gstreamer1.0-x gstreamer1.0-alsa gstreamer1.0-gl gstreamer1.0-gtk3 gstreamer1.0-qt5 gstreamer1.0-pulseaudio
