# PiCar: Autnomous Lane Navigation
________________________________________________________________________________________________________________________________________

## Overview 
________________________________________________________________________________________________________________________________________

This repository contains the notebook that sees the implementation and optimization of a convolutional network. The underlying task is to prediction two
quantities; steering angle and speed of a [SunFounder PiCar](https://www.sunfounder.com/smart-video-car-kit-v2-0.html). 

**Data collection**
<br>
The data collection was performed in segments, where each particular scenario of the final test enirvonment was targeted. The remote controlled car was manuvoured via external controls around the following tracks:
<br><br>
<img src="https://github.com/akinolawilson/PiCar-Autonomous-Lane-Navigation/blob/akinolawilson-sorting/ring_diagram.png?raw=true" width="200"/>
<br><br>
Where the following situation were consider:
- Clear ring
- Clear T-junction 
- Ring track with obsteciules 
- T-junction with traffic lights 
- T-junction without stationarity
<br><br>
In total, there are around 3000 training examples. The set is split using 70:20:10 ratio between the training, validation and evaluation sets. To investigate the raw datasets, please find them via [this link](https://drive.google.com/drive/folders/1YWuxnK8l4nPIidwyP39jph4pokjsmlE3?usp=sharing). 
<br><br>
## File content
________________________________________________________________________________________________________________________________________
**Data preparation**
<br><br>
The raw files are separated via their original collection. There are around 13 folders. The <ins>data_exploration.ipynb</ins> notebook contains the sortation and exploration of the folders content, preparing it for the training process and visualizing descriptive statistics.
<br><br>
**Modelling**
<br><br>
The  <ins>CNN_model.ipynb</ins> contains the fitting and optmization process of the CNN model. Tensorflows' hyperparameter API alongside the TensorBoard API has been used for the model optimization process. 
________________________________________________________________________________________________________________________________________
