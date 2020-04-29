# PedNet
Object detection optimized specifically for pedestrians, cyclists, and vehicles on edge/mobile hardware. Below is a comparison between Mobilenet V1 and PedNet.

<p float="left">
  <img src="docs/vid01_pednet.webp" width="430">
  <img src="docs/vid01_mobilenet.webp" width="430"> 
</p>

### Usage
Within the `model/` directory there are two versions of PedNet; one that's been compiled for the Coral TPU, and one for TensorFlow Lite.

<b>TF Lite</b>: To use this version, simply install the TensorFlow Lite interpreter library which can be found [<a target="_blank" href="https://www.tensorflow.org/lite/guide/python">here</a>]. If you're installing this on a Raspberry Pi running Raspbian Buster make sure to use the Python wheel built for Linux (ARM 64) and Python 3.7 which can achieved with the following: 
```sh
pip3 install https://dl.google.com/coral/python/tflite_runtime-2.1.0.post1-cp37-cp37m-linux_armv7l.whl
```

<b>Coral TPU</b>: In order to utilize the Coral TPU, the Edge TPU runtime and TensorFlow Lite interpreter library must be installed. The TensorFlow Lite installation is the same as above, and the Edge TPU can be installed by following the directions [<a target="_blank" href="https://coral.ai/docs/accelerator/get-started/#requirements">here</a>].



### Model versions
| model | architecture | cpu | tpu | pedestrians | cyclists | vehicles | e-scooters |
|---|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| pednet_20200326 | mobilenet ssd v1 | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ❌ | 
| coming soon | ? | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | ✔️ | 

### Training data
| class | imgs (#) | annotations (#) |
| --- | --- | --- |
| bicycle | 255 | 550 |
| pedestrian | 296 | 2856 |
| vehicle | 1242 | 8715 |
| e-scooter | --- | --- |

### Performance
coming soon...
