# Hi, I'm Dur E Haider 👋

Final-year Computer Engineering student at NUST CEME, specializing in GPU architecture, hardware acceleration, and real-time systems optimization.

## 🔬 Current Research

I'm working on **GPU-accelerated medical imaging pipelines** for 3D reconstruction and segmentation. My research focuses on:

- **CUDA kernel optimization**: Achieved ~4× speedup (30s → 7s) through kernel fusion and batched memory transfers
- **Texel density balancing**: Stabilizing texture resolution in diagnostically critical regions (tumor boundaries)
- **Memory hierarchy optimization**: Coalesced memory patterns, shared-memory tiling, and stream-based compute/I/O overlap
- **GPU–FPGA co-design**: Exploring hybrid architectures for real-time medical visualization pipelines

## 💡 Technical Focus

**GPU & Graphics:**
- CUDA (kernel design, occupancy optimization, memory coalescing)
- OpenGL, VTK
- Real-time rendering and visualization
- Performance profiling (timers, occupancy analysis)

**Hardware Design:**
- Verilog/VHDL (Vivado, Xilinx ISE)
- FPGA implementation (Spartan-6)
- Pipeline design and hazard mitigation
- Design verification and testbench development

**Medical Imaging:**
- 3D reconstruction from volumetric data
- Segmentation (lung tumor ROIs)
- Surface mesh optimization
- Clinical visualization workflows

**Tools & Languages:**
- C/C++, Python, MATLAB
- Unity, Blender (asset pipeline)
- GitHub, VS Code, ModelSim
- Wireshark (network validation)

## 🎯 What I'm Exploring

Making **high-performance 3D reconstruction** accessible through:
- GPU resource management and runtime scheduling
- Real-time latency requirements for interactive visualization
- Balancing throughput, latency, and resource utilization constraints
- Hardware-software co-optimization (GPU–FPGA partitioning)

My final year project demonstrates stable medical visualization with optimized texel density distribution and ~4× runtime improvement through CUDA acceleration.

## 🚀 Featured Projects

### Hardware Texel Density Balancer (Final Year Project)
GPU-accelerated pipeline for lung tumor 3D reconstruction with adaptive texel density balancing in critical regions. Targets consistent perceptual quality under varying zoom/scale while respecting performance budgets.

**Tech Stack:** CUDA, C/C++, VTK, Blender  
**Outcome:** Runtime reduced from ~30s to ~7s; uniform texel density on malignant boundaries

### Pipelined MIPS Processor
32-bit MIPS implementation in Verilog with full hazard handling (RAW/WAR), forwarding network, and branch flush control. Deployed on Nexys 3 (Spartan-6) with seven-segment ALU state display.

**Tech Stack:** Verilog, Vivado/ISE, ModelSim  
**Key Features:** Five-stage pipeline (IF/ID/EX/MEM/WB), timing closure optimization

### FPGA-PC Communication (UDP Stack)
Real-time Ethernet communication between PC and Nexys 3 FPGA. Implemented UDP handshake and transmission routines with Wireshark validation.

**Tech Stack:** VHDL, Xilinx ISE, Wireshark  
**Focus:** Low-latency exchange, MAC/PHY interface, FSM-based handshakes

## 📚 Currently

- Completing undergraduate thesis on **GPU-accelerated medical visualization**
- Preparing applications for **Fall 2026 Master's programs** in GPU systems, real-time graphics, and high-performance computing
- Exploring GPU scheduling frameworks and resource management for multi-tasking environments

## 📫 Connect

- **LinkedIn:** [linkedin.com/in/dur-haider-a5bb1826a](https://linkedin.com/in/dur-haider-a5bb1826a)
- **Email:** durhaider2@gmail.com
- **Location:** Islamabad, Pakistan

---

*Interested in GPU architecture, real-time systems, FPGA co-design, and hardware-accelerated medical imaging.*
