# Driver Drowsiness Detection using OpenCV in Python
I have built an application that will detect the drowsiness of a driver and alert the driver before any fatal incident occurs.
<br />
<br />
The project is divided into two modules – **Eye Detection** and **lane Detection**

## **Eye Detection:**
In this module I applied Face Landmark Recognition (68-point landmark detectors: This pre-trained landmark detector identifies 68 points ((x,y) coordinates) in a human face. These points localize the region around the eyes, eyebrows, nose, mouth, chin and jaw) and extract only the eye region. With the eyes I computed EAR (Eye Aspect Ratio), this indicates whether the eyes are closed for sufficient amount of time, if closed then alarm goes on.

## **Lane Detection:**
To make the system more efficient, I have added lane detection. The alarm will go on if any deviation is detected.
## **The flow of the project is as follows:**
**Step 1:** Setup a camera that monitors a stream for faces, if a face is found, we apply facial landmark detection and extract the eye regions.<br />
<br />
**Step 2:** We calculate the EAR and indicate whether the eyes are closed or open. <br />
<br />
**Step 3:** Setup a camera that monitors the lane and check for any deviation. <br />
<br />
**Step 4:** If the eyes are closed the alarm will go on or if eyes are closed and there is 
        any deviation in the lane the alarm will go on. 


