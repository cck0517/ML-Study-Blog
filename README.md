# ML-Study-Blog
This is a blog keeping track of my daily ML study for ML researches.

## Day 9/16
**Study source:** [Spinning Up RL Introduction](https://spinningup.openai.com/en/latest/spinningup/rl_intro.html)

**Topics covered:**
- Reviewed basic RL knowledge
- Reviewed Q values, Value functions, Advantages
- Action spaces (real valued)
- Sampling from categorical policies and diagonal Gaussian policies

## Day 9/17
**Study source:** [Spinning Up RL Introduction Part 2](https://spinningup.openai.com/en/latest/spinningup/rl_intro2.html)

**Notes:**
- **Model-Free vs Model-Based RL:** Whether the agent has access to (or learns) a model of the environment (for predicting state transitions and rewards)
- **Pros of having a model:** (like AlphaZero) can help agent plan ahead, sample efficiency improvement
- **Cons of having a model:** Getting the ground truth model is fundamentally hard, and simulating it is hard. Sometimes the bias of the model are being exploited by the agent, so it does well in the simulated env but poorly in real world
- Also studied types of different model/model-free algorithms/works

## Day 9/22 - 9/23

**Notes:**

**Policy Gradient Update:** Using gradient descent to maximize the mean reward over time. This is done by carefully constructing a "Loss function", which, when we take the gradient, the gradient of the "loss function" will have the same analytical formula as the policy gradient. Because this gradient of the loss function takes place as an expectation, so one practical way of approximating it is to sample enough rollouts (we want fixed number of steps instead of number of trajectories, because we want stable batches, as the mean for estimating the expectation is taken over number of steps, not trajectories)

**Plans for the RL field:**

**Basics:** Intro to RL (finished), standard Machine learning concepts (regularization, attention mechanisms)

**Implementations:** Vanilla policy update algorithms first, then maybe ppo, and maybe GRPO, and others (focus on understandings)

**Read the key papers, identify researches to do, and boundaries to push:** https://spinningup.openai.com/en/latest/spinningup/spinningup.html

## Day 9/24
**Notes:**
- Did diagonal Gaussian distribution sampling implementation exercise
- Started working on vanilla policy gradient update implementation — see [Vanilla Policy Gradient](https://spinningup.openai.com/en/latest/algorithms/vpg.html)


## Day 9/25
**Notes:**
- Completed studying implementation of Vanilla Policy Gradient (VPG) algorithm
- Read PPO Algo and implementation details: https://spinningup.openai.com/en/latest/algorithms/ppo.html

