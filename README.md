# Tiny-Transformer-Semantic-Visualizer
A standalone, 0.8MB single-file HTML interactive simulator that visualizes how a Transformer model conceptualizes semantics using classic Italian literature.

🌟 The Project
Born from a "bored afternoon" and a conversation with an AI agent, this tool was built to deconstruct and visualize the mathematical representation of meaning. It’s a "glass-box" approach to understanding Large Language Models (LLMs), moving away from the "black-box" mystery.

📚 Featured Corpus
The simulator processes and maps the semantic space of 5 classic Italian masterpieces:

Pinocchio (Collodi)

Cuore (De Amicis)

Al Polo Australe in Velocipede (Salgari)

I promessi sposi (Manzoni)

I Robinson (Calgari)

🛠 Key Features
3D Semantic Map: Watch word embeddings shift and cluster in real-time.

12-Dimensional Vectors: Every word is mapped across 12 human-readable semantic axes (Concrete, Animate, Human, Action, Abstract, Nature, Social, Temporal, Functional, Technical, Frequency, Syntax).

Interactive Pipeline: Step-by-step visualization of Embedding, Attention, and Softmax layers.

Attention Heatmaps: See exactly how the model "relates" words within a sentence context.

Zero-Dependency: Runs anywhere. No Python, no pip install, no server. Just raw HTML/JS and Three.js.

Deep Feature Inspection: Full 12-dimensional semantic breakdown for every token.

Smart OOD Handling: Contextual mapping for words outside the core dictionary based on the books.

🧠 How it works
The simulator uses a simplified but mathematically honest implementation of the Transformer architecture.

Static Embeddings: Words are initialized based on their 12D semantic traits.

Contextual Shift: As tokens pass through layers, the Attention Mechanism recalculates their positions based on the surrounding context.

Visualization: High-dimensional math is projected into a 3D space using Three.js for intuitive exploration.

🚀 Why this exists
This project demonstrates the power of AI-Augmented Development. By using an AI agent as an "orchestrator," I was able to bridge the gap between complex linear algebra, 3D rendering, and linguistic theory in a single afternoon.
