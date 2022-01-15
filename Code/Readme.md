
## How to use? 
<ol>
  <li>Clone the repository after preproeccsing to run and validate the model</li>
  <p><code>git clone https://github.com/ayerramsetti/Real-Time-Object-Detection-using-YOLO-V3.git</code></p>
</ol>
<ol start="2">
  <li>To install and Setup darknet</li>
  <p><code>!make</code></p>
 Next Clean all the data and cfg folders first except the labels folder present in data folder of darknet
</ol>
<ol start="3">
  <li>To Train the custom detector</li>
  <p><code>!./darknet detector train //path to data file bdd100k.data  //path to config file yolov3-tiny-bdd100k.cfg  //path to darkent layer-darknet53.conv.74 -dont_show -map</code></p>
 Check if there are any unloaded images, remove them and train the detector again using the same path mentioned above
</ol>
<ol start="4">
  <li>To Test the best mAP from the generated weights files after custom training</li>
  <p><code>!./darknet detector map //path to bdd100k.data //path to yolov3-tiny-bdd100k.cfg //path to yolov3-tiny-bdd100k_best.weights</code></p>
</ol>
<ol start="5">
  <li>To Test the custom detector</li>
  <p><code>!./darknet detector test //path to bdd100k.data //path to yolov3-tiny-bdd100k.cfg //path to yolov3-tiny-bdd100k_best.weights //path to test image -thresh 0.3</code></p>
</ol>
<ol start="6">
  <li>To view the Test Image</li>
  <p><code>imShow('predictions.jpg')</code></p>
</ol>
<ol start="7">
  <li>To detect the objects in Video</li>
  <p><code>!./darknet detector demo //path to bdd100k.data //path to yolov3-tiny-bdd100k.cfg //path to yolov3-tiny-bdd100k_best.weights -dont_show //path to test video -i 0 -out_filename //path to save final result video</code></p>
</ol>
