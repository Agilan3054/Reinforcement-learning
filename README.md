# Reinforcement Learning 

## CIA-1: Upper Confidence Bound (UCB) Algorithm

The `StockOptimizer` class simulates a stock selection optimization process using the Upper Confidence Bound (UCB) algorithm. It aims to maximize viewer engagement by balancing exploration and exploitation, selecting the stock with the highest Q-value over time.

### Key Features
- **Reward Calculation**: Simulates viewers and compares to generate reward for each stock.
- **UCB-Based Action Selection**: Chooses actions by calculating UCB values, promoting balance between exploration and exploitation.
- **Q-Value Updates**: Iteratively refines Q-values with rewards to optimize stock selection.

### Visualization
- **Time Series Plot**: Shows Q-value evolution for each stock over time.
- **Final Q-Value Bar Chart**: Highlights final Q-value estimates for all stocks.
- **Heatmap**: Displays Q-value progression across time steps for each stock.

### Code Highlights
- `get_reward`: Computes rewards based on viewer simulation.
- `choose_stock`: Selects stock actions using UCB.
- `optimize`: Trains the optimizer over specified time steps.
- `_show_visualizations`: Generates various plots for analysis.

# CIA-2: Grid Environment Navigation with Q-Learning

The `QLearningAgent` class learns optimal navigation strategies in a grid environment with a start point, a goal, and obstacles. It uses Q-learning to update a Q-table, balancing exploration and exploitation to find the optimal path.

## Key Features

- **Epsilon-Greedy Action Selection**: Balances exploration (random actions) with exploitation (optimal actions) based on the epsilon-greedy policy.
- **Q-Value Updates**: Temporal difference learning is used to update Q-values, which improves the agent's navigation strategy.
- **Training**: The agent runs through multiple episodes to iteratively refine its Q-values and learn the best path.

## Visualization

- **Q-Value Heatmap**: After training, the Q-values across the grid are visualized as a heatmap, highlighting the optimal path and decision-making.
- **Environment Rendering**: The grid with the start, goal, and obstacles is rendered. The agent's movement and final path are also visualized.

## Code Highlights

- **`choose_action(state)`**: Selects actions based on the epsilon-greedy policy.
- **`update(state, action, reward, next_state)`**: Updates Q-values for state-action pairs using temporal difference learning.
- **`train(episodes=1000)`**: Runs multiple episodes to train the agent, refining Q-values in each step.
- **`render()`**: Visualizes the agent's journey through the grid environment, showing the path taken to reach the goal.
