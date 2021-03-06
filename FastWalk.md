[Home Page](https://github.com/TrackerLounge/Home)

[Digital Tracking Pit](https://github.com/TrackerLounge/DigitalTrackingPit)

# Fast Walk
This set of tracks is a fast walk.

<img src='/FastWalk/TopViewThreeBoxes_Small.JPG' width=800>

<img src='/FastWalk/threeFootPrintWithDistances.png' width=400>



# Track 00 is in wet sand

<img src='/FastWalk/Track00TopView_Small.JPG' width=800>

<img src='/FastWalk/track00InBlenderWithTexture_Small.JPG' width=800>

If you would like to take a look at the mesh in blender, the track.blend file can be downloaded from:
<a id="raw-url" href="https://raw.githubusercontent.com/TrackerLounge/DigitalTrackingPit/master/FastWalk/track00_textured_decimated_5.zip">Download FILE - track00_textured_decimated_5.zip</a>

For some purposes it may be easier to work with the model without the sand texture applied. For example, if you want to apply a shader based on elevation, having no texture is easier. See [Tracking and Edge Detection](https://github.com/TrackerLounge/TrackingAndEdgeDetection) and [Experiments with Image Processing, Computer Vision, and Machine Learning and Tracking](https://github.com/TrackerLounge/TrackingAndComputerVision)

<img src='/FastWalk/track00InBlender_Small.JPG' width=800>

If you would like to take a look at the mesh in blender, the untextured track.blend file can be downloaded from:
<a id="raw-url" href="https://raw.githubusercontent.com/TrackerLounge/DigitalTrackingPit/master/FastWalk/track00.zip">Download FILE - track00.zip</a>

If we were to cut the model into a thin strip along a line from the deepest point in the toe area to the deepest point in the heal area, it would look something like:

<img src='/FastWalk/track00CrossSectionFromToeToHeal.jpg' width=800>

We can see a nice disk crumble pressure release in this track.

If we were to cut the model into a thin strip along  the deepest point in the toe area from the pinky toe side to the big toe side, it would look something like:

<img src='/FastWalk/track00CrossSectionFromPinkyToeToBigToe.jpg' width=800>

Note: I had trouble with this cross section from pinky to big toe. It was hard to find the deepest point and even a small shift forward or back greatly changed the shape of the cross section.

# Track 01 is in dry loose sand

<img src='/FastWalk/Track01TopView_Small.JPG' width=800>

<img src='/FastWalk/track01InBlenderWithTexture_Small.JPG' width=800>

If you would like to take a look at the mesh in blender, the track.blend file can be downloaded from:
<a id="raw-url" href="https://raw.githubusercontent.com/TrackerLounge/DigitalTrackingPit/master/FastWalk/track01_textured_decimated_7.zip">Download FILE - track01_textured_decimated_7.zip</a>
Note: I had to decimate this to get it small enough to upload - it lost quality as a result.

<img src='/FastWalk/track01InBlender_Small.JPG' width=800>

If you would like to take a look at the mesh in blender, the track.blend file can be downloaded from:
<a id="raw-url" href="https://raw.githubusercontent.com/TrackerLounge/DigitalTrackingPit/master/FastWalk/track01_decimated_20.zip">Download FILE - track01_decimated_20.zip</a>

This track proves difficult to edge detect because it has a dish pressure release inside the borders of the track, and raising above the surrounding sand. At the same time it has a plate formation on the outside of the track, again rising above the surrounding sand. This creates a complex situation for edge detection and object segmentation and association from a computer vision perspective. 

If we were to cut the model into a thin strip along a line from the deepest point in the toe area to the deepest point in the heal area, it would look something like:

<img src='/FastWalk/track01CrossSectionFromToeToHeal.jpg' width=800>

We can see a nice dish pressure release in this track and a bit of a plate pressure release outside the track from pressure along the wall of the track.

If we were to cut the model into a thin strip along  the deepest point in the toe area from the pinky toe side to the big toe side, it would look something like:

<img src='/FastWalk/track01CrossSectionFromPinkyToeToBigToe.jpg' width=800>

If we were to color the untextured model along the Z-axis we would see:

<img src='/FastWalk/track01ColoredByZAxis_Small.jpg' width=800>

It is common in computer vision to search for edges of a track. For more on edge detection techniques see [Tracking and Edge Detection](https://github.com/TrackerLounge/TrackingAndEdgeDetection)

If we use [Fast Fourier Transform and Edge Detection](https://github.com/TrackerLounge/TrackingAndEdgeDetection/blob/master/FastFourierTransformAndEdgeDetection.md)
with settings 600 and 10, we get:

<img src='/FastWalk/track01ColoredByZAxis_Small_FFTEdge.jpg' width=800>

If we convolve the FFT binary image we see:

<img src='/FastWalk/track01ColoredByZAxis_Small_FFTEdge_Convolve.jpg' width=800>


# Track 02 is in wet packed sand

<img src='/FastWalk/Track02TopView_Small.JPG' width=800>

<img src='/FastWalk/track02InBlenderWithTextured_Small.JPG' width=800>

Unfortunately I could not upload the textured file to Github. I can upload a decimated file, if I decimated the model by a factor of 5, so that it is smaller than the 25 MB limit. <a id="raw-url" href="https://raw.githubusercontent.com/TrackerLounge/DigitalTrackingPit/master/FastWalk/track02_textured_decimated_5.zip">Download FILE - track02_textured_decimated_5.zip</a>

<img src='/FastWalk/track02InBlender_Small.JPG' width=800>

If you would like to take a look at the mesh in blender, the track.blend file can be downloaded from:
<a id="raw-url" href="https://raw.githubusercontent.com/TrackerLounge/DigitalTrackingPit/master/FastWalk/track02_decimated_20.zip">Download FILE - track02_decimated_20.zip</a>
Note: I had to apply a decimator modifier of type planer by a factor of 20 to reduce the number of verticies to make the file small enough to upload to github.

If we were to cut the model into a thin strip along a line from the deepest point in the toe area to the deepest point in the heal area, it would look something like:

<img src='/FastWalk/crossSectionFromToeToHeal.jpg' width=800>

We can see a nice dish pressure release in this track and a bit of a plate pressure release outside the track from pressure along the wall of the track.

If we were to cut the model into a thin strip along  the deepest point in the toe area from the pinky toe side to the big toe side, it would look something like:

<img src='/FastWalk/crossSectionFromPinkyToeToBigToe.jpg' width=800>


