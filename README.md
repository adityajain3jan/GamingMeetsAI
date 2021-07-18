# SoC- Gaming Meets AI

## Project Description:
The goal was to create a reinforcement learning based agent that could play the game 2048. 
The agent has been implemented using PyTorch. Some other python libraries such as pickle and matplotlib have been used in order to store the agent's state, and to visualze the learning learning process. 
Deep Q-learning has been used to train the agent.

## Description of Files:
- GamingMeetsAI: This folder contains the complete final code of the project in four seperate files:-
  * [ModelAndAgent.ipynb](https://github.com/adityajain3jan/GamingMeetsAI/blob/main/GamingMeetsAI/ModelAndAgent.ipynb): This file contains three classes: ReplayBuffer, Model and Agent. ReplayBuffer is a python list of a default capacity of 100,000 items. Model contains a sequential network of three hidden layers having 512, 256 and 128 neurons respectively. Finally, the Agent class is a template for our learning agent, and contains functions for training the model instance, running the episodes, updating target network, selecting actions.
  * [TrainAndTest.ipynb](https://github.com/adityajain3jan/GamingMeetsAI/blob/main/GamingMeetsAI/TrainAndTest.ipynb): This is the main file where we will train and test the agent. the train_agent method can be called by supplying the number of training episodes as argument. The state of the agent will be automatically loaded from and saved into a file with extension '.pkl'. Similarly, the trained model can be tested by using the test_agent method and supplying the number of testing episodes.
  * [myagent.pkl](https://github.com/adityajain3jan/GamingMeetsAI/blob/main/GamingMeetsAI/myagent.pkl): This file stores the state of the agent after each training. When testing and training is done, the agent is automatically loaded from this file.
  * [mygame.py](https://github.com/adityajain3jan/GamingMeetsAI/blob/main/GamingMeetsAI/mygame.py): This file contains the code for the 2048 Game environment which has been used for the agent.
 
 - [Soc_Project_Report.md](https://github.com/adityajain3jan/GamingMeetsAI/blob/main/SoC_Project_Report.md): This file contains the complete progress report, including the links for the various resources that I used.
 - [ProjectReport.pdf](https://github.com/adityajain3jan/GamingMeetsAI/blob/main/Progress%20Report.pdf): Contains the progress report, in pdf format.
 
 ## Running the Code:
 ### Requirements:
 Make sure that you have gym, numpy, matplotlib, wandb, torch and pickle packages installed. If not, then they can be installed using the following command:
 pip install (package name)
 
 Once this is done, download the folder GamingMeetsAI and open the same through jupyter notebook. Now, simply uncomment the test_agent and train_agent functions as desired. 
 The arguments to the test_agent and train_agent functions can be varied as needed.
