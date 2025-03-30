sudo python3 -m pip install imutils
sudo python3 -m pip install pyrf24
sudo apt-get install python3-opencv
---
load runtime về:  wget https://raw.githubusercontent.com/diy-hus/coral/main/tflite_runtime-2.5.0.post1-cp39-cp39-linux_armv7l.whl
hoặc từ trang chủ
https://github.com/google-coral/pycoral/releases/download/v2.0.0/tflite_runtime-2.5.0.post1-cp39-cp39-linux_armv7l.whl
sudo python3 -m pip install tflite_runtime-2.5.0.post1-cp39-cp39-linux_armv7l.whl

echo "deb https://packages.cloud.google.com/apt coral-edgetpu-stable main" | sudo tee /etc/apt/sources.list.d/coral-edgetpu.list
curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
sudo apt update
sudo apt install libedgetpu1-stdw
sudo raspi-config > enable camera
