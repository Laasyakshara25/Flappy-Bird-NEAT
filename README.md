# Flappy Bird AI Using NEAT Algorithm

This project showcases an AI agent learning to play the classic Flappy Bird game using the NEAT (NeuroEvolution of Augmenting Topologies) algorithm. By simulating evolution, the AI refines its skills over generations, transforming from a random neural network to selecting a best performing bird that masterfully plays the game.



## What is NEAT?

NEAT is a genetic algorithm that evolves neural networks by improving both their structure and weights over time. Unlike fixed architectures, NEAT starts with simple networks and makes them more complex only when needed, ensuring efficiency and encouraging innovation.

### Inputs and Outputs:
- **Inputs to the AI:**
  - Bird's vertical position.
  - Distance to the next pipe (horizontal and vertical).
  
- **Output from the AI:**
  - One action:  **Jump** or **Don't Jump**.

### Fitness Function:
The fitness function rewards the AI for:
- Surviving longer in the game.
- Successfully passing through pipes. 
This encourages the AI to improve its gameplay strategy over time.


##  Neural Network Details

- **Activation Function:** Tanh
  - This function ensures smooth gradients and handles negative values well, aiding the learning process.
- **Population Size:**
  - Starts with a certain number of birds and eliminates the poor performing ones over generations.
 - **Max Generation:**
    - Maximum number of generations of genomes the AI is trained on.



## Evolution Process

1. Start with a population of simple neural networks.
2. Test each network in the Flappy Bird environment.
3. Use the fitness function to rank networks based on their performance.
4. Combine the best-performing networks and introduce random changes to maintain diversity.
5. Over successive generations, watch the AI improve and master the game.


## Output Preview

![Flappy Bird AI Learning](https://github.com/Laasyakshara25/Flappy-Bird-NEAT/blob/main/output/flappy-bird.gif)
![Terminal Output](




 **Clone the Repository:**
   ```bash
   git clone https://github.com/Laasyakshara25/Flappy-Bird-NEAT.git
   cd flappy-bird.py
```
**Install Dependencies:**
```bash
pip install pygame neat-python
```
**Run the game**
```bash
python flappy_bird.py

