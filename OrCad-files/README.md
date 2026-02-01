## OrCAD Simulation Files

This ZIP archive contains OrCAD Capture simulation files used for circuit analysis and verification of the analog synthesizer design.

**File:** `simulations-files-from-OrCad.zip`

The archive includes a complete OrCAD project with separate schematic blocks and testbenches for individual functional sections of the system.

### Simulation blocks overview

- **synth_top**  
  Top-level schematic integrating all functional blocks into a complete system for overall verification.

- **exponential_sweep_tb**  
  Testbench used to analyze the exponential converter behavior and verify the control voltage to current/voltage relationship.

- **lfo_tb**  
  Testbench for the LFO block, used to verify oscillation frequency, waveform stability, and AGC behavior.

- **lintoexp**  
  Linear-to-exponential conversion block implementing the exponential response required for the 1 V/oct standard.

- **summator**  
  Summing amplifier block combining keyboard CV, octave shift voltage, and LFO modulation signal.

- **vco**  
  Core voltage-controlled oscillator block based on a relaxation oscillator topology (integrator + Schmitt trigger).

- **vco_tune_tb**  
  Testbench used to analyze VCO tuning accuracy, frequency range, and pitch deviation.

- **wien**  
  Wien bridge oscillator used as an LFO, including automatic gain control (AGC).

Each block can be simulated independently, while the top-level schematic allows verification of the complete signal chain and interaction between subsystems.
