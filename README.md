# AI-Learns-to-Play-Flappy-Bird
An implementation of Flappy Bird that uses the NEAT (NeuroEvolution of Augmenting Topologies) algorithm to train an AI to play the game. Built with Python and Pygame.

## Description

This project implements a Flappy Bird game where artificial neural networks learn to navigate the bird through pipes. The NEAT algorithm is used to evolve increasingly better gaming strategies through natural selection.

### Features

- Classic Flappy Bird gameplay mechanics
- NEAT algorithm implementation for AI learning
- Visual display of current generation and score
- Population-based training with multiple birds simultaneously
- Real-time visualization of AI learning process

## Requirements

- Python 3.x
- pygame
- neat-python

## Installation

1. Clone the repository
2. Install the required packages:
```bash
pip install pygame neat-python
```

## Usage

Run the game using:
```bash
python flappy_bird.py
```

## How it Works

- The AI uses neural networks to control the birds
- Each bird receives three inputs:
  - Bird's Y position
  - Distance to top pipe
  - Distance to bottom pipe
- The network outputs whether to jump or not
- Each generation consists of 15 birds
- Birds are rewarded for passing through pipes and staying alive
- The fittest birds are selected to produce the next generation

## Configuration

The NEAT algorithm parameters can be modified in `config-feedforward.txt`, including:
- Population size
- Network architecture
- Mutation rates
- Species settings

## Credits

Images and base game mechanics inspired by the original Flappy Bird game.
NEAT implementation based on the neat-python library.
