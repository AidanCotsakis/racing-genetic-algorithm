# Racing Game with Genetic Algorithm

This project is a racing game that uses a genetic algorithm to optimize car paths around a track. Cars evolve across generations, learning progressively efficient paths with each iteration. Built with Pygame, this project combines pathfinding, dynamic scoring, and visually enhanced gameplay to illustrate the principles of genetic algorithms in a gaming environment.

## **Features**

- **Genetic Algorithm Optimization**: Cars improve route efficiency over time, adapting their movement "brains" through generations.
- **Dynamic Checkpoint System**: A checkpoint scoring system that encourages cars to follow the race course.
- **Pygame-Based Visualization**: Rendered visuals include custom track tiles, trees, and car sprites for immersive gameplay.
- **High Customizability**: Flexible settings for track layout, car attributes, mutation rates, and visual aspects.

## **Setup Instructions**

1. **Install Dependencies**: Ensure Python and Pygame are installed.
   ```bash
   pip install pygame numpy pillow
   ```
2. **Run the Program**: Launch the main file to start the game.
    ```bash
    python racingGeneticAlgorithm.py
    ```

## **Usage**
The program starts automatically with AI-driven cars.
- **Settings**: Modify parameters in `racingGeneticAlgorithm.py` such as `numberOfCars`, `mutations`, and `fps` to fine-tune gameplay and algorithm performance.
- **Track**: Modify `track` and `checkpoints` to create a custom track that the cars learn to drive.

## **Project Structure**
- **`car` Class**: Defines car properties and actions, including movement, checkpoint tracking, and score calculation.
- **Rendering Functions**: Methods like `drawGround`, `drawWalls`, and `renderBackground` handle track and background rendering.
- **Genetic Algorithm Functions**: `newGeneration` and `mutate` manage the evolution of car "brains" through selective breeding and mutation.

## **How It Works**
- **Initial Setup**: Cars are generated with random movement patterns.
- **Simulation Loop**: Each car navigates the track, collecting checkpoints and avoiding collisions.
- **Evolution**: After each generation, top-performing cars are selected, cloned, and mutated to form the next generation.
- **Visual Feedback**: Track and car visuals update in real time, showing progress.