# Cozmo what is this
fork from [rizal72/Cozmo-Voice-Commands](https://github.com/rizal72/Cozmo-Voice-Commands)

### About Cozmo-What-Is-This
Add a new command to [Cozmo-Voice-Commands](https://github.com/rizal72/Cozmo-Voice-Commands): `Cozmo, what is this`, then cozmo will tell you what it saw

![](http://oav6fgfj1.bkt.clouddn.com/cozmodc8e1dad.png)

```
- Cozmo, what is this 
- I'm thinking! Oh, it is the coffee mug.
```

The project use [Inception-v3 model](https://www.tensorflow.org/tutorials/image_recognition) to  identify objects

**Please note:**  `cozmo what is this` only supports English


### About Inception-v3 model
Inception-v3 is trained for the ImageNet Large Visual Recognition Challenge using the data from 2012. This is a standard task in computer vision, where models try to classify entire images into 1000 classes, like "Zebra", "Dalmatian", and "Dishwasher"


### About [Cozmo-Voice-Commands](https://github.com/rizal72/Cozmo-Voice-Commands)
Issue multiple voice commands to [Cozmo](https://anki.com/en-us/cozmo), and watch him execute all of them sequentially: highly customizable, you can add new commands with ease. Recognizes *English, Italian, French, Dutch* but it's very easy to add new languages!


### Three steps installation
Assuming that you've already performed the [**Cozmo SDK Setup**](http://cozmosdk.anki.com/docs/), specific for your platform:  

1.  requires `portaudio`:

  * on **MacOS** (see [Homebrew](http://brew.sh/index_it.html) if you don't know what `brew` is):  
`brew install portaudio`

  * on **Linux**:  
`sudo apt-get install flac portaudio19-dev python-all-dev python3-all-dev && pip3 install --user PyAudio`

  * on **Windows**:  
you only need to [install git](https://git-scm.com/download/win) as it is not included by default.  

2. clone the project :  `git clone https://github.com/wwj718/Cozmo-What-Is-This`

3. install the requirements:

  *  cd Cozmo-What-Is-This
  *  pip install -r requirements.txt (python3.5 virtual env)
  *  python classify_image.py  --model_dir tf/imagenset/

### Usage
`python cvc.py`

  * Optional arguments:  
`--version[-V]`: print version and exit  
`--no-wait[-N]`: enable deprecated continuous listening mode  
`--log[-L]`: enable verbose logging  
* choose speech recognition language and press enter.
* press **SHIFT** when you are ready, then issue your commands by voice (you have 5 seconds to start talking before it Timeouts), not too far from your PC, taking care to include the words "**Cozmo**" or "**Robot**" before any command you'll say: _" COZMO, what is this? "_  



### Todo next
*  add new languages: chinese


