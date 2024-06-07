**Multi-class Classification**

To start with simple experiments that beforehand were expected to obtain good results, we used a dataset available on [GitHub](https://github.com/giulbia/baby_cry_detection.git) characterised by the clarity with which it represents the different sounds, including the plain one.


**Binary Classification**

The directory and [audio file system](data/Audios) that has been created with the [videos](data/Videos) and has the following five directories: 

  * **Unclassified**, this directory contains a total of 58 videos with different lengths and video formats. In the videos, medical personnel can be observed exposing the neonates to different stimuli. Sometimes the video contains a single stimulus, thus the shorter files, and on other occasions several stimuli which generates longer files.
  * **Severe_encephalopathy**, this directory contains a single video file of a newborn with severe signs of encephalopathy, which means that this baby does not cry at all when exposed to various stimuli. The video lasted 16 minutes and 54 seconds.
  * **Moderate_encephalopathy**, this directory contains a single file with a duration of 90.7 seconds. In it, the same stimulus with varying intensity, is repeated up to three times on the neonate, to test its response to the pain.
  * **Mild_encephalopathy**, this directory contains a single video file of a newborn baby exposed to different stimuli. Due to its long duration, audio was extracted and divided into a series of clips that represent each of the stimulations given to the newborn. This was to evaluate more precisely whether the models correctly classified the moments in which the newborn cried.
  * **No_encephalopathy**, this directory contains two video files of 89.4 and 55.08 seconds. These files contain the stimulations performed on two different babies. Due to their healthy state, their response to the presented stimuli is that of an intense cry.

