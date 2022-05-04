# Tensorflow Object Detection Walkthrough with Raspberry Pi
<p>The following repository will allow you to leverage Tensorflow Object Detection models that have been converted to TFLite on a Jetson.<p/>
## Steps
<br/>

<b>Step 1.</b>Install the required dependencies on the Jetson
<pre>
pip3 install opencv-python 
sudo apt-get install libcblas-dev
sudo apt-get install libhdf5-dev
sudo apt-get install libhdf5-serial-dev
sudo apt-get install libatlas-base-dev
sudo apt-get install libjasper-dev 
sudo apt-get install libqtgui4 
sudo apt-get install libqt4-testv
echo "deb https://packages.cloud.google.com/apt coral-edgetpu-stable main" | sudo tee /etc/apt/sources.list.d/coral-edgetpu.list
curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
sudo apt-get update
sudo apt-get install python3-tflite-runtime
</pre>
<br/>
<b>Step 2.</b> Copy your detect.tflite model into the same repository and update the labels.txt file to represent your labels. 
<br/><br/>
<b>Step 3.</b> Run real time detections using the detect.py script
<pre>python3 detect.py</pre>
<br/><br/>
