# CameraServer application
This project consists of two pieces.

It uses [gstreamer](https://gstreamer.freedesktop.org/download/) to obtain the raw MJPEG stream from a USB camera.  It publishes that raw stream to TCP port 9999.  See the stream-camera command files for the command line constructed to do this.

Then, it publishes a python command line utility called ipcamera that takes the raw MJPEG stream and reformats into an MJPEG stream over HTTP.  It publishes that stream to port 1337 with the URL endpoint of /mjpeg_stream.

The command line utility is built, using `gradlew build`, into a pip package and is located in the ./build/python/dist directory.

# Dependencies
1. Python3
2. gstreamer

# Credits
1. [http://synack.me/blog/implementing-http-live-streaming](http://synack.me/blog/implementing-http-live-streaming)
2. [https://gist.github.com/sakti/4761739](https://gist.github.com/sakti/4761739)

Vision processing on desktop for simulation and network tables
https://www.youtube.com/watch?v=QIGn90hKnv8

Pi Vision including setup, project build and deploy. Don’t forget to change the hostname!! **** VERY USEFUL!!!
Part 4 pulls everything together including an application pushing data to network tables.
Part 5 is code analysis. 
Part 6 - GRIP
Part 7 - Debugging
https://github.com/Team997Coders/BB2018BallFindingVision
https://www.youtube.com/watch?v=Zgt2vMSxNbs
