# Real-time finger counting

This is an example project from our master programme in vision and robotics [Vibot](http://www.vibot.org) for Real-time image processing module.
We used Celoxica RC10 board with Xilinx FPGA and coded in Handel C with PixelStreams library.

<iframe width="425" height="325" src="//www.youtube.com/embed/oemHAE98QHM" frameborder="0" allowfullscreen></iframe>

The approximate pipeline (from what I recall):
 - segmentation of hand wearing a color glove is done by color thresholding in two color spaces
   - the hand/glove color segmentation can be calibrated with a button press on the board
   - also threshold for image visualization on the screen can be chosen with joystick
 - rectangular region of interest (ROI) is fit to the hand
 - closed fist, open hand showing or not showing thumb are detected by width/height ratios
 - at some fixed positions of the ROI, horizontal scan lines are counting the number of crossed fingers


[PixelStreams] http://www.mentor.com/products/fpga/handel-c/pixelstreams)
[Celoxica RC 10 board](http://teal.gmu.edu/courses/ECE448/documentation/RC10%20Manual.pdf)