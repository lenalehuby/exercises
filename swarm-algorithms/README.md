# swarm-algorithms

## Project Overview
### Flock Logic & Swarm Sense
### Why Simulate Swarms?
There’s something oddly compelling about watching a flock twist and turn, or seeing a swarm of insects shift as one big cloud. For researchers and tinkerers alike, these group dynamics raise a lot of questions: Do big and small flocks actually behave differently? How do they react to obstacles like trees, people, or the occasional telephone pole? And what makes this “swarm intelligence” look so organized, even when it isn't?

This project explores those questions through simulation. The models here aren’t just limited to birds; swap the sprites out, and you could be simulating sheep, partygoers, or a crowd at a concert. Sometimes, the rules are surprisingly universal.

### What’s in This Repo?
The main focus is on two families of algorithms:

Swarm and flocking simulations (inspired by bird, bug, and herd behavior)

A swarm-inspired search algorithm for finding maximum points on tricky surfaces ("where's the highest hill in a weird landscape?")

You’ll find code for both “classic” boids, alignment, cohesion, separation, and more physics-y variants (“gravity boids”), with and without obstacles to bump into. The optimization notebook sends virtual agents to crawl all over a surface, testing whether a swarm can figure out where the biggest peak actually is.

### Is This “AI”?
Well, it depends. Machine learning tools (especially neural networks) get all the buzz, but there’s a long tradition of “artificial” agents just following simple rules, and sometimes those rules lead to pretty convincing results. Swarm intelligence may not write poetry or play chess, but it does let digital creatures fake teamwork surprisingly well.

### Techniques & Tools Used
Vector arithmetic modules (you need math before you get to birds)

Boids: basic flocking behavior

Obstacles: making things harder for flocks

Gravity-inspired swarms: a nudge toward realism

Particle Swarm Optimization: for tricky optimization landscapes

tkinter (for fast, if not pretty, visualizations)

If you want fancier graphics, you could swap in Pygame or something with more polish. But the focus here is what the code is doing, not how fancy it looks.

## Milestones
Vector Arithmetic — vector_arithmetic.ipynb

Boids — boids.ipynb

Boids with Obstacles — boids_with_obstacles.ipynb

Gravity Boids — gravity_boids.ipynb

Gravity Boids with Obstacles — gravity_boids_with_obstacles.ipynb

Swarm-based Maximum Finder — swarm_maximum.ipynb

### How to Get Started
Grab a notebook, make sure Python and some basics (numpy, tkinter) are installed, and start running things. Change up the number of agents, tweak parameters, toss in more obstacles and don’t be afraid to break something. That’s usually where the learning happens.

### Shoutouts
Project based on the Manning liveProject: Simple AI Algorithms for Classification

### License
This is mainly meant for learning and tinkering, not commercial use.
