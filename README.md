# Playground
A python library consisting of pipelines for visual analysis of different sports using Computer Vision and Deep Learning.

### Update : Badminton detector for Videos has been added. Note: There are some FPS issues in the video detector. We will resolve them soon!

### Update : FPS improvement achieved with Tiny YOLO

## To setup project, open up a new terminal and enter the following:
```
sh setup_conda.sh
```
OR
```
sh setup_pip.sh
```

## To test, simply open up a new terminal and enter the following code:
```
# For singe image:

from Badminton.Badminton import Detector
obj = Detector()
obj.detect_players_image("Badminton/images/bad.jpg")



# For video:

from Badminton.Badminton import Detector
obj = Detector()
obj.detect_players_video("Badminton/images/video.mp4")


# For using tiny yolo for better FPS:
# For video:

from Badminton.Badminton import Detector
obj = Detector(tiny=True)
obj.detect_players_video("Badminton/images/video.mp4")

```
