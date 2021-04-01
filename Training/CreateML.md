# Training the model using Create ML

[Control training in Create ML with Swift](https://developer.apple.com/videos/play/wwdc2020/10156)

[CreateML App](https://developer.apple.com/videos/play/wwdc2019/430)

FitnessClassifierModel

Prediction

Predictor + Pose

Data collection:

- 50+ examples per class

- Diverse subjects

- Include a folder of other poses such as resting

Capturing the action

- Keep camera stable

- Good contrast between subject and background

- Avoid loose, flowing clothing

Choosing training parameters

- Prediction window should include an entire action

- Consistent frame rate between training and test videos

Using the model in your app

- Selecting a single person out of multiple people

- Counting action repetitions, find a reliable trigger and start prediction in the correct time. 

- Scoring or judging quality of an action (confidence value)

---

Training dataset

- 8 "Pose A" 2s video clips

- 8 "Not Pose A" 2s video clips 

Data augmentation

- Horizontal flip

Recurrent neural network model training

- 80 iterations 

Prediction window on live camera feed

- 60 frame

Prediction results

- Prediction class("Pose A" or "Not Pose A")

- Confidence interval 

---

hmdb51 dataset

The dataset contains 6849 clips divided into 51 action categories, each containing a minimum of 101 clips. Each clip are 2 seconds. The actions categories can be grouped in five types:

1.  General facial actions smile, laugh, chew, talk. 
2.  Facial actions with object manipulation: smoke, eat, drink.
3.  General body movements: cartwheel, clap hands, climb, climb stairs, dive, fall on the floor, backhand flip, handstand, jump, pull up, run, sit down, sit up, somersault, stand up, turn, walk, wave.
4.  Body movements with object interaction: brush hair, catch, draw sword, dribble, golf, hit something, kick ball, pick, pour, push something, ride bike, ride horse, shoot ball, shoot bow, shoot gun, swing baseball bat, sword exercise, throw.
5.  Body movements for human interaction: fencing, hug, kick someone, kiss, punch, shake hands, sword fight.
