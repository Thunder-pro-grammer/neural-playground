# Neural Network Playground

This is a desktop app that lets you watch a neural network learn in real time. All the network's math is built using NumPy, with no AI libraries like TensorFlow or PyTorch.

What it does
Open the app and you'll see a neural network rendered as connected circles and lines. Click Train and the network learns to solve XOR (a classic logic problem) over 3000 epochs(1 epoch is 1 run through the data). You can watch the weights change color and thickness as the network learns, and see the loss number drop as it gets more accurate. Click Reset to randomize the weights and start over.

Features:
- The Train button runs training and redraws the network, showing updated weights as colored, differently-thick lines, along with the current loss."
- The reset button resets the network so that you can train the data again, and it resets loss to a "-" and changes to a number when you click train.


How I built it
- `network.py` contains the neural network itself and all the math for it: forward pass, backpropagation, and gradient descent
- `ui/canvas.py` renders the network visually, coloring each connection based on whether its weight is positive or negative, and scaling thickness based on how strong that weight is
- `ui/app.py` builds the desktop interface using CustomTkinter

How to run it
Option 1 - Download the exe: Download the “main.exe” from the Releases page: https://github.com/Thunder-pro-grammer/neural-playground/releases/tag/v1.0
          Windows users you may encounter a screen after downloading that says windows protected your PC. To by pass this click more info on the screen then click run anyway.
          For mac users you will need to downlaod the source code zip file on the release pages then open in an IDE and in the IDE terminal you will need to run this command: 
          pip install numpy customtkinter matplotlib, then run the project.

Option 2 -
1. Clone the repo
2. Install dependencies: `pip install numpy customtkinter matplotlib`
3. Run `main.py`

Why I built it:
I built this project because I wanted to understand how neural networks learn. I’ve watched some AI tools perform amazing tasks and become curious about the details of what’s happening within the networks. I also made this project with the intention of practicing my python. I chose to make this a visualizer to help people better understand the changes to the weights within the network.

AI Use:
I did use little bit of AI help for UI.
