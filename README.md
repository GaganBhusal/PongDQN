# Pong-DQN

Implementation of the Deep Q-Learning Network(DQN) to play the atari Pong from OpenAI Gymnasium environment.

# Demo
![Pong Demo](video/pong.gif)

# Problem Statement


The Atari Pong environment consists of two paddles and a ball.The agent controls the green paddle on the right and the brown paddle is controlled by the built in Computer AI. The objective is to score points by getting the bass past the opponent's paddle. Each succesful score yields 1 point to scoring player. A match ends when either of them reaches 21 points, and the first one to do so is the winner.

The environment provides raw RGB images of size 210 x 160 pixels. This is what we see or a human player see. For training they are processed by :
* Grayscale Conversion to reduce computional complexity.
* Cropping 34 pixels from top and 16 pixels from bottom to focus on the gamefield and to remove unnecessary areas like score display (results in 160 x 160 pixels)
* Resizing to 84 x 84 pixels for efficieny.
* Frame Stack: 4 continuous frames are stacked together to capture temporal dynamics and to find out ball velocity and direction.



# Description


