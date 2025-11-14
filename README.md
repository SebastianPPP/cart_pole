# Q-Learning for CartPole-v1: Reinforcement Learning

This project implements the classic **Q-learning algorithm** (Reinforcement Learning) to solve the **CartPole-v1** problem from the **Gymnasium** environment. The agent's goal is to learn to control the cart to keep the pole in a perfectly vertical balance for the longest possible time.

---

## Key Concepts Revisited

* **Q-learning:** A value-based algorithm that uses a **Q-table** to store optimal actions for observed states.
* **State Discretization (Quantization):** The process of converting the continuous state space (position, angle, velocities) into a finite and manageable number of discrete "bins."
* **Bellman Equation:** The core principle behind the Q-table update, used to iteratively estimate the maximum cumulative future reward.
* **$\epsilon$-greedy:** The strategy for balancing **exploration** (random actions) and **exploitation** (utilizing the best-known action).

---

## Training Structure

* **Hyperparameters:** Key parameters were defined, such as the **learning rate** (`LEARNING_RATE`), **discount factor** (`DISCOUNT_FACTOR`), and the **exploration decay rate** (`EPSILON_DECAY_RATE`).
* **Discretization:** The state space was divided into $20 \times 20 \times 20 \times 20$ discrete bins.
* **Training Loop:** The agent runs for **20,000 episodes**, making decisions and updating the Q-table according to the Bellman equation in each step.

---

## Results 

The training demonstrated a slow but stable learning process.