# Videos-from-waggle-like-activity


As part of the process for the waggle dance detection we created four new videos in order to apply clustering in the raw, dense background video with pollen, honey and bees. 

First video -> Grayscale video, just conversion from coloured video to grayscaled one.

Second video -> GrayBlur, applied low-pass filtering with a Gaussian blur

Third video -> Thresholded, removing the background and thresholding 

Forth video -> FrameDiff, with the frame differencing the program checks the diferrences between two videoframes. To find any differences between the frames we needed the blur and threshold on the frames in order to district real movemnet form noise. Because frames could differ too when the light conditions from the video change and here we have a lot of changes, like camera autofocus, brightness correction etc. 

For further analysis I'm using the 'Thresholded' and 'FrameDiff' videos in order to extract informations like orientation, waggle frequency and spacial coordinates from each cluster.


NOTES: 
1. I saved the large contours in the detection in order to group eventually the clusters
2. On the videos there are a small delay for easier viewing (up to 1 sec)
3. We have more than 60000 video frames from the raw video
