---
layout: page
permalink: /projects/index.html
title: Projects
---

## Projects

A collection of things I'm building or have built. I use these projects to learn, experiment, and solve problems I find interesting.

### Current Work

**Akshara Mantapa: Infinite Kannada Text Library** · [GitHub](https://github.com/sanathNU/Akshara-Mantapa) · [Web Demo](/https://sanathnu.github.io/Akshara-Mantapa/)  
*Rust, WebAssembly, SvelteKit*  
* Implemented a searchable infinite Kannada text corpus inspired by Borges’ *Library of Babel*.
* Built a 56,028-symbol grapheme-cluster alphabet for Indic scripts using greedy longest-match segmentation.
* Architected a dual-runtime Rust backend with an Axum HTTP server for development and WebAssembly compilation via `wasm-pack` for static deployment.
* Designed a minimalist SvelteKit frontend with hierarchical addressing, real-time search highlighting, and smooth page navigation.

**Double Ratchet Algorithm** · [GitHub](https://github.com/sanathNU/DoubleRatchetJava)
* A Java implementation of Signal’s [Double Ratchet cryptographic protocol](https://signal.org/docs/specifications/doubleratchet/) that generates a fresh encryption key for each message, providing forward secrecy and post-compromise security for asynchronous encrypted messaging.

**Exploring Cryptography**
* Studying and documenting post-quantum cryptographic schemes, with a focus on lattice-based protocols including [CRYSTALS-Kyber](https://pq-crystals.org/kyber/) and [CRYSTALS-Dilithium](https://pq-crystals.org/dilithium/), emphasizing their design principles and practical implications.

---

### Archived Projects

A list of projects I've worked on in the past.

*   **Customer Personality Analysis Project** - Analyzed customer data from Kaggle using clustering techniques (K-Means, Agglomerative Clustering, DBSCAN) to segment personalities into Browsers, Aristocrats, and Need-Based customers, providing insights to optimize marketing strategies.
    *   **Technologies**: Numpy, Pandas, SMOTE Scikit-learn, Scipy
<br> <br>

*   **Kannada MNIST Autoencoder Project** - Trained an Autoencoder on the Kannada handwriting dataset, testing different layer configurations to see what worked best for capturing the nuances in the data.  ([Notebook link](https://github.com/sanathNU/Kannada-MNIST-Autoencoder))
    *   **Technologies**: Tensorflow, PyTorch

