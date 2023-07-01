# Flappy Bird AI using NEAT
This project implements an AI that can play the game Flappy Bird using the NEAT (NeuroEvolution of Augmenting Topologies) algorithm. The AI learns to play the game by evolving a neural network that controls the bird's actions.

Gameplay
The goal of the game is to navigate the bird through a series of pipes without colliding with them. The bird automatically moves forward, and the player can make it jump by pressing the spacebar. The game ends if the bird collides with a pipe or touches the ground.

NEAT Algorithm
The NEAT (NeuroEvolution of Augmenting Topologies) algorithm is used to train the neural network that controls the bird. NEAT evolves a population of neural networks by combining the best-performing networks and mutating their structure. Over time, the population improves, and the AI learns to play the game more effectively.

The neural network takes three inputs: the bird's current y-position, the vertical distance to the top pipe, and the vertical distance to the bottom pipe. The output of the network determines whether the bird should jump or not.

The fitness of each bird is based on how long it stays alive. Additional rewards are given for passing through pipes.

Configuration
The NEAT algorithm is configured using a configuration file. The config file specifies the parameters for the NEAT algorithm, such as population size, mutation rates, and fitness function.

Results
The AI will run for 50 generations, and the best performing genome will be displayed at the end. You can modify the number of generations or add early stopping conditions as needed.

During the training process, you can enable the visualization of the best bird's performance by uncommenting the relevant code in the eval_genomes function.

Note: The code contains a commented section that saves the best performing network as a pickle file. You can uncomment this code if you want to save the best network for later use.

Enjoy watching the AI learn to play Flappy Bird!


