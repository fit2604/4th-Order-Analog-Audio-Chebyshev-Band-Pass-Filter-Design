# 4th-Order-Analog-Audio-Chebyshev-Band-Pass-Filter-Design

This project focuses on the design, simulation, and analysis of high-order active analog filters using LTspice. It features a comparative study between Chebyshev and Butterworth 2nd-order responses, implemented through various circuit topologies. The project validates theoretical models (Laplace transforms) against physical implementations using LM324 operational amplifiers.

Technical Specifications

1. Chebyshev Filter Design (2nd Order)
   The Chebyshev response is designed for a sharper roll-off at the expense of passband ripple.
   Biquad 1: fn1 = 695.5  Hz, Q = 1.306
   Biquad 2: fn2 = 3231 Hz, Q = 1.307.
   Damping Coefficients ($\zeta$): Calculated as 1/(2Q).

   2. Butterworth Filter Design (2nd Order)
    The Butterworth response is optimized for a maximally flat passband.
    Biquad 1: fn1 = 500 Hz, Q = 0.71.
    Biquad 2: fn2 = 4500 Hz, Q = 0.71

Circuit Topologies

The project implements these filters using two major active filter architectures:

Sallen-Key Topology: Chosen for its simplicity and low component count, used for both Butterworth and Chebyshev low-pass stages.

KHN (Kerwin-Huelsman-Newcomb) State-Variable: A robust topology that provides simultaneous Lowpass, Highpass, and Bandpass outputs with high stability.

Ideal vs. Real Comparison: Ideal behavior is modeled using Laplace Transfer Functions in voltage-controlled sources , while real-world behavior is simulated using LM324 Op-Amps.


Simulation and Analysis

The project includes two main types of simulations:

AC Analysis (.ac dec 300 0.01 300K): Used to generate Bode plots (Magnitude and Phase) to verify the frequency response and cut-off frequencies.

Transient Analysis (.tran 60m): Used to observe the time-domain behavior of the filters when subjected to various input signals.

CONCLUSION

This project provides a robust framework for designing and validating high-order active analog filters . By bridging the gap between mathematical models and physical hardware, it serves as a complete reference for professional signal conditioning.
      
