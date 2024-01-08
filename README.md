# MTB simulator
 MTB play-thorugh simulator, where a posture recognition model is used to assign points

https://teachablemachine.withgoogle.com/train
How the pre-trained neural net works..... 

It is based on a large classification network, in our case posture recognition. This model is trained on a lot of data and tries to fit "junction" points to the human body.  We train a network that takes those junction points and tries to predict the class it belongs to! The advantage is that we don't look on a pixel level to the data (training set and test set).  We just look at the junction points, which in turn means that the model should be very robust in terms of predicting different people in different rooms. It does look at relative position within the viewport (webcam)! So a neutral central position of the user is necessary, we can also train on relative shoulder angle, head angle etc.  

SO this is a nice update