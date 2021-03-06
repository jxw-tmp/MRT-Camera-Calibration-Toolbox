# MRT Camera Calibration Toolbox [![Codacy Badge](https://api.codacy.com/project/badge/Grade/67ad4a269978453c836973f0d2b3e9f0)](https://www.codacy.com/manual/MT-MRT/MRT-Camera-Calibration-Toolbox?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=MT-MRT/MRT-Camera-Calibration-Toolbox&amp;utm_campaign=Badge_Grade)

## Introduction

The MRT Camera Calibration Toolbox is an application, developed in Python using OpenCV and tkinter, which determines the parameters of a camera's perspective projection by performing an intrinsic and extrinsic geometric calibration.

The application provides intrinsics, extrinsics and lens distortion parameters for each camera (two for stereo mode). For the stereo mode, the transformations between the individual camera coordinate systems are given as well. The information for each camera pose can be loaded using images or text files with the 2D points of the pattern. The calibration can be also made by using random subgroups from the total set of images. The computed parameters are the averaged over all iterations, and both the final results and the results per calibration can be exported to text files. 

## Reasons for using this Toolbox

-   Calibration of multispectral stereo camera systems
-   Calibration of camera systems with different resolutions
-   Visualization of the reprojection error
-   Image Cover Visibility
-   Statistical validation by means of calibration with subsets
-   Import and export of data
-   It's free!

## Requirements

To use the toolbox, the modules listed below have to be installed on your computer. 

-   Python3 (Tested for Python 3.4, Python 3.6 and Python 3.7)
-   OpenCV 4.1.0
-   tkinter 8.6
-   PIL 6.1.0
-   numpy 1.17.0
-   matplotlib 3.1.1

## Installation

You can download the source code and execute the toolbox [main.py](https://github.com/MT-MRT/MRT-Camera-Calibration-Toolbox/blob/master/main.py) directly on your computer through the Linux or Windows terminal:

```bash
cd path/to/your/toolbox
python3 main.py
```

## Getting Started

Check this animation of a running example of the MRT Camera Calibration Toolbox. 

![example](https://github.com/MT-MRT/MRT-Camera-Calibration-Toolbox/blob/master/docs/example_single_chessboard.gif)

## Documentation

Further information on the use of the Toolbox and the underlying calculations can be found in [this pdf](https://github.com/MT-MRT/MRT-Camera-Calibration-Toolbox/blob/master/docs/UserManual.pdf).

## Contributing 

Contributions are very welcome. Open a fresh issue to start a discussion around a feature idea or a bug.

## Acknowledgments

For [quaternions.py](https://github.com/MT-MRT/MRT-Camera-Calibration-Toolbox/blob/master/quaternions.py) code based on: Christoph Hagen. "averaging quaternions". Available here: [https://github.com/christophhagen/averaging-quaternions](https://github.com/christophhagen/averaging-quaternions)

Toolbar icons obtain from: [https://www.iconfinder.com](https://www.iconfinder.com)

## Citation

So far no publication has been written on the current toolbox, we recommend the following paper for citation of the geometric calibration of cameras in several spectral ranges:
```BibTeX
@INPROCEEDINGS{Schramm2020,
  author  = {Schramm, Sebastian and Rangel, Johannes and Aguirre Salazar, Daniela and Schmoll, Robert and Kroll, Andreas},
  title   = {Multispectral Geometric Calibration of Cameras in Visual and Infrared Spectral Range},
  doi     = {10.1109/JSEN.2020.3019959},
  note    = {accepted, Early Access},
  url     = {https://ieeexplore.ieee.org/document/9178752},
  journal = {IEEE Sensors},
  year    = {2020},
}
```

## Contact

If you have any questions, please email Daniela Aguirre Salazar at daguirres@unal.edu.co or Sebastian Schramm at sebastian.schramm@mrt.uni-kassel.de.

[Visit us](https://www.uni-kassel.de/maschinenbau/institute/mess-und-regelungstechnik/mrt.html)

<p align="center">
  <a href="https://www.uni-kassel.de/maschinenbau/institute/mess-und-regelungstechnik/mrt.html"><img src="https://github.com/MT-MRT/MRT-Camera-Calibration-Toolbox/blob/master/docs/MRT-Logo.png" alt="MRT" width="250"/>
</p>
