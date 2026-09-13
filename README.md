# Pseudo-NMOS-Based-2-1-Multiplexer
Design and transient simulation of a pseudo-NMOS 2:1 multiplexer using Cadence Virtuoso.


## Objective

Design and analyze a 2:1 multiplexer using pseudo-NMOS logic and verify its functionality through transient simulation in Cadence Virtuoso.

## Concept

Pseudo-NMOS logic uses an always-ON PMOS transistor as the pull-up network and NMOS transistors as the pull-down network. It reduces transistor count compared to conventional CMOS logic but introduces static power dissipation and degraded output levels.

A CMOS inverter is added at the output to restore the logic levels and improve the output voltage swing.

## Circuit Description

- Inputs: A, B
- Select: S
- Output: Y
- Supply Voltage: 1.8 V
- Logic Style: Pseudo-NMOS

The NMOS pull-down network selects the required input based on the select signal, while the always-ON PMOS provides the pull-up path.

## Tools Used

- Cadence Virtuoso
- Schematic Editor
- Transient Simulation

## Design Implementation

![MUX Schematic](image.png)

The design consists of an always-ON PMOS pull-up, an NMOS pull-down network, and a CMOS inverter for output signal restoration.

## Testbench

![Testbench](testbench.jpeg)

Pulse voltage sources are applied to A, B, and S, with a 1.8 V DC supply used for the circuit.

## Simulation Results

![Waveform](waveform.jpeg)

Transient simulation verifies the multiplexer functionality and demonstrates the degraded output level before the inverter and the restored logic swing after the inverter.

## Key Observations

- Reduced transistor count compared to conventional CMOS logic
- Static power dissipation due to the always-ON PMOS
- Degraded output voltage levels in pseudo-NMOS logic
- Improved output swing using a CMOS inverter
- Trade-off between area, power, and performance

## Google site link
https://sites.google.com/view/cmosopenended/results

## Conclusion

The pseudo-NMOS based 2:1 multiplexer was successfully designed and simulated in Cadence Virtuoso. The design demonstrates the advantages of reduced transistor count while highlighting the static power and output-level limitations of pseudo-NMOS logic.
