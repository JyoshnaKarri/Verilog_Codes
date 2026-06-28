# Verilog RTL Portfolio — 50+ Modules with Waveforms

A structured collection of 50+ RTL modules written in Verilog, covering combinational logic, sequential circuits, communication protocols, and digital design patterns — each with a testbench and GTKWave waveform verification.

**Tools:** Icarus Verilog · GTKWave  
**Language:** Verilog HDL  
**Live Site:** [View Portfolio](https://jyoshnakarri.github.io/Verilog_Codes/)

---

## 📦 Module Categories

### Combinational Logic
| Module | Description |
|---|---|
| Half Adder | 1-bit addition — sum and carry |
| Full Adder | 1-bit addition with carry-in |
| 4-bit Ripple Carry Adder | Chained full adders |
| 2:1 / 4:1 Multiplexer | Datapath selection logic |
| Decoder (2:4, 3:8) | Binary to one-hot |
| Encoder (4:2, 8:3) | One-hot to binary |
| Priority Encoder | Outputs highest active input |
| Comparator | Magnitude comparison of two numbers |
| ALU | Arithmetic and logic unit — ADD, SUB, AND, OR, XOR, SLT |

### Sequential Logic
| Module | Description |
|---|---|
| D / JK / T Flip-Flop | Core memory elements |
| 4-bit Ring Counter | Shift-register based counter |
| Johnson Counter | Twisted ring counter |
| Up/Down Counter | Configurable direction counter |
| LFSR | Linear Feedback Shift Register — pseudo-random sequence |
| Mealy FSM | Output depends on state + input |
| Moore FSM | Output depends only on state |
| PWM Generator | Configurable duty cycle pulse-width modulator |
| Shift Register (SISO/SIPO/PISO/PIPO) | All four shift register types |

### Communication Protocols
| Module | Description |
|---|---|
| UART TX | Serial transmitter — configurable baud rate |
| UART RX | Serial receiver with start/stop bit detection |
| SPI Slave | SPI protocol — slave mode implementation |

### Memory & FIFO
| Module | Description |
|---|---|
| Synchronous FIFO | Single-clock FIFO with full/empty flags |
| Asynchronous FIFO | Dual-clock FIFO with Gray code pointers |
| Single-Port RAM | Read/write memory — synchronous |
| ROM | Read-only memory — combinational output |

### Clock Domain Crossing (CDC)
| Module | Description |
|---|---|
| 2-FF Synchroniser | Metastability-safe signal synchroniser |
| Pulse Synchroniser | Single-pulse transfer across clock domains |
| Handshake Protocol | Valid-ready handshake for CDC data transfer |
| Glitch-Free Clock Mux | Safe clock switching between two domains |
| Reset Synchroniser | Async assert, synchronous deassert |

### Verification & Miscellaneous
| Module | Description |
|---|---|
| CRC-8 | Cyclic redundancy check — error detection |
| Arbiter | Priority-based bus arbiter |
| Debounce Circuit | Button debounce using FSM |

---

## 🛠️ How to Simulate

```bash
# Compile
iverilog -o output.vvp module.v module_tb.v

# Run simulation
vvp output.vvp

# View waveform
gtkwave output.vcd
```

---

## 📁 Repository Structure

```
Verilog_Codes/
├── combinational/
│   ├── half_adder.v · half_adder_tb.v
│   ├── full_adder.v · full_adder_tb.v
│   └── ...
├── sequential/
│   ├── d_flipflop.v · d_flipflop_tb.v
│   ├── pwm.v · pwm_tb.v
│   └── ...
├── protocols/
│   ├── uart_tx.v · uart_tx_tb.v
│   ├── uart_rx.v · uart_rx_tb.v
│   └── ...
├── memory/
│   ├── sync_fifo.v · sync_fifo_tb.v
│   ├── async_fifo.v · async_fifo_tb.v
│   └── ...
├── cdc/
│   └── ...
└── waveforms/
    └── (GTKWave screenshots for each module)
```

---

## 🔗 Links

- 🌐 [Live Portfolio Site](https://jyoshnakarri.github.io/Verilog_Codes/)
- 📂 [100 Days VLSI Journey](https://github.com/jyoshnakarri/100-days-vlsi)
- 💼 [LinkedIn](https://www.linkedin.com/in/jyoshna-k-5b1626401/)
