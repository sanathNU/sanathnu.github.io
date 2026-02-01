---
layout: page
permalink: /projects/index.html
title: Projects
---

# Projects

A collection of things I'm building or have built. I use these projects to learn, experiment, and solve problems I find interesting.

## Current Work

**∞ Akshara Mantapa: Infinite Kannada Text Library** · [GitHub](https://github.com/sanathNU/Akshara-Mantapa) · [Web Demo](https://sanathnu.github.io/Akshara-Mantapa/)  
*Rust, WebAssembly, SvelteKit*  
* Implemented a searchable infinite Kannada text corpus inspired by Borges’ [*Library of Babel*](https://en.wikipedia.org/wiki/The_Library_of_Babel).
* Built a 57,324-symbol grapheme-cluster alphabet for Indic scripts using greedy longest-match segmentation.
* Architected a dual-runtime Rust backend with an Axum HTTP server for development and WebAssembly compilation via `wasm-pack` for static deployment.
* Designed a minimalist SvelteKit frontend with hierarchical addressing, real-time search highlighting, and smooth page navigation.

---

**🔑 End-to-End Encryption Engine with Double Ratchet** · [GitHub](https://github.com/sanathNU/DoubleRatchetJava) 
*Java, Java Cryptography Extension (JCE)*

* Implemented Double Ratchet–based end-to-end encrypted asynchronous messaging in Java.
* Achieved forward secrecy and post-compromise security using ECDH, HKDF, AES-GCM, and HMAC-SHA256.

---

**⚛️ Post-Quantum & ZK Proof Benchmarking Framework** · [GitHub](https://github.com/sanathNU)
*Rust, ml-kem, arkworks, Docker, Kubernetes*

* Designed HTTP microservices wrapping ml-kem (NIST FIPS 203) and arkworks R1CS Groth16 implementations.
* Measured ~17x throughput gap between lattice-based KEM and ZK proving across parameter sets.
* Containerized services with Kubernetes manifests for horizontal scaling experiments.

---

## Archived Projects

A list of projects I've worked on in the past.

*   **Customer Personality Analysis Project** - Analyzed customer data from Kaggle using clustering techniques (K-Means, Agglomerative Clustering, DBSCAN) to segment personalities into Browsers, Aristocrats, and Need-Based customers, providing insights to optimize marketing strategies.
    *   **Technologies**: Numpy, Pandas, SMOTE Scikit-learn, Scipy
<br>

*   **Kannada MNIST Autoencoder Project** - Trained an Autoencoder on the Kannada handwriting dataset, testing different layer configurations to see what worked best for capturing the nuances in the data.  ([Notebook link](https://github.com/sanathNU/Kannada-MNIST-Autoencoder))
    *   **Technologies**: Tensorflow, PyTorch

