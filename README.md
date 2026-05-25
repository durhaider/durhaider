# Dur E Haider Hussain Fayyaz

**Final-year Computer Engineering student at NUST**, specializing in FPGA-based digital systems, hardware acceleration, and real-time systems optimization. Strong proficiency in Verilog/VHDL design, FPGA implementation, and CUDA-accelerated compute pipelines.

---

## Current Work

Currently completing my **Final Year Project**: a GPU-accelerated medical imaging pipeline for 3D lung tumor reconstruction and segmentation. Every CUDA optimization, from kernel fusion to memory coalescing to stream-based overlap.

- **CUDA kernel optimization:** Achieved **~8.7× speedup (52 min → 6 min)** through kernel fusion, batched memory transfers, and occupancy-driven block sizing
- **Memory hierarchy optimization:** Coalesced access patterns, shared-memory tiling, and compute/I/O stream overlap
- **Texel density balancing:** Stabilizing texture resolution on tumor boundaries for clinical reliability
- **GPU–FPGA co-design direction:** Exploring hybrid architectures for real-time medical visualization

---

## Technical Focus

### FPGA & Hardware Design (primary strength)

- **Verilog/VHDL:** RTL design, parameterized modules, FSM-based controllers, generate statements
- **FPGA implementation:** Spartan-6 (Nexys 3), Xilinx UltraScale+ (ZCU106/KCU105)
- **Toolchain:** Vivado, Xilinx ISE 14.7, ModelSim
- **Pipeline design:** Hazard detection and forwarding, branch flush control, timing closure
- **Verification:** Custom testbenches, directed and pseudo-random stimulus, CDC debug, timing constraint analysis
- **Protocols on FPGA:** UDP/Ethernet stack (MAC/PHY/UDP wrappers), PCIe transaction layer verification, UART/USART modules
- **FPGA-specific optimization:** LUT/FF/BRAM resource trade-offs, clock domain crossing synchronization, clock divider generation

### GPU & CUDA

- CUDA kernel design and profiling (nvprof, occupancy analysis)
- Memory coalescing, shared-memory tiling, stream-based pipeline overlap
- Performance characterization and bottleneck-driven optimization
- OpenGL, VTK for visualization pipelines

### Medical Imaging

- 3D reconstruction from volumetric CT data
- Lung tumor segmentation and ROI extraction
- Surface mesh optimization and texel density control
- Clinical visualization workflows

### Tools & Languages

- C/C++, Python, MATLAB
- Verilog, VHDL
- Vivado, Xilinx ISE, ModelSim
- Wireshark, GitHub, VS Code

---

## Featured Projects

### Hardware Texel Density Balancer

GPU-accelerated pipeline for lung tumor 3D reconstruction with adaptive texel density balancing in diagnostically critical regions. Designed, implemented, and optimized end-to-end without collaboration. All CUDA knowledge entirely self-taught.

**Tech stack:** CUDA, C/C++, VTK, Python
**Outcome:** Runtime reduced from ~52 minutes to ~6 minutes (**8.7× speedup**); uniform texel density maintained on malignant boundaries under varying zoom and scale

**What drove the speedup:**
- Profiled sequential CPU pipeline to identify bottlenecks before writing any CUDA
- Batched all CT slice transfers into single GPU transfers, eliminating per-slice PCIe overhead
- Fused segmentation and reconstruction kernels, removing repeated kernel launch latency
- Restructured memory access for coalescing, reducing memory transactions up to 32× per warp
- Moved hot intermediate data from 600-cycle global memory into 4-cycle on-chip shared memory
- Introduced CUDA streams to overlap active compute with next-batch data transfer

---

### Pipelined MIPS Processor

32-bit MIPS processor in Verilog with full hazard handling (RAW/WAR), forwarding network, and branch flush control. Deployed on Nexys 3 (Spartan-6) with seven-segment ALU state display for real-time hardware debugging.

**Tech stack:** Verilog, Vivado/ISE, ModelSim, Spartan-6
**Key features:** Five-stage pipeline (IF/ID/EX/MEM/WB), timing closure, on-chip hardware validation

---

### FPGA Procedural Shader Pipeline (VGA)

Real-time GPU-inspired procedural shader in Verilog generating animated planetary shading and starfields at 640×480@60Hz without a framebuffer. Implemented fixed-point nonlinear lighting and CORDIC-based trigonometric modulation under FPGA resource constraints.

**Tech stack:** Verilog, Xilinx ISE, Spartan-6
**Key features:** CORDIC trig, fixed-point arithmetic, zero framebuffer architecture

---

### FPGA–PC Ethernet Communication (UDP Stack)

Full UDP/IP/Ethernet stack implemented in VHDL on Nexys 3 (Spartan-6). Built IP-wrapper, UDP-wrapper, and Ethernet-wrapper-with-preamble modules. Verified end-to-end payload integrity using Wireshark.

**Tech stack:** VHDL, Xilinx ISE, Wireshark
**Focus:** Low-latency exchange, MAC/PHY interface, FSM-based handshakes, resource utilization documentation

---

### PCIe Communication Verification (NECOP Internship)

Verified high-speed PCIe transaction layer behavior on Xilinx UltraScale+ using custom Verilog testbenches. Covered all four AXI lanes (RQ/RC/CQ/CC), DMA transfers, BAR access, reset sequencing, and CDC crossing analysis.

**Tech stack:** Verilog, Vivado, UltraScale+
**Focus:** Directed and pseudo-random stimulus, timing constraint collaboration, CDC debug

---

### Single and Multi-cycle MIPS Variants

Datapath and FSM-based control unit variants of MIPS. Compared throughput vs critical-path trade-offs across implementations. Verified in ModelSim and deployed on FPGA.

**Tech stack:** Verilog, ModelSim, Spartan-6

---

### Facial Recognition Lock (ESP32-CAM + OpenCV)

Embedded authentication pipeline on ESP32-CAM streaming MJPEG frames to OpenCV for face recognition. GPIO-controlled relay actuated lock on authorization. Event logging to SPIFFS flash for audit trail.

**Tech stack:** C++ (ESP32 Arduino), OpenCV, Python

---

### PC-to-PC IPv6 Communication

Configured IPv6 topology in Cisco Packet Tracer, replicated on hardware. Verified packets, latencies, NDP behavior, and addressing using Wireshark.

**Tech stack:** Cisco Packet Tracer, Wireshark

---

## Connect

- **LinkedIn:** [linkedin.com/in/dur-haider-a5bb1826a](https://linkedin.com/in/dur-haider-a5bb1826a)
- **Email:** durhaider2@gmail.com
- **Location:** Islamabad, Pakistan
