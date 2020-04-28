# PedNet
Object detection optimized specifically for pedestrians, cyclists, and vehicles on edge/mobile hardware. Below is a comparison between Mobilenet V1 and PedNet.

<img src="docs/vid01_pednet.webp">
<img src="docs/vid01_mobilenet.webp">

### Usage
coming soon...

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
