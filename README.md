# Rppg_monitoring
The goal of this project is to optimize rPPG for continuous and unobtrusive monitoring. Adaptive skin identification for ROI denition in rPPG is investigated in this study, and the results are compared to our prior real-time rPPG-based technique.



you need to install _:'
-scipy
-dlib
-imutils
-numpy
-opencv-python
-PyQt5
-pyqtgraph


*there is a video attatched that show the operation and the results*

**introduction 
here is no doubt that monitoring vital signs and supervising
our health statue is very necessary and critical thing,
especially important organs in our body like our heart,
that could be considered as the engine of the whole body and
we can deduce alot from its condition through many
parameters, one of the most important of parameter is the heart
rate.
It’s known that there is some traditional methods to measure
the heart rate, such as Electrocardiography (ECG that offers
most accurate HR measurement, but require attaching medical
electrodes to the person also pulse oximeter which based on
photoplethysmography (PPG), must be attached to body
part, like toes or an earlobe. Although these methods are
efficient it also needs a high cost and it’s kind of hard to reach,
especially according to the current quarantine situations. So the
orientation now is going to the contactless camera based
monitoring which called remote photoplethysmography
(RPPG)


Methodology steps :- 

-Raw Signal Extraction
In this step we are trying to extract the first two methods, here
we trying to define the face of the person that setting in front
of the camera and then tracking his face in each frame for a 10
second after this step we should had extracted the row RGB
signal(changing in his skin color for each frame) that will be
after processed and extract the persons heart rate.

-Face detection
To get an accurate face detection Viola Jones technique or
Liao technique is used in this step the face of the person will
be detected and will be a bounding box around person’s face

-Face tracking
Whatever it’s very complex, time and resources wasting to
detect the person’s face on each frame for a 10 second, also it
will cause unwanted noise for each frame, so instead of
redetect the face we use KLT tracker in which a special points
of the face are tracked for each frame.


CHOOSING ROI
Used the returned skin pixel from the last
step to get rid of background noise,
which is the drawback of this approach.
Then choosing the most suitable
region of interest (ROI)


CONSTITUTE TEMPORAL RGB SIGNALS

FAST FOURIER TRANSFORM (FFT)

Peaks Detection



CONSTITUTE TEMPORAL RGB SIGNALS
