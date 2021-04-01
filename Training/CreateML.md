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
