# warehouse-rl-project

## Project Overview

This all started with a classic challenge in industry: figuring out how to make warehouse work less tedious for people. In this project, I took on the role of an AI engineer at Okanogan, a fictional company with real-enough warehouse headaches. The plan was to use autonomous robotic carts to move products between shelves and shipping areas, without having robots crash into anything. The hope, I suppose, was to make the place run more smoothly and keep accidents to a minimum.

### Key Technologies
- Python 3.7+
- OpenAI Gym for simulating the robot’s environment
- NumPy to manage state-action tables and handle randomness
- Matplotlib for making sense of performance trends
- PyTorch, since deep learning is pretty much expected now
- Jupyter and Colab, which can sometimes save you from dealing with install nightmares

## What Actually Happened (Milestone by Milestone)

### Milestone 1: Framing the Problem

If you’ve ever looked at OpenAI’s Taxi-v3 scenario, you know the type of setup: a grid world, a tiny yellow taxi, and a set of clear rules about picking up and dropping off passengers. Mapping this to warehouse robots makes surprising sense. Each task starts somewhere, has a goal location, and is littered with places where things can go wrong. Calling this “intelligent” might be stretching it; in practice, it feels a lot like trial and error that happens to have nicer terminology.

### Milestone 2: Tabular Q-Learning—The Basics

I implemented Q-learning with a classic grid. Every move the bot makes updates a massive table of possibilities and learned consequences. Repeated training helped the bot avoid bad moves and, eventually, started to look almost competent in simple environments. Of course, as soon as things get more complex, you realize how limited Q-tables are. For basic scenarios though, Q-learning gets the job done.

### Milestone 3: First Foray into Deep RL

This step was more challenging. I swapped out the Q-table for a neural network using deep Q-learning, and switched the test to Gym’s CarRacing-v0. The idea was for the robot to process screen pixels and learn to navigate more like it would in a real setting. Results were mixed. Training sometimes felt unstable, and networks sometimes forgot good behaviors. Improving performance took a fair amount of patience, but gradual progress was visible every now and then.

### Milestone 4: Making Deep RL Work Reliably

Next came a batch of stability tricks: implementing experience replay buffers to cut down on correlation in samples, and target networks to keep learning objectives from shifting too quickly. These additions made a real difference. The agent eventually learned to avoid obstacles and get to the goal with much more regular success, though “regular” might be an optimistic word for it. Progress didn’t necessaraly  move in one direction, but overall navigation did improve.

### Milestone 5: Custom Grid-World Warehouse

The last milestone moved past the standard Gym environments. I made a custom grid-world where shelves acted as immovable obstacles, and the agent was penalized for bumping into them. Q-learning didn’t care about the new setup because it just needed rules and a clear way to win. Watching the agent finally start to move efficiently around shelves was satisfying after all the trial runs and failures.

## What Stood Out

Q-learning is approachable and works for small, clear-cut problems. It has significant limits once you try to scale up. Deep RL carries more potential, but also a decent amount of instability and unpredictability. Stability methods help, and building custom environments is probably where most of the learning (and the headaches) happen.

## If You Use This

Splitting the work into clear milestones helped me keep my own confusion in check. Dependency management is always something to watch out for, even on Colab. Don’t skip the plots and visualizations; those slow-learning curves tell half the story. If nothing else, the process is just as much about working around limitations as it is about finding breakthroughs.

I hope this summary feels more honest than polished. Good luck if you decide to wrangle a warehouse robot yourself.
