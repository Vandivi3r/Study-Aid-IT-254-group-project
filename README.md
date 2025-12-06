## StudyAssistantProject
This project uses AI models and an arduino to help the user study. The python code will turn on your camera, set a timer, and either give messagages depending on how focused you are on what you are studing. 

## Our Demos
For the first demo it buzzed whenever the person is looking away from the camera.

For the second demo we updated the model to enable it to be more accurate. Added a timer, the model and the buzzer were fully syncronized at this point and it would be able to tell if the person was distracted or not. started working on the "study guide" feature.

For our final demo there is  a study guide at end once the timer is up that will test you based on what you were studying.

* link for the main project: https://github.com/Im2Slothy/StudyAssistantProject

Required Items for this Project
- commputer running python 3.11+ (The code was ran on 3.11.8)
- A camera 
- OpenAI API key
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

3. Install required python packages(make sure you are running python 3.11.8 or you will have a bad time)
" pip install -r requirements.txt "

4. Connect the hardware, upload the main.ino to your Arudino
5. Change the COM port value in the python file to what ever port your Arudino is connected to (check arduino ide)

## Using the Program
1. Run the python file

2. Drag and drop a PDF of what you want to study (optional) 
   
3. Choose study method
- For custom method input: study time, break time and number of cycles (has to be more than 0)

4. The model will detect if you are looking at it or if you are distracted it will buzz and speak

5. At the end it will give you a study guide that will help you review your subject of choice
