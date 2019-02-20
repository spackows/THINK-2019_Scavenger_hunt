# THINK-2019_Scavenger_hunt
Sample for THINK 2019 user experience session

## Demo videos

<table>
  <tr>
    <th>Indoor scavenger hunt BINGO</th>
    <th>San Francisco scavenger hunt BINGO</th>
  </tr>
  <tr>
    <td><a href="https://youtu.be/1u2qe3pJCyw" target="_other"><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/thumbnail-indoor.jpg" width="300px"/></a></td>
    <td><a href="https://youtu.be/6yKptg4t37s" target="_other"><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/thumbnail-san-fran.jpg" width="300px"/></a></td>
  </tr>
</table>

<p>&nbsp;</p>


## Instructions
These instructions describe how to build a scavenger hunt BINGO sample web app with given, indoor objects.

After you get the sample working, collect images of your favourite objects or tourist destinations and make your own scavenger hunt BINGO app!

<p>&nbsp;</p>


### Step 1: Collect training data

Download these 12 .zip files to your local computer:
- <a href="" target="other">bowl.zip</a>
- <a href="" target="other">brush.zip</a>
- <a href="" target="other">bucket.zip</a>
- <a href="" target="other">cup.zip</a>
- <a href="" target="other">glove.zip</a>
- <a href="" target="other">hickeytape.zip</a>
- <a href="" target="other">measuringtape.zip</a>
- <a href="" target="other">pig.zip</a>
- <a href="" target="other">puzzle.zip</a>
- <a href="" target="other">shoe.zip</a>
- <a href="" target="other">stapler.zip</a>
- <a href="" target="other">_nagative.zip</a>

#### About the sample training data

The sample training data includes 50 images of 11 indoor objects:

<table>
<tr>
  <td><b>bowl</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/indoor-scavenger-hunt-web-app/code/static/images/exemplars/bowl.png" width="100"/></td>
  <td><b>brush</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/indoor-scavenger-hunt-web-app/code/static/images/exemplars/brush.png" width="100"/></td>
  <td><b>bucket</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/indoor-scavenger-hunt-web-app/code/static/images/exemplars/bucket.png" width="100"/></td>
  <td><b>cup</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/indoor-scavenger-hunt-web-app/code/static/images/exemplars/cup.png" width="100"/></td>
  <td><b>glove</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/indoor-scavenger-hunt-web-app/code/static/images/exemplars/glove.png" width="100"/></td>
  <td><b>hockey tape</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/indoor-scavenger-hunt-web-app/code/static/images/exemplars/hockeytape.png" width="100"/></td>
</tr>
<tr>
  <td><b>measuring tape</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/indoor-scavenger-hunt-web-app/code/static/images/exemplars/measuringtape.png" width="100"/></td>
  <td><b>pig</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/indoor-scavenger-hunt-web-app/code/static/images/exemplars/pig.png" width="100"/></td>
  <td><b>puzzle</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/indoor-scavenger-hunt-web-app/code/static/images/exemplars/puzzle.png" width="100"/></td>
  <td><b>shoe</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/indoor-scavenger-hunt-web-app/code/static/images/exemplars/shoe.png" width="100"/></td>
  <td><b>stapler</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/indoor-scavenger-hunt-web-app/code/static/images/exemplars/stapler.png" width="100"/></td>
</tr>
</table>

The images include 7 different backgrounds:

<table>
<tr>
  <td><b>white</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/background_03.png" width="100"/></td>
  <td><b>yellow</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/background_07.png" width="100"/></td>
  <td><b>beige</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/background_12.png" width="100"/></td>
  <td><b>blue</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/background_18.png" width="100"/></td>
</tr>
<tr>
  <td><b>green</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/background_24.png" width="100"/></td>
  <td><b>black</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/background_34.png" width="100"/></td>
  <td><b>dark wood</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/background_47.270.png" width="100"/></td>
  <td><b>light wood</b><br/><img src="https://github.com/spackows/THINK-2019_Scavenger_hunt/raw/master/background_68.0.png" width="100"/></td>
</tr>
</table>

The file `_negative.zip` contains imags of only backgrounds, to be used as a negative class in training the model.

#### Tips and comments
- <p>With the IBM Watson Visual Recognition service, you can use images as small as 224 x 224 pixels with no loss of performance.  So, preprocessing training images to be 224 x 224  can make life easier (faster upload times, for example, than when using larger images.)</p>
- <p>The guidelines recommend to "make sure that the backgrounds in your training images are comparable to what you expect to classify."  In our scavenger hunt scenario, the run-time background might vary.  So, the sample training images include a varity of possible backgrounds.</p>
- <p>The guidelines recommend including at least 50 training images in each class.  (The sample training data here has 50 images for each class.)  Anecdotally, we have had success even with fewer images per class.  So if you don't have 50 images for one or more classes, try to train the model with what you have, because it might work well enough for you.</p>
- <p>Because objects might be in any orientation in a scavenger hunt scenario, the training data includes images of the objects positioned every which way.  For use cases where you know the run-time orientation of objects being classified, this might not be what you want to do.</p>
- <p>Anecdotally, including a negative class in training isn't always needed.  Experiment to determine what works best for your case.</p>
- <p>The guidelines recommend that the subject in the images take up at least 1/3 of the image.  In our case, we made a guess about where people playing a scavenger hunt would position their camera.  This meant that the measuring tape and hockey tape would be smaller in the training images than the other objects.</p>

See: [IBM Watson Visual Recognition guidelines for good training](https://console.bluemix.net/docs/services/visual-recognition/customizing.html#customizing-guidelines-training)

<p>&nbsp;</p>


### Step 2: Train a visual recognition model

<p>&nbsp;</p>


### Step 3: Prototype app code in a notebook

<p>&nbsp;</p>


### Step 4: Copy prototype code into a web app

