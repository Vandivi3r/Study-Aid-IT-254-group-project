## StudyAssistantProject
This project is using AI models and an arduino in order to help the user focus on studying. The python code will turn on your camera, allow you to set up a timer, and either give motivation messagages or sassy remarks depending on how focus you are on what you are studing. 

## Our Demos
For the first demo we did wanted to test our code to see if it will buzz whenever the person is looking away from the camera or looking at the camera.

For the second demo we were able to update the model to enable it to be more in tune with want we want for the final project, There was a timer, the model and the buzzer were fully syncronized at this point and it would be able to tell if the person was distracted or not. We also started working on the "study guide" part of the project.

For our final demo, we were able to add text to speech and snarky comments the text to speech would say. There is also a study guide at end once the timer is up that will test you based on what you were studying.

* link for the main project: https://github.com/Im2Slothy/StudyAssistantProject

##Required Items for this Project
- A laptop with python 3.11+ (The code was ran on 3.11.8)
- A camera
- All the python libraries that are listed in requirements.txt
- OpenAI API key which is needed for the remarks and the study guide at the end

**Arduino requirements**
- Arduino IDE for the .ino file
- Buzzer
- Wires
- LED light
- Resistor

* Do not forget to run the Arguino file before the python file

## Setup 
1. Download the files in this respository

2. Create a file name .env in the main project folder and add your OpenAI API key to it
" OPENAI_API_KEY=api_key_goes_here "

3. Install required python packages
" pip install -r requirements.txt "

4. Connect the hardware, upload the main.ino to your Arudino, may need to change the COM port to what ever port your Arudino is connected to on the main.py file

## Using the Program
1. Run the python file

2. Upload a PDF of what you want to study (which is optional) by dragging and dropping
   
3. Choose study method then it will start
- Put in your study time, break time, and how many cycles you want (has to be more than 0) if you choose the custom study method

4. Now the model will detect if you are looking at it or if you are distracted and will buzz and speak if you are

5. At the end it will give you a study guide that will help you review your subject of choice
