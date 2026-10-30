---
layout: page
permalink: /projects/index.html
title: Projects
---

# Projects

A collection of things I'm building or have built. I use these projects to learn, experiment, and solve problems I find interesting.

## Selected Projects

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

## Hackathons & Short Builds

Weekend hackathons and course projects, mostly built with teammates. Rough edges, fast ideas.

*   **Symbolon** · [GitHub](https://github.com/anurag-bg-neu/symbolon) · *Hackachusetts, Oct 2026* (4th place)  
    Privacy-preserving genetic carrier screening: couples compare lab-signed carrier genes via Diffie-Hellman private set intersection over ristretto255, learning only their shared risk, while selective disclosure lets a patient prove trial eligibility without revealing the rest of their genome.
    *   **Technologies**: Python, FastAPI, libsodium (ristretto255), Ed25519
<br>

*   **Benchwork** · [GitHub](https://github.com/varshiniskamath24/Benchwork) · *OpenAI Hackathon, Jul 2026*  
    Biology research engine that turns a plain-English question into a query pipeline over live databases (UniProt, ChEMBL, Open Targets, STRING), building a provenance-tracked knowledge graph where every claim is tiered as evidenced, inferred, or an open hypothesis.
    *   **Technologies**: Python, TypeScript, SQLite
<br>

*   **CGE-RL: Consensus-Gated Ensemble RL** · [GitHub](https://github.com/sanathNU/CGE-RL) · *Course Project, Apr 2026*  
    Dual-process ensemble RL that pairs heterogeneous agents (DQN/SAC + PPO) and gates on KL divergence between their policies: agreement yields a fast consensus action (System 1), disagreement hands off to a deliberate meta-controller (System 2).
    *   **Technologies**: Python, Stable-Baselines3, Gymnasium
<br>

*   **Bit Bounty** · [GitHub](https://github.com/yashasuttangi/crypto-bounty) · *MIT Bitcoin Hackathon, Apr 2026*  
    Trustless bug bounty protocol where ETH payouts trigger on cryptographic proof, not human review: hunters submit exploit bytecode, the contract runs it inside an always-reverting self-call, and pays out atomically if an invariant breaks.
    *   **Technologies**: Solidity, TypeScript, Python
<br>

*   **Parsel** · [GitHub](https://github.com/Aryan7901/SAKS) · *Red Hat Hackathon, Mar 2026* (People's Choice Award)  
    Local-first desktop app: drop in an invoice or DNA sequence and on-device LLMs return structured data, with nothing leaving the machine and optional Google Sheets sync via MCP.
    *   **Technologies**: Tauri, React, TypeScript, Python, RamaLama
<br>

*   **Eathos** · [GitHub](https://github.com/keivalya/eathos) · *Google × DeepMind Hackathon, Mar 2026*  
    Multi-agent AI nutritionist that turns one fridge photo into a waste-reducing meal plan, prioritizing soon-to-expire ingredients, with a human-in-the-loop step to confirm what was detected.
    *   **Technologies**: Python, FastAPI, Google ADK, Gemini, React

---

## Archived Projects

A list of projects I've worked on in the past.

*   **Customer Personality Analysis Project** - Analyzed customer data from Kaggle using clustering techniques (K-Means, Agglomerative Clustering, DBSCAN) to segment personalities into Browsers, Aristocrats, and Need-Based customers, providing insights to optimize marketing strategies.
    *   **Technologies**: Numpy, Pandas, SMOTE Scikit-learn, Scipy
<br>

*   **Kannada MNIST Autoencoder Project** - Trained an Autoencoder on the Kannada handwriting dataset, testing different layer configurations to see what worked best for capturing the nuances in the data.  ([Notebook link](https://github.com/sanathNU/Kannada-MNIST-Autoencoder))
    *   **Technologies**: Tensorflow, PyTorch

