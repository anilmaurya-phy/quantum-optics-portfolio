🧪 INFN Research Project: Quantum Information with Integrated Photonics

This repository is complemented by experimental research conducted at the Istituto Nazionale di Fisica Nucleare (INFN), focusing on the implementation of a photonic Controlled-NOT (CNOT) gate using integrated silicon photonics.

🔬 Overview

The project explores how quantum information processing can be realized using photons as qubits in an integrated photonic platform.

Photons are encoded using polarization and manipulated through an on-chip optical circuit consisting of beam splitters, phase shifters, and interferometers.

⚙️ Experimental Architecture

The system consists of:

Photon Source
Twin photons generated via Spontaneous Parametric Down-Conversion (SPDC)
State Preparation
Polarization encoding of computational basis states:
|00⟩, |01⟩, |10⟩, |11⟩
Integrated Photonic Circuit
Silicon chip with:
Directional couplers (beam splitters)
Thermo-phase shifters (TPS)
Interference regions
Synchronization
Optical Delay Lines (ODLs) ensure simultaneous photon arrival
Detection System
Single-photon detectors (SNSPDs) + coincidence measurements (TDC)
🔄 Operational Flow
SPDC Source → State Preparation → Photonic CNOT Circuit → Detection
⚛️ CNOT Gate Operation
✔ Single-Photon Regime
Inputs: |00⟩, |01⟩
No quantum interference required
Deterministic propagation
High fidelity observed
✔ Two-Photon Interference Regime
Inputs: |10⟩, |11⟩
Requires Hong–Ou–Mandel interference
Quantum interference at beam splitters

For indistinguishable photons:

|1⟩ₐ |1⟩ᵦ → (|2⟩ₐ |0⟩ᵦ + |0⟩ₐ |2⟩ᵦ) / √2

➡ Leads to suppression of coincidence counts (HOM dip)

📊 Experimental Observations
✔ High fidelity (>95%) for |00⟩, |01⟩
⚠ Reduced fidelity for |10⟩, |11⟩
❌ Weak or absent HOM interference in early runs
Strong sensitivity to:
Phase stability (TPS)
Optical delay alignment
Photon indistinguishability
⚠️ Limiting Factor: Photon Source

The main limitation is the single-photon source:

g²(0) < 0.01 → confirms single-photon regime
No HOM dip → photons are distinguishable
Irregular photon spectrum observed
Temporal jitter and spectral mismatch

➡ The photonic circuit works correctly, but imperfect photons limit quantum interference

🔧 Current Work
Improving photon indistinguishability (spectral + temporal overlap)
Stabilizing thermo-phase shifters (TPS)
Fine-tuning optical delay lines (ODLs)
Collaboration with Aurea Technology for source optimization
🎯 Research Significance

This project demonstrates the bridge between quantum information theory and real experimental systems:

Quantum gates depend critically on physical parameters
Photon indistinguishability is essential for quantum computation
Integrated photonics enables scalable quantum technologies
🔗 Connection to This Repository

The simulations in this repository (entanglement, interferometers, etc.) are directly related to the experimental work:

Interferometer simulation → models beam splitter physics
Entanglement simulation → relates to photon correlations
Future work → includes HOM interference simulation
🚀 Next Step

Planned extension:

🔥 Simulation of Hong–Ou–Mandel interference
Photonic quantum circuit modeling
Noise and decoherence analysis
