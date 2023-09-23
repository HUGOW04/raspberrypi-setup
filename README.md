# raspberrypi-setup

git clone https://github.com/raspberrypi/pico-sdk.git

mkdir pico

cd pico

cp ~/pico-sdk/external/pico_sdk_import.cmake .

mkdir build 

cd build

export PICO_SDK_PATH=../../pico-sdk

make

