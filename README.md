# Tiny-Transformer-Semantic-Visualizer
A standalone, 0.9MB single-file HTML interactive simulator that visualizes how a Transformer model conceptualizes semantics using classic Italian literature.

Link: https://vladi24.github.io/Tiny-Transformer-Semantic-Visualizer/

The Project
Born from a "bored afternoon" and a conversation with an AI agent, this tool was built to deconstruct and visualize the mathematical representation of meaning. It’s a "glass-box" approach to understanding Large Language Models (LLMs), moving away from the "black-box" mystery.
It was made entirely by codex, with my inputs explaining the structure and the features.


Featured Corpus
The simulator processes and maps the semantic space of 5 classic Italian masterpieces:

Pinocchio (Collodi)
Cuore (De Amicis)
Al Polo Australe in Velocipede (Salgari)
I promessi sposi (Manzoni)
I Robinson (Calgari)


Key Features
3D Semantic Map: Watch word embeddings shift and cluster in real-time.

12-Dimensional Vectors: Every word is mapped across 12 human-readable semantic axes (Concrete, Animate, Human, Action, Abstract, Nature, Social, Temporal, Functional, Technical, Frequency, Syntax).

Interactive Pipeline: Step-by-step visualization of Embedding, Attention, and Softmax layers.

Attention Heatmaps: See exactly how the model "relates" words within a sentence context.

Zero-Dependency: Runs anywhere. No Python, no pip install, no server. Just raw HTML/JS and Three.js.

Deep Feature Inspection: Full 12-dimensional semantic breakdown for every token.

Smart OOD Handling: Contextual mapping for words outside the core dictionary based on the books.


How it works
The simulator uses a simplified but mathematically honest implementation of the Transformer architecture.
Static Embeddings: Words are initialized based on their 12D semantic traits.
Contextual Shift: As tokens pass through layers, the Attention Mechanism recalculates their positions based on the surrounding context.
Visualization: High-dimensional math is projected into a 3D space using Three.js for intuitive exploration.

How to Use
1. Setting the Scene (Sidebar)
Input Phrase: Choose a preset phrase or type your own. This is the sequence the model will "analyze."

Hyperparameters:

Temperature: Controls randomness in text prediction. High = creative/chaotic, Low = predictable.

Position Encoding: Adjusts how much the "order" of words affects their meaning.

Layer Selection: This is the most important slider. It allows you to travel through the model's "depth." Layer 0 is the raw dictionary meaning; higher layers show the meaning "refined" by context.

Pipeline Controls: Use the Step Forward/Back buttons to follow the mathematical journey of a token from input to prediction.

2. Exploring the Tabs (Workspace)
🗺️ 3D Map (The Heart of the Sim)
This is a 3D projection of the Contextual Embeddings.

Observe the Shift: Move the Layer slider and watch how words physically move in space as they "understand" each other.

Interaction: Click on a word sphere to see its 12-Dimensional Semantic Profile (Concrete, Animate, etc.).

📖 3D Dictionary
A massive cloud of 1,000+ words mapped by their base meanings.

Clusters: Look for "clouds" of similar words (e.g., animals, emotions, locations).

Search: Use the search bar to find specific words and see where they sit in the Italian language landscape.

🔥 Heatmap (Attention Mechanism)
This grid shows the "Relationship Weights" between words.

Reading the grid: If the cell between "Gatto" and "Mangia" is bright, it means the model is using the word "Mangia" to understand "Gatto."

Layered Insight: See how attention refocuses as you move through different layers.

🏗️ Pipeline
A technical step-by-step breakdown. Perfect for verifying the math:

Embedding -> Attention -> Add & Norm -> Feed Forward.

It includes a Next Token Predictor that suggests the most likely next word based on the 5 included books (Pinocchio, Salgari, etc.).

3. Recommended Experiments
To truly understand how an AI "thinks," try these:

The Context Test: Type a sentence with an ambiguous word. Change the surrounding words and watch (in the 3D Map) if that word's dot moves towards a different cluster.

The "Salgari" Effect: Type a sentence about the sea or adventure. See if the Text Prediction (in Pipeline) suggests words typical of Salgari’s style.

Matrix Sabotage: (Advanced) Try slightly editing the Q, K, or V matrices in the sidebar. You’ll see the Attention Heatmap distort, showing how the "brains" of the AI are wired.

💡 Pro Tip
If a word isn't in the core 1,000-word dictionary, the simulator will use Smart Contextual Mapping. It will "guess" the semantic dimensions of the unknown word by looking at its neighbors


Why this exists
This project demonstrates the power of AI-Augmented Development. By using an AI agent as an "orchestrator," I was able to bridge the gap between complex linear algebra, 3D rendering, and linguistic theory in a single afternoon.
