# video-compression-artifact-visualizer

A demonstrative notebook that shows how, under unfavorable conditions, even light amounts of video compression may affect the accuracy of machine learning models. 

The video I used for testing is [Ampulla Pluto DashCam Sample / Night Rain City](https://www.youtube.com/watch?v=ZfqXfaB4Qj8) (although I think that any video with a convoluted/noisy environment should be sufficient). I used a short video to reduce processing time since I used Colab's CPU.

For object detection, YOLOv8 is used. On the original video, it is able to (correctly) detect 3 objects, but only 1 object from the compressed video. 

This demonstrates the importance of VCM (Video Coding for Machines) to prevent the loss of relevant information for ML models.

To do:
- Use SR models on the compressed videos and run them through YOLO to compare the results.
