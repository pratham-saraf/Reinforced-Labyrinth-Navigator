# Reinforcement Learning Maze Solver

This project implements a maze-solving algorithm using reinforcement learning techniques in Python. The algorithm utilizes value iteration and SARSA algorithms to enable an autonomous agent to navigate through a maze environment, learning optimal paths to reach the goal while avoiding obstacles.

## Features

- **Maze Solving Algorithms:** Implemented value iteration and SARSA algorithms to solve maze environments efficiently.
- **Interactive Visualization:** Utilized Pygame to create an interactive visualization, enabling users to observe the maze-solving process in real-time.
- **Dynamic Pathfinding:** The agent autonomously learns and updates action policies, adapting its navigation strategy based on the maze layout and goal position.

## Usage

1. **Installation:**
   - Clone this repository.
   - Install the required dependencies:
     ```bash
     pip install -r requirements.txt
     ```

2. **Run the Maze Solver:**
   - Execute `main.py` to visualize the maze-solving algorithm in action.
   - Adjust maze layouts, dimensions, or algorithms within the code as needed.

## Maze Layout

The maze layout is represented in the `level` variable within `main.py`. Modify this variable to change the maze's structure and complexity.

## How It Works

The maze-solving algorithm operates as follows:

1. **Initialization:**
   - The maze environment is created using the `Maze` class, which takes the maze layout, goal position, and other parameters.
   - Walls and open spaces in the maze are identified and stored for reference during navigation.

2. **Reinforcement Learning Algorithms:**
   - **Value Iteration:** The algorithm iterates through the maze, updating state values based on the immediate rewards and potential future rewards.
   - **SARSA (State-Action-Reward-State-Action):** Used to update action values based on the current state-action pair and the subsequent state-action pair.

3. **Policy Update:**
   - Action policies are dynamically updated based on the learned values, guiding the agent's movement within the maze.
   - The agent chooses actions according to these policies, moving towards the goal while avoiding walls and obstacles.

4. **Visualization:**
   - Pygame is utilized to create an interactive visualization of the maze-solving process.
   - The agent's movement and decision-making process are displayed in real-time, providing a visual representation of the algorithm's navigation through the maze.

5. **Continuous Learning:**
   - The algorithm continues to learn and update its strategies, refining its pathfinding abilities as it explores different maze layouts.

6. **User Interaction:**
   - Users can observe the agent's progress, visualize its decision-making, and witness how the algorithm adapts to different maze configurations in real-time.

This reinforcement learning-based maze solver intelligently navigates through maze environments, continuously learning and updating its strategies to find optimal paths towards the goal.


## Contributing

Contributions are welcome! Feel free to open issues or pull requests for enhancements, bug fixes, or additional features.

## License

This project is licensed under the [MIT License](LICENSE).



