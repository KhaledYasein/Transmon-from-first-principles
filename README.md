# Transmon Physics from First Principles

A line-by-line derivation of transmon-qubit physics and the three native two-qubit gates (flux-controlled, cross-resonance, parametric), with reproducible QuTiP notebooks.

> **Author:** Khaled Yasein
> **Source material:** Based on the lecture course *Quantum Computing with Superconducting Qubits* (Prof. S. Filipp, TUM / Walther-Meißner-Institut). The derivations, organisation, and exposition in this repository are my own work, developed while studying the course; the underlying physics and pedagogical scope follow the course content.

## Why this repo exists

The transmon literature is split between two extremes: comprehensive reviews and original papers (Koch 2007, Krantz 2019, Blais 2021) that compress many algebraic steps, and tutorials that skip the parts where the physics actually lives — the Schrieffer–Wolff transformation for the cross-resonance gate, the three-level structure that makes the entangling rate non-zero, the renormalisation of the qubit capacitance by the resonator coupling.

This repo fills the middle. It is a line-by-line derivation of the transmon and its native two-qubit gates, paired with notebooks that numerically verify each result. If you have ever read a paper that says "after a Schrieffer–Wolff transformation one obtains..." and wanted to actually do the transformation, this is for you.

## What's inside

### notes/ — Four PDF derivation references

- **Lecture5_Deep_Derivations.pdf** — LC oscillator, graph-theoretic circuit quantization, Josephson effect from the tunneling Hamiltonian, CPB, transmon via Taylor expansion and RWA.
- **Lecture5_Worked_Example_Transmon_Resonator.pdf** — Concrete circuit (3 capacitors + 1 JJ + 1 inductor), Lagrangian, capacitance matrix inversion, Jaynes–Cummings, dispersive readout via Schrieffer–Wolff.
- **Lecture6_CPB_Transmon_cQED_Decoherence.pdf** — CPB in the charge basis, charge-dispersion suppression, transmon regime, inductively shunted qubits, cQED, dispersive readout with three-level correction, decoherence channels.
- **TwoQubitGates_FirstPrinciples_Reference.pdf** — Full derivations of all three native two-qubit gate families: flux-controlled (iSWAP), cross-resonance (CNOT via ZX), parametric (iSWAP / CZ). Schrieffer–Wolff for CR with explicit commutators, static-ZZ analysis, tunable couplers, virtual-Z calibration.

### notebooks/ — Reproducible QuTiP verifications (coming soon)

Numerical verification of each major analytical result, designed to be runnable end-to-end on a clean Python environment.

## License

Notes: CC-BY 4.0 (attribution required, derivative works allowed).
Code: MIT.

## Contact

Khaled Yasein — ge62zom@mytum.de

If you find a typo, a sign error, or a derivation that could be cleaner, please open an issue.