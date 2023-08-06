# Pong Game with AI using NEAT (NeuroEvolution of Augmenting Topologies)
*Bawanga Senevirathne - 06th Aug. 2023*

NEAT is a genetic algorithm which takes inspiration from human history and natural selection. 
NEAT can be identifies as a building layer on top of a neural network.

When using NEAT, it creates a set of neural networks with pre-defined features such as input-nodes, output-nodes and hidden-nodes. And some random mutations are being performed to these neural networks. NEAT algorithm only modifies the hidden layer(s) nodes, the amount input and output nodes are kept unchanged.

If we decide to start with 10 neural networks with NEAT,

![image](https://github.com/bsen-alt/Python-pong-AI/assets/89639082/72b03e04-8260-4739-a659-433af9200e3a)

NEAT identifies the above neural networks as Genomes, and allocates a value to each of them, the value is called Fitness. Fitness of a Genome is a score for how it performs the task (as for natural selection – how long a species survive).

**The Fitness score of Genomes of this project = Number of times the AI hits the ball moving the paddle**

![image](https://github.com/bsen-alt/Python-pong-AI/assets/89639082/b6d8020e-6c43-45d6-87a7-83af1eb619ab)


Using these fitness values, we can eliminate some under-performing Genes, and we can breed the best genomes together and to move to the next generation. Then proceed to next generation.
This generation iteration process continues until a neural network satisfies our criteria – in this case a Fitness Level of 100.

NOTE: NEAT does more advanced operations behind the curtains, such as grouping genomes – that 
will protect species without leading them to extinction, how long an under-performed genome is 
kept alive in the algorithm, adding random mutations to the off-spring genomes from later 
generations etc.


Training for Paddle y direction

![Alt Text](/gifs/pong-paddle.gif)

Training with generational iterations

![Alt Text](/gifs/pong-gen-train.gif)

AI playing with me - Me on Left, AI on Right

![Alt Text](/gifs/pong-ai-vs-me.gif)


