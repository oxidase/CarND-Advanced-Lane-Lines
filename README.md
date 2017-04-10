## Advanced Lane Finding
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)


The project goal is to write a software pipeline to identify the lane boundaries in a video,
but the main output is a detailed writeup of the project.

The Project
---

The goals / steps of this project are the following:

* Compute the camera calibration matrix and distortion coefficients given a set of chessboard images.
* Apply a distortion correction to raw images.
* Use color transforms, gradients, etc., to create a thresholded binary image.
* Apply a perspective transform to rectify binary image ("birds-eye view").
* Detect lane pixels and fit to find the lane boundary.
* Determine the curvature of the lane and vehicle position with respect to center.
* Warp the detected lane boundaries back onto the original image.
* Output visual display of the lane boundaries and numerical estimation of lane curvature and vehicle position.

The images for camera calibration are stored in the folder called `camera_cal`.
The images in `test_images` are for testing pipeline on single frames.
Test images also extracted from video files as
```
ffmpeg -i project_video.mp4  project_video/%04d.jpg
ffmpeg -i challenge_video.mp4  -r 1/1 challenge_video/%04d.jpg
ffmpeg -i harder_challenge_video.mp4 harder_challenge_video/%04d.jpg
```

The [write up about processing pipeline](./writeup.pdf) describes the pipeline in details.

The output project video
---

[![Project video](http://img.youtube.com/vi/DHH_G5XM7T8/0.jpg)](http://www.youtube.com/watch?v=DHH_G5XM7T8 "Project output video")
