# COMP 498 - Project
Steve Ferreira, 27477546  
Section: Winter 2018 - GG  
Date: March 20, 2018  

**I certify that this submission is my original work and meets the Faculty's Expectations of Originality.**

## Prequisits
- OpenCV
- C++ 11
- CMake
- Make

## Compilation instructions

**This project uses the C++11 standard, and you will need a recent compiler capable of supporting these features.**

This project uses CMake >=3.5 (https://cmake.org/) to generate build files for any platform. It can be installed on Linux or macOS using a package manager, or Windows using the official installer. Ensure it is added to your system PATH and accessible via command line.

Then, CMake can be used in the command line to generate build files for any environment desired.

1. `cd [path to assignment]`
2. `mkdir build`
3. `cd build`
4. `cmake -G "your generator here" ..`
    - Run `cmake -G` to see a list of possible generators, eg. `Xcode`, `Unix Makefiles`, versions of Visual Studio, etc.
5. Build the project using whichever build system you chose.

## Objectives
1. Implement [Harris Corner Detection](https://en.wikipedia.org/wiki/Harris_Corner_Detector) algorithm.
2. Implement simple keypoint descriptor based on [SIFT](https://en.wikipedia.org/wiki/Scale-invariant_feature_transform).
3. Find matching keypoint descriptors between two images.
4. Determine [Homography](https://en.wikipedia.org/wiki/Homography_(computer_vision)) for stitching using [RANSAC](https://en.wikipedia.org/wiki/Random_sample_consensus).
5. Stitch images together.

## Results
### Matching Keypoints
![Raw Matches][raw]
### Refined Inlier Matches
![Refined Matches][refined]
### Final Panorama
![Final Result][final]

## Notes
This assignment has been tested on Linux, using OpenCV 3.4.0, CMake 3.10.2, Make 4.2.1

[raw]: https://github.com/Shmeve/image-stitching/blob/master/results/README/Step_1_and_2.png?raw=true
[refined]: https://github.com/Shmeve/image-stitching/blob/master/results/README/Step_3.bmp?raw=true
[final]: https://github.com/Shmeve/image-stitching/blob/master/results/README/Step_4.bmp?raw=true
