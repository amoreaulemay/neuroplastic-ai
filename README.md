# Neuroplastic AI

**An Open Source Exploration into Neuroplastic Neural Networks**

## Overview

**Neuroplastic AI** is a personal experimental project that aims to explore a novel approach to adaptive neural 
networks inspired by neuroplasticity. The project is built on the idea of evolving a neural network's basic operational 
nodes -- such as arithmetic operators and logic gates -- through iterative epochs of training, mutation, and optimization.
While this project is inspired by established ideas in neural networks and evolutionary computation, it is purely 
exploratory and experimental.

---

## Disclamer

**Important Notice:**

- This project represents personal experimentation and exploration. I do **not** hold a PhD in this field, and the ideas
here have not been peer-reviewed.
- The methods and experiments within this repository are provided "as-is" for educational and exploratory purposes. There
is no guarantee that any approach will work as intended.
- Use, modify, and experiment with the code at your own risk.

---

## Project Motivation and Concept

The primary goal of **Neuroplastic AI** is to simulate a form of neuroplasticity in a neural network. The code concepts
include:

1. **Basic Operational Nodes:**
The network begins with fundamental nodes (e.g., addition, subtraction, logic gates) that perform elementary operations.

2. **Epoch-Based Learning:**
  - Given a specific problem and an expected solution, the network runs multiple epochs trying to compute the solution.
  - In each epoc, the network's current configuration attempts to generate a correct solution. The outcome can be one,
  several, or no solutions.

3. **Randomized Mutation and Evolution:**
  - If a solution is not found, the network introduces randomized mutations to certain nodes, essentially "evolving" the
  network's structure.
  - The mutated configuration is tehn tested in subsequent epochs.
  - Mutations that lead to a correct solution are retained; otherwise, they are discarded.

4. **Pathway Embedding and Compression:**
  - Every problem is embedded within the system to create a unique representation.
  - As the network discovers multiple pathways to a solution, it compresses these pathways to identify the most optimized one.
  - The optimized pathway is saved as a new operation node, which encapsulates the original computation pipeline.

5. **Guided Problem Solving with RAG:**
  - For new problems, the system uses an embedding approach combined with a Retrieval-Augmented Generation (RAG) framework.
  - Cosine similarity and a reranker help find previous, similar problems, providing an initial guess at an optimal solution
  pathway based on a preset threshold.

---

## Roadmap and Experimentation

This project will combine theoretical exploration with small-scale experiments. The primary areas of focus include:

- [ ] **Theoretical Documentation:**
  - [ ] Outline the principles behind neoplasticity in neural networks.
  - [ ] Discuss the potential benefits, challenges, and limitations of evolving operational nodes.
- [ ] **Prototype Experiments:**
  - [ ] Test the effectiveness of mutation and selection in evolving node configurations.
  - [ ] Evaluate the process of compressing pathways into new, optimized operational nodes.
  - [ ] Implement and refine the RAG mechanism to guide problem-solving based on similar past problems.

---

## Contributing

Contributions, suggestions, and ideas are very welcome! If you'd like to help improve or experiment further with this project:

1. Fork the repository.
2. Create your feature branch: `git switch -c feature/your-feature`
3. Commit your changes: `git commit -m "feat: add some feature"`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a pull request.

Please open an issue to discuss major changes before proceeding with them.

---

## License

This project is open-sourced under the MIT License.
