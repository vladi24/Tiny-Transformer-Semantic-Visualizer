# Tiny Transformer Semantic Visualizer

A standalone interactive simulator that makes the internal mechanics of a Transformer easier to see, inspect, and reason about.

Instead of treating language models as opaque black boxes, this project turns core Transformer ideas into something visual and manipulable: semantic vectors, contextual shifts, attention weights, layer-by-layer evolution, and next-token prediction.

**Live demo:** https://vladi24.github.io/Tiny-Transformer-Semantic-Visualizer/

---

## What this is

This project is a **didactic, interactive Transformer simulator** built to help users develop intuition for how meaning can be represented and transformed inside a model.

It focuses on visibility and interpretability:

- words are represented as semantic vectors
- context changes those vectors across layers
- attention weights can be inspected directly
- the full pipeline can be explored step by step
- high-dimensional relationships are projected into a 3D semantic space

The goal is not to hide complexity behind abstraction, but to expose the moving parts clearly enough that a curious user can follow them.

---

## What this is not

This is **not** a production language model, and it is **not** intended as a faithful reproduction of a modern large-scale LLM.

It is a **conceptually simplified but structurally honest** simulator of key Transformer ideas, designed for understanding rather than benchmark performance.

If you want to *see* what embeddings, attention, contextual refinement, and token prediction are doing, this is for you.

---

## Why it exists

Transformer-based models are often discussed in ways that feel either too abstract or too magical.

This project was built to bridge that gap.

It offers a **glass-box view** of language-model mechanics, making concepts such as:

- embeddings
- attention
- residual refinement
- feed-forward transformation
- semantic clustering
- next-token prediction

feel less like invisible mathematics and more like an inspectable system.

---

## Core idea

The simulator represents words through a set of **human-readable semantic dimensions**, then lets those representations evolve under contextual interaction.

As tokens pass through the model:

1. they begin with a base semantic profile
2. attention reweights relationships between them
3. representations shift depending on surrounding words
4. the resulting state is visualized both numerically and spatially

This makes it possible to observe meaning not as a fixed dictionary entry, but as something dynamically reshaped by context.

---

## Features

### 3D semantic map
Watch token representations move and reorganize in real time as layers change.

### 12-dimensional semantic vectors
Each word is mapped across interpretable semantic axes such as concreteness, action, abstraction, sociality, technicality, and more.

### Interactive Transformer pipeline
Explore the model step by step, from input representation to attention and prediction.

### Attention heatmaps
Inspect how strongly tokens relate to one another within a sentence.

### 3D dictionary view
Browse a larger semantic landscape and observe clusters of related words.

### Layer-by-layer evolution
Move through the model depth and see how token meaning becomes context-sensitive.

### Next-token prediction
Observe how the current state of the sequence influences likely continuations.

### Zero-dependency deployment
Runs directly in the browser as a standalone HTML/JS project.

---

## Literary corpus

The simulator is grounded in a small corpus of classic Italian literature, used as the semantic background for its language space and prediction behavior.

This gives the project a distinct identity: it is not just a generic AI demo, but a semantic playground shaped by a specific linguistic and literary atmosphere.

---

## How it works

At a high level, the simulator follows this logic:

- **Static semantic initialization**  
  Tokens start from a base semantic representation.

- **Contextual interaction**  
  Attention updates each token based on the others in the sequence.

- **Layered refinement**  
  Meaning becomes progressively more contextual as you move through layers.

- **Projection into 3D space**  
  High-dimensional relationships are mapped into a visual space for exploration.

The result is not a full industrial Transformer implementation, but a simplified environment where the logic of the architecture becomes easier to grasp.

---

## How to use it

### 1. Enter a phrase
Choose a preset sentence or write your own.

### 2. Adjust the controls
Experiment with:

- temperature
- positional encoding
- layer depth
- pipeline step controls

### 3. Explore the views
Use the tabs to inspect the model from different angles:

- **3D Map** for contextual embeddings
- **3D Dictionary** for broader semantic structure
- **Heatmap** for attention relationships
- **Pipeline** for step-by-step mechanics
- **Details** for per-token semantic inspection

### 4. Run experiments
Try changing the surrounding words of an ambiguous token and observe whether its position and relationships change.

That is where the project becomes most interesting: when you can *see* context altering meaning.

---

## Suggested experiments

### Ambiguous word test
Use a word with multiple possible meanings and place it in different sentence contexts.

### Genre/style influence
Write phrases that evoke adventure, nature, or technical discourse and observe how predictions and clustering respond.

### Matrix perturbation
Modify Q/K/V-related parameters and watch how attention behavior deforms.

This is a very direct way to understand how sensitive the system is to internal structure.

---

## Who this is for

This project is especially useful for:

- students trying to understand Transformer mechanics
- teachers who want a visual explanation tool
- curious non-specialists who find standard explanations too abstract
- developers who want an intuitive toy model before dealing with large frameworks

---

## Technical philosophy

This project deliberately favors:

- interpretability over scale
- intuition over benchmark performance
- conceptual clarity over architectural completeness

Its purpose is educational, exploratory, and explanatory.

---

## AI-assisted development

This project was rapidly prototyped with AI-assisted development, guided by a specific didactic and interface design goal.

The value of the project is not in “AI generated code” as such, but in the combination of:

- conceptual design
- interface choices
- explanatory structure
- semantic framing
- interactive experimentation

---

## Running locally

Clone the repository and open `index.html` in a browser.

```bash
git clone https://github.com/vladi24/Tiny-Transformer-Semantic-Visualizer.git
cd Tiny-Transformer-Semantic-Visualizer
