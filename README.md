Usage:

## build & make

```
mkdir build
cd build
cmake ..
make
```

## run dji sample program

```
cd /Payload-SDK-master
sudo /build/bin/dji_sdk_on_jetson_cxx
```

## run & reason

Notice: TRT files must be matched with yolov5.yaml, including architecture, inputs and labels.
```
cd /Payload-SDK-master
sudo /build/bin/disease-detect /configs/yolov5.yaml /checkpoints/yolov5-e-coco.trt
```

## "sudo" without password
Add following contents in /etc/sudoers
$user_name is your user account
'''
$user_name  ALL=(ALL:ALL) NOPASSWD: ALL
'''
Then run dji_sdk_on_jetson_cxx without password

## refresh

send & receive messages on reasoning board

## unfinished

save & call messages from remoting controller
