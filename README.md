# Multi-armed-bandits


## 1. Cricket Strategy Optimization (MDP)
This code implements a dynamic programming solution to optimize batting decisions in cricket through Markov Decision Processes (MDPs). The model helps determine optimal shot selection strategies that balance risk and reward under varying game conditions.

### Key Features

### Dynamic game state modeling considering:
- **Wickets remaining**
- **Balls left in innings**
- **Run-scoring probabilities**
- **Wicket-loss probabilities**

### Risk-reward optimization through:
- **State-value function estimation**
- **Action-value (Q-value) calculations**
- **Bellman equation-based updates**

## 2. UCB Algorithm
- Implements the **Upper Confidence Bound** method for multi-armed bandits.
- Maintains **confidence intervals** around estimated rewards for each arm (action).
- Balances **exploration/exploitation** by prioritizing arms with higher upper bounds on reward.
- Refines reward estimates over time and converges on the **optimal arm** for long-term gains.

## 3. ETC Algorithm
- Implements the **Explore-Then-Commit** strategy for multi-armed bandits.
- First explores during a specified phase to sample each arm and gather **reward statistics**.
- After exploration, commits to the arm with the **highest observed average reward**, reducing uncertainty while trading off early experimentation.

