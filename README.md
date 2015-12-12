# Kinect with OpenNI2

## OpenNI 2.2 + Nite 2.2 + Kinect SDK 1.8 + (windows 10) 32/64 bit 

### Install

a. Install Kinect SDK 1.8 

b. Install OpenNI 2.2 SDK 32bits / 64bits ( install both 64 bits and 32bits if u are using win64)

c. Install Nite 2.2 ( install both 64 bits and 32bits if u are using win64)

### Test

Run SimpleViewer.exe for Testing. It will be located at

64bits 
~ (OpenNI ) C:\Program Files\OpenNI2\Samples\Bin
~ (Prime Sensor) C:\Program Files\PrimeSense\NiTE2\Samples\Bin

32bits 
~(OpenNI ) C:\Program Files (x86) \OpenNI2\Samples\Bin
~ (Prime Sensor) C:\Program Files (x86) \PrimeSense\NiTE2\Samples\Bin


### Java JNI

Extract all dll.zip in the project folder. (./kinect-openni2 and ./kinect-openni2/lib/OpenNI2/Drivers)

OR

If you want to change the native library path, add the following and load the library OpenNI2.dll (directory to wherever it is on your machine or user loadLibrary() if you want a relative path)

```java

static {
    try {
        System.load("C:\\Program Files\\OpenNI2\\Redist\\OpenNI2.dll");
    }
    catch (Exception e)
    {
        e.printStackTrace();
    }
}

```

### Reference 

Installation Guide

https://www.youtube.com/watch?v=m5uTH3S9P9g

https://docs.google.com/file/d/0B3e4_6C5_YOjcmZpak12Q2MyZHM/edit?pli=1