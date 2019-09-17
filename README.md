# ffmpegso_linux_builds
FFMPEG builds for linux, .so file format for use with OpenCV camera video recorder and player

FFMPEG is the library that was made to support video format for video playing and recording. 

The purpose of making a standalone build for linux was to port ffmpeg to opencv when the required dependency in missing.
If OpenCV doesnot have ffmpeg in it, then:
                cap=cv2.VideoCapture()
                ret, frame = cap.read()
                            commands will not work, hence we will have to install ffmpeg in it.

This library combined with opencv.so forms a complete computer vision video analysis and rendering software that can be send
 to lambda for forming a microservice.
