# RealSense-TouchDesigner-particle
It is a Rnd project to use Intel RealSense with TouchDesigner for tracking and particle system on 3d model.

## Usage

#### Download RealSense Software
Install RealSense Viewer  
Install firware through viewer

## How it works

### Depth Image
Using depth image from camera to create trail.

### Particles
There are 2 sources connected to particle operators.
- model
- trail

### Tracking position
The shuffled CHOP data from trail position will be applied on force and trail particle itself. And this value will be normallized with lag operators.  

### Modes
There are 2 modes in this project, one is "idle", other is "play". You can check this modes from op("manager_script"). And functions from there will be called from CHOP execute.
