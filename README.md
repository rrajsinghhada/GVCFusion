# GVCFusion &nbsp;[![](https://img.shields.io/badge/python-3.8.5-blue.svg)](https://www.python.org/downloads/) [![platform](https://img.shields.io/badge/platform-windows-green.svg)](https://github.com/xenon-19/Gesture_Controller) 

Gesture Voice Controller Fusion System makes human computer interaction simple by making use of Hand Gestures and Voice Commands. The computer requires almost no direct contact. All i/o operations can be virtually controlled by using static and dynamic hand gestures along with a voice assistant. This project makes use of the state-of-art Machine Learning and Computer Vision algorithms to recognize hand gestures and voice commands, which works smoothly without any additional hardware requirements. It leverages models such as CNN implemented by [MediaPipe](https://github.com/google/mediapipe) running on top of pybind11. It consists of two modules: One which works direct on hands by making use of MediaPipe Hand detection, and other which makes use of Gloves of any uniform color. Currently it works on Windows platform.

Note: Use Python version: 3.8.5

# Features
 _click on dropdown to know more_ <br>

### Gesture Recognition:
<details>
<summary>Neutral Gesture</summary>
 <figure>
<!--   <img src="https://github.com/xenon-19/Gesture_Controller/blob/9be82cfc75aa4c04fff0e12dd4de853f9d83a101/demo_media/palm.gif" alt="Palm" width="711" height="400"><br> -->
  <figcaption>Neutral Gesture. Used to halt/stop execution of current gesture.</figcaption>
</figure>
</details>
 

<details>
<summary>Move Cursor</summary>
<!--   <img src="https://github.com/xenon-19/Gesture_Controller/blob/e20edfb1f368ffa600d96bd91031942ec97cb2ab/demo_media/move%20mouse.gif" alt="Move Cursor" width="711" height="400"><br> -->
  <figcaption>Cursor is assigned to the midpoint of index and middle fingertips. This gesture moves the cursor to the desired location. Speed of the cursor movement is proportional to the speed of hand.</figcaption>
</details>

<details>
<summary>Left Click</summary>
<!-- <img src="https://github.com/xenon-19/Gesture_Controller/blob/9be82cfc75aa4c04fff0e12dd4de853f9d83a101/demo_media/left%20click.gif" alt="Left Click" width="711" height="400"><br> -->
 <figcaption>Gesture for single left click</figcaption>
</details>

<details>
<summary>Right Click</summary>
<!-- <img src="https://github.com/xenon-19/Gesture_Controller/blob/9be82cfc75aa4c04fff0e12dd4de853f9d83a101/demo_media/right%20click.gif" alt="Right Click" width="711" height="400"><br> -->
 <figcaption>Gesture for single right click</figcaption>
</details>



<details>
<summary>Drag and Drop</summary>
<!-- <img src="https://github.com/xenon-19/Gesture_Controller/blob/9be82cfc75aa4c04fff0e12dd4de853f9d83a101/demo_media/drag%20and%20drop.gif" alt="Drag and Drop" width="711" height="400"><br> -->
 <figcaption>Gesture for drag and drop functionality. Can be used to move/tranfer files from one directory to other.</figcaption>
</details>




### Voice Assistant ( ***Dee*** ):
<details>
<summary>Launch / Stop  Gesture Recognition</summary>
<!-- <img src="https://github.com/xenon-19/Gesture_Controller/blob/4041eedc2f75fa2923902000b606a05a677629e8/demo_media/voice%20commands/proton%20launch%20stop%20gest.png" alt="launch stop gesture recognition" width="250" height="auto"> -->
<ul>
  <li>
    <code> Dee Launch Gesture Recognition </code><br>
    Turns on webcam for hand gesture recognition.
  </li>
  <li>
    <code> Dee Stop Gesture Recognition </code><br>
    Turns off webcam and stops gesture recognition.
    (Termination of Gesture controller can also be done via pressing <code>Enter</code> key in webcam window)
   </li>
</ul>
</details>

<details>
<summary>Launch Translator Mode</summary>
<!-- <img src="https://github.com/xenon-19/Gesture_Controller/blob/4041eedc2f75fa2923902000b606a05a677629e8/demo_media/voice%20commands/proton%20launch%20stop%20gest.png" alt="launch stop gesture recognition" width="250" height="auto"> -->
<ul>
  <li>
    <code> Dee turn on Translator mode </code><br>
    Turns on Translator mode.
  </li>
  <li>
    <code> Dee exit Translator mode </code><br>
    Exit Translator Mode
    (In Translator mode it asks for the language in which you want Dee to Translate and the whatever she hears she translates to that language.)
   </li>
</ul>
</details>

<details>
<summary>Google Search</summary>
<!-- <img src="https://github.com/xenon-19/Gesture_Controller/blob/4041eedc2f75fa2923902000b606a05a677629e8/demo_media/voice%20commands/proton%20search.png" alt="proton search github" width="800" height="auto"> -->
<ul>
  <li>
    <code>Dee search {text_you_wish_to_search}</code><br>
    Opens a new tab on Chrome Browser if it is running, else opens a new window. Searches the given text on Google.
  </li>
</ul>
</details>

<details>
<summary>Find a Location on Google Maps</summary>
<!--  <img src="https://github.com/xenon-19/Gesture_Controller/blob/4041eedc2f75fa2923902000b606a05a677629e8/demo_media/voice%20commands/proton%20find%20location.png" alt="proton find location" width="800" height="auto"> -->
  <ol>
    <li> 
      <code>Dee Find a Location</code><br>
      Will ask the user for the location to be searched.
    </li>
    <li> 
      <code>{Location_you_wish_to_find}</code><br>
      Will find the required location on Google Maps in a new Chrome tab.
    </li>
  </ol>
</details>


<details>
<summary>Current Date and Time</summary>
<!-- <img src="https://github.com/xenon-19/Gesture_Controller/blob/d49c868acc41ac6c89489bfd80e5e5015a8cb571/demo_media/voice%20commands/proton%20date%20time.png" alt="proton date / time" width="250" height="auto"> -->
  <ul>
    <li>
      <code> Dee what is today's date </code> / <code> Proton date </code><br>
      <code> Dee what is the time </code> / <code> Proton time </code><br>
      Returns the current date and time.
    </li>
  </ul>
</details>

<details>
<summary>Copy and Paste</summary>
<!--  <img src="https://github.com/xenon-19/Gesture_Controller/blob/4041eedc2f75fa2923902000b606a05a677629e8/demo_media/voice%20commands/proton%20copy.png" alt="proton copy" width="500" height="auto"> -->
<!--  <img src="https://github.com/xenon-19/Gesture_Controller/blob/4041eedc2f75fa2923902000b606a05a677629e8/demo_media/voice%20commands/proton%20paste.png" alt="proton paste" width="500" height="auto"> -->
  <ul>
    <li>
      <code> Dee Copy </code><br>
      Copies the selected text to clipboard.<br>
    </li>
    <li>
      <code> Dee Paste </code><br>
      Pastes the copied text.
    </li>
  </ul>
</details>

<details>
<summary>Sleep / Wake up Dee</summary>
<!--   <img src="https://github.com/xenon-19/Gesture_Controller/blob/4041eedc2f75fa2923902000b606a05a677629e8/demo_media/voice%20commands/proton%20bye%20wake%20up.png" alt="proton sleep / wake up" width="250" height="auto"> -->
  <ul>
    <li>
      Sleep<br>
      <code> Dee bye </code><br>
      Pauses voice command execution till the assistant is woken up.
    </li>
    <li>
      Wake up<br>
      <code> Dee wake up </code><br>
      Resumes voice command execution.
    </li>
  </ul>
</details>

<details>
<summary>Exit</summary>
<!--    <img src="https://github.com/xenon-19/Gesture_Controller/blob/4041eedc2f75fa2923902000b606a05a677629e8/demo_media/voice%20commands/proton%20exit.png" alt="proton exit" width="250" height="auto"> -->
  <ul>
    <li>
      <code> Dee Exit </code> <br>
      Terminates the voice assisstant thread. GUI window needs to be closed manually.
    </li>
  </ul>
</details>

# Getting Started

  ### Pre-requisites
  
  Python: (3.6 - 3.8.5)<br>
  Anaconda Distribution: To download click [here](https://www.anaconda.com/products/individual).
  
  ### Procedure
  ```bash
  git clone https://github.com/rrajsinghhada/GVCFusion.git
  ```
  For detailed information about cloning visit [here](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository-from-github/cloning-a-repository).
  
  Step 1: 
  ```bash
  conda create --name gest python=3.8.5
  ```
  
  Step 2:
  ```bash
  conda activate gest
  ```
  
  Step 3:
  ```bash
  pip install -r requirements.txt
  ```
  
  Step 4:
  ```bash 
  conda install PyAudio
  ```
  ```bash 
  conda install pywin32
  ```
  
  Step 5:
  ``` 
  cd to the GitHub Repo till src folder
  ```
  Command may look like: `cd C:\Users\.....\Gesture-Controlled-Virtual-Mouse\src`
  
  Step 6:
  
  For running Voice Assistant:
  ```bash 
  python Dee.py
  ```
  ( You can enable Gesture Recognition by using the command "Proton Launch Gesture Recognition" )
  
  Or to run only Gesture Recognition without the voice assisstant:
  
  Uncomment last 2 lines of Code in the file `Gesture_Controller.py`
  ```bash 
  python Gesture_Controller.py
  ```
  

  
