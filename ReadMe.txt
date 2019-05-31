#Takashi Nalkano et.al. 2015

#Nakano T, Otsuka M, Yoshimoto J, Doya K (2015) A Spiking Neural
 Network Model of Model-Free Reinforcement Learning with
 High-Dimensional Sensory Input and Perceptual Ambiguity. PLoS ONE
 10(3): e0115620. doi:10.1371/journal.pone.0115620

#nest-1.9.7905 was used for the simulation. 

This is spiking neural network models of free-energy-based
reinforcement learning.  We test our SNN model on three tasks with
increasing levels of difficulty:

1. center reaching task (a reinforcement learning (RL) problem),
2. digit center reaching task (a history-independent partially
observable RL (PO RL) problem),
3. digit-matching T-maze task (a history-dependent PORL problem).


1. center reaching task (a reinforcement learning (RL) problem), 
Model file
	-SpikingRBM_CR.py
The following files are generated after the simulation.
	-History.txt #history of states, actions, free-energy and
         firing of action neurons in decision making period that the
         agent experienced.
	-HistoryNstep.txt #steps to the goal
	-HistoryCumR.txt #cumulative reward
	-Wha.txt # learned weight between action and hidden neurons
	-Whs.txt # learned weight between state and hidden neurons

2. digit center reaching task (a history-independent partially
observable RL (PORL) problem),
Model file
	-SpikingRBM_Digit.py
The following files are required for the simulation.
	-files in digit22 folder
The following files are generated after the simulation.
	-History.txt #history of states, actions, free-energy and
         firing of action neurons in decision making period that the
         agent experienced.
	-HistoryNstep.txt #steps to the goal
	-HistoryCumR.txt #cumulative reward
	-Wha.txt # learned weight between action and hidden neurons
	-Whs.txt # learned weight between state and hidden neurons

3. digit-matching T-maze task (a history-dependent PORL problem).
Model file
	-SpikingRBM_MTmaze.py
The following files are required for the simulation.
	-files in shrunk_digit_easy_test_20_15T folder
	-Wcd50_noBias.txt #weights from observation to memory neurons
	-MMweight2301.txt #reccurent connection weights of memory neurons
The following files are generated after the simulation.
	-History.txt #history of states, actions, free-energy and
         firing of action neurons in decision making period that the
         agent experienced.
	-HistoryNstep.txt #steps to the goal
	-HistoryCumR.txt #cumulative reward
	-Wha.txt # learned weight between action and hidden neurons
	-Whs.txt # learned weight between state and hidden neurons
	-Whm.txt # learned weight between memory and hidden neurons
