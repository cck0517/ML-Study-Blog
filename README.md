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