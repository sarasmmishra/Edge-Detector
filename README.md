This repository contains a Verilog implementation of an edge detector module, along with its testbench. The edge detector identifies rising and falling edges of an input signal and outputs a pulse when an edge is detected.

Features:
1. Detects both rising and falling edges of a binary input signal.
2. Provides an output pulse on edge detection.
3. Parameterized states for modularity and readability.

Parameters:

1. The module uses the following states to detect edges:
2. IDLE: Initial state.
3. RISING_EDGE: Detects rising edges (0 to 1 transitions).
4. FALLING_EDGE: Detects falling edges (1 to 0 transitions).

Functionality:

1. On reset, the module initializes to the IDLE state.
2. The state transitions based on the input data_in and the current state.
3. An output pulse (edge_out) is generated when an edge is detected.

Simulation Details:

1. Clock period: 10ns
2. Reset signal is asserted high for 20ns.
3. Input signal (data_in) transitions are provided to test both rising and falling edges.

Waveform Example:

1. reset is asserted to initialize the module.
2. data_in transitions from 0 to 1 and 1 to 0 at regular intervals.
3. edge_out pulses are observed at each transition
