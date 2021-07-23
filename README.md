# UAV-Eagle dataset

This repository contains the UAV-Eagle dataset accompanying the paper "Brain over Brawn - Using a Stereo Camera to Detect, Track and Intercept a Faster UAV by Reconstructing Its Trajectory".

The UAV-Eagle dataset contains 510 annotated images of our custom quadcopter Eagle in an unconstrained environment. This dataset is quite challenging due to the presence of illumination changes, motion effects, changes in viewpoint, and the presence of various objects in the background. The dataset can be used as a testbed for the detection of UAVs, demonstrating the robustness of the detector in real-world conditions and the ability to detect a previously unseen object of interest.

The UAV-Eagle dataset is available [here](https://drive.google.com/drive/folders/1hj6-H6DaqPVJ89fErsB4hi9atHF7RCoD?usp=sharing) or by running ``` ./download_uav_eagle.sh ``` in terminal.

If you use this dataset for your research, please cite the preprint:
```
@misc{barišić2021brain,
      title={Brain over Brawn - Using a Stereo Camera to Detect, Track and Intercept a Faster UAV by Reconstructing Its Trajectory}, 
      author={Antonella Barišić and Frano Petric and Stjepan Bogdan},
      year={2021},
      eprint={2107.00962},
      archivePrefix={arXiv},
      primaryClass={cs.RO}
}
```

## Dataset

The directory is organised as follows:

```
UAV-Eagle/
  ├──images/
  |  ├── frame0000.jpg
  |  ├── frame0001.jpg
  |  ├── ...
  └──labels/
     ├── frame0000.txt
     ├── frame0001.txt
     ├── ...

```
For each image there is a ```.txt``` file with the same filename containing annotations in the YOLO format: ```<object-class> <x> <y> <width> <height>```. Note: ```<x> <y>``` is the center of the bounding box and all values are normalised.

Example of detection on the dataset:

<img src="https://user-images.githubusercontent.com/26712043/110366460-991fdb80-8046-11eb-83cd-ad2a378dbca8.jpg" width="415"/> <img src="https://user-images.githubusercontent.com/26712043/110366462-9a510880-8046-11eb-83a3-7a9316968e64.jpg" width="415"/> 

## Contact

For more information, please contact [Antonella Barisic](mailto:antonella.barisic@fer.hr).
