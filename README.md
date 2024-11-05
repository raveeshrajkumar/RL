# Reinforcement Learning CIA Assignments

This repository contains two assignments as part of the Continuous Internal Assessment (CIA) for Reinforcement Learning. These assignments demonstrate implementations of RL techniques applied to specified problems, using concepts like Markov Decision Processes (MDP) and K-arm bandit solutions.

## Files in the Repository

- **CIA1.ipynb**: This notebook addresses a news value maximization problem using a K-arm bandit solution. The task is to maximize views for politically and commercially affiliated articles by treating each article as an "arm" of the bandit. 
  - **Problem Statement**: Politically and commercially affiliated media companies need to maximize views on selected articles. The solution builds a system that prioritizes these “aligned” articles to drive engagement.
  - **Solution Approach**: 
    - Each article a user might click on represents an arm in the K-arm bandit setup.
    - Articles are denoted as \( a_1, a_2, \ldots, a_k \), with each \( a_i \) being "aligned" to specific viewer interests.
    - Rewards are measured by click counts, focusing solely on view generation rather than full reads.
    - The system balances exploration and exploitation, occasionally displaying random articles to test new possibilities while mainly focusing on articles known to attract clicks.
    - This approach identifies the most engaging articles, guiding future content to follow characteristics of high-view articles, thus maximizing views.

- **CIA2.ipynb**: This notebook focuses on creating a 100x100 grid environment for an RL agent using MDP (Markov Decision Process). The agent must navigate from a start point to a goal point while avoiding obstacles placed within the grid. The main objectives are:
  - To define and optimize policies and actions at every state for the agent
  - To benchmark Dynamic Programming (DP) methods with other RL solutions on the same grid-based navigation problem

## Assignment Objectives

### CIA-1: News Value Maximizer using K-arm Bandit
- **Objective**: Develop a K-arm bandit solution to maximize views on selected articles, with a focus on politically and commercially affiliated media.
- **Implementation**: The notebook implements a K-arm bandit approach with an emphasis on exploration-exploitation balance, where each article click represents a reward.
- **Key Components**: Arm selection based on reward maximization to enhance visibility for high-view articles.

### CIA-2: Grid Navigation using MDP
- **Objective**: Set up a grid environment with obstacles, allowing the RL agent to optimize navigation from a start to a goal position.
- **Implementation**: This notebook defines the grid environment as a Markov Decision Process (MDP) and benchmarks the Dynamic Programming method against other RL techniques, such as value iteration or Q-learning, for policy optimization.

## Requirements
- Python 3.x
- Jupyter Notebook
- Libraries: numpy, matplotlib, and any other relevant RL libraries such as gym or stable-baselines (if used)

## How to Run
1. Clone the repository.
2. Install the required libraries.
3. Open each `.ipynb` file in Jupyter Notebook or JupyterLab.
4. Run the cells sequentially to observe the implementations and outcomes.

## Results
The notebooks include:
- **CIA1**: Insights into which articles attract the most views, providing guidance for maximizing viewership.
- **CIA2**: Comparative analysis of DP and other RL solutions for navigating the 100x100 grid environment.
