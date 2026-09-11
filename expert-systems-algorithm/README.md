# expert-systems-algorithm
A collection of interactive Python notebooks demonstrating core expert system algorithms, from 20-questions-style games to rule-based logic and property elimination. Includes simple inference engines, animal identification, and explanation tracing, easily adaptable to other decision or diagnostic tasks.


## Project Overview
This project is all about building expert systems, the kind of programs that use a knowledge base and rules to guide users toward answers, instead of just guessing like a neural network. The “problem domain” here is animal identification: can you use a computer to help zoo visitors (or anyone, really) figure out what creature they're looking at?

Three different styles of system attack this (borderline silly but useful) question. Think “20 Questions” for animals, but with more logic and less shouting across a petting zoo fence.

### What’s Actually Inside
Animal Game: Almost a classic 20-questions game. It leads you through yes/no questions right up to a (mostly) sensible answer.

Truthifier: Stores animal facts as rule-based logic, then asks what it thinks are the most informative questions next.

Eliminator: Takes a slightly different route, using Boolean properties and logical deduction to rule out impossible candidates.

Want to diagnose an engine or troubleshoot a website? The machinery here isn’t just for animal fans and bored zoo guides, the structure works for almost any “decision tree” or diagnostics task.

### Why Not Just Use a Neural Net?
Expert systems might sound old-school, but they have one huge advantage over modern black boxes: explanations. They don’t just spit out an answer, they can tell you why they picked it. In fields where stakes are high or mistakes are expensive, that’s not nothing.

Training a neural network is quicker than building a decent expert ruleset, but you’ll never get the neural net to explain its decisions in plain language. If you want to know what an expert system’s thinking, it’ll give you chapter and verse (sometimes a little too eagerly).

### Core Techniques
Knowledge base creation (writing facts & rules)

Building simple inference engines

Picking best questions given current knowledge

Parsing and evaluating logical expressions (so if it says "has feathers AND lays eggs," you know what that means)

(Minimal UI, the focus here is the logic, not the window dressing)

### Milestones
Animal Game — animal_game.ipynb

Truthifier — truthifier.ipynb

Eliminator — eliminator.ipynb

### Getting Started
Open a notebook and run it.

Play around with rules and facts, add new animals or properties, or swap the animal questions for your own favorite decision problem.

### Shoutouts

- Project based on the Manning liveProject: _Simple AI Algorithms for Classification_

#### License

This is mainly meant for learning and tinkering, not commercial use.
