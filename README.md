# Hi, I'm Wiesmes! 👋

I'm an Electrical Engineering student at Lehigh University working at the intersection of **robotics, machine learning, and accelerated computing** — building systems where software has to run fast on real hardware.

I develop software for an autonomous underwater vehicle competing in RoboSub, research FPGA and GPU acceleration for real-time ML inference, and build simulation and digital twin tooling for computational modeling research. I'm a Machine Learning Fellow with Break Through Tech AI.

Currently seeking internship opportunities in **robotics, autonomous systems, embedded software, and accelerated computing**.

## 📫 Connect With Me

- LinkedIn: [linkedin.com/in/wiesmes](https://www.linkedin.com/in/wiesmes/)
- Email: <wwa228@lehigh.edu>

## 🎓 Education

**Lehigh University** — Bethlehem, PA
Bachelor of Science in Electrical Engineering | Expected May 2028
GPA: 3.91

**Relevant Coursework:**

- Computer Architecture
- Digital Systems
- Signals & Systems
- Probability & Statistics
- Linear Algebra
- Engineering Computing Methods (Python)
- Object-Oriented Programming (Java)
- Electronic Circuits
- Semiconductor Devices
- ElectroMagnetism
- Robotics *(Teaching Assistant)*

## 💼 Experience

### 🌊 Lehigh Underwater Robotics (RoboSub)
**Fall 2025 – Present**

**Software**
- Develop the ROS 2 perception and navigation stack for an autonomous underwater vehicle on Ubuntu Linux and an NVIDIA Jetson Nano.
- Implemented map-free gap-follow navigation from Intel RealSense RGB-D depth and AprilTag detection; the vehicle holds heading through gates without a global map.
- Set up a simulation-first validation workflow so changes are tested before scarce pool time.

**Hardware**
- Integrated and tested the AUV's power, sensing, compute, and actuation subsystems on the bench and in the pool.
- Isolated power-delivery, wiring, sensor, sonar, thruster, and ESC faults with an oscilloscope and multimeter.

---

### 🏎️ Teaching Assistant — ECE Autonomous Systems Laboratory (E116), Lehigh University

**Aug 2026 – Present**

- Support 80+ students across 16 teams building Linux/ROS 2 autonomous vehicles; cover PWM calibration, stereo vision, gap-follow navigation, and race-day scoring.
- Diagnose hardware and software faults on live platforms and separate wiring, calibration, and software root causes.

---

### ⚡ Undergraduate Researcher, High-Performance Systems, Lehigh University · 
**Feb 2026 to present**

- Integrated a Vitis HLS kernel into a Zynq-7020 system over AXI4, packaged it as IP in a Vivado block design, and generated a bitstream that met timing (WNS +1.314 ns).
- Brought up the Arty Z7-20: bitstream over JTAG, bare-metal Vitis platform, ARM-side C driver that verifies all 256 results over UART.
- Built a scripted HLS flow (Tcl, Python, Makefiles) that logs latency and resource metrics per kernel variant.
- Hand-optimized a 32x32 int16 GEMM to II=1 (165,953 to 1,032 cycles); the baseline for research on LLM-guided HLS optimization.

---

### 🤖 Machine Learning Fellow — Break Through Tech AI (Cornell Tech)

**Jun 2026 – Present**

**AI Studio capstone with Automation Anywhere (Fall 2026)**
- Fine-tuned SmolLM2-360M-Instruct and Qwen2.5-1.5B-Instruct with LoRA/QLoRA (PyTorch, Hugging Face PEFT) on 26,900 customer-support tickets for theme labeling, with an LLM as the teacher model.
- Ran EDA and evaluation: removed 918 duplicate rows, scored outputs with an LLM judge, and traced a 0/5 verbatim-copying result to model capacity (Qwen baseline 3.68/5 vs. fine-tuned 3.75/5).

**Summer ML foundations**
- Trained a feedforward neural network in Keras/TensorFlow and benchmarked it against a tuned logistic regression baseline on an imbalanced binary classification task (84.6% accuracy, 0.680 F1).
- Built end-to-end Scikit-learn pipelines with imputation, one-hot encoding, and GridSearchCV hyperparameter search.
---

### 🔬 Research Assistant — Computational Modeling & ML Systems, Lehigh University

**Jan 2025 – Jan 2026**

- Built a Python/Tkinter digital twin interface unifying simulation, control, and model analysis, with asynchronous subprocess and multithreaded execution for non-blocking monitoring.
- Ported a NumPy physics-simulation and optimization pipeline to JAX; runtime fell from 8 hours to under 1 hour per run.
- Integrated ML-based parameter estimation into the simulation loop.

## 🛠️ Technical Skills

**Languages:** C, C++, Python, SystemVerilog, Java, MATLAB, Tcl

**FPGA & Digital Design:** Vivado, Vitis HLS, Vitis, Zynq-7020, AXI4, Icarus Verilog, GTKWave, Yosys, FSM design, timing closure

**Embedded & Hardware:** Raspberry Pi Pico (RP2040), MSP430, bare-metal ARM (Cortex-A9), PWM, ADC, JTAG, UART, Multisim, PSpice, SolidWorks

**Bench & Test:** Oscilloscopes, DMMs, function generators, soldering, board bring-up, fault isolation

**Robotics & Perception:** ROS 2, NVIDIA Jetson Nano, Intel RealSense RGB-D, AprilTag, gap-follow navigation

**Machine Learning:** PyTorch, Hugging Face PEFT (LoRA/QLoRA), TensorFlow/Keras, Scikit-learn, JAX

**Build Flow & Tools:** Linux, Git, Makefiles, batch synthesis scripting, report parsing, NumPy, Pandas, Matplotlib

## 📂 Featured Projects

### ⚡ hls-llm-study — HLS Accelerator and LLM-Guided Optimization

Vitis HLS kernels on a Zynq-7020 with a scripted synthesis flow (Tcl, Python, Makefiles) that logs latency and resource metrics per variant. A vecadd accelerator runs on the Arty Z7-20 with a bare-metal C driver; a hand-optimized 32×32 GEMM reaches II=1 (165,953 to 1,032 cycles) as the baseline for testing whether an LLM can optimize kernels from synthesis feedback.

**Technologies:** Vitis HLS, Vivado, C/C++, Python, Tcl, Zynq-7020
🔗 github.com/wiesmes/hls-llm-study

---

### 🌊 RoboSub Autonomy Stack

ROS 2 perception and navigation stack for an autonomous underwater vehicle — map-free gap-follow navigation using RGB-D depth and AprilTag detection, running on an NVIDIA Jetson Nano.

**Technologies:** ROS 2, Python, Ubuntu Linux, Jetson Nano, Intel RealSense
🔗 github.com/wiesmes/Underwater-robotics-autonomy

---

### 🎭 Theater Lighting, Visualization & Spotlight Controller

Seven-state synchronous Moore FSM in SystemVerilog controlling house lighting, a visualization display, and a servo spotlight with performer tracking. Hand-derived through Karnaugh map minimization and verified to a synthesized netlist — exactly three flip-flops, no inferred latches.

**Technologies:** SystemVerilog, Icarus Verilog, GTKWave, Yosys
🔗 github.com/wiesmes/theater-lighting-fsm

---

### 🔧 SystemVerilog RTL Design Portfolio

17 RTL modules spanning combinational and sequential logic, each with a directed testbench simulated in Icarus Verilog, debugged in GTKWave, and synthesized with Yosys.

**Technologies:** SystemVerilog, Icarus Verilog, GTKWave, Yosys
🔗 github.com/wiesmes/Systemverilog-digital-design

---

### 🌡️ Temperature-Controlled Fan System

Closed-loop thermal control on a Raspberry Pi Pico using thermistor ADC sensing and PWM fan drive through an N-channel MOSFET. Holds 29.4–30.8 °C around a 30 °C setpoint with 14-second response.

**Technologies:** Raspberry Pi Pico, Embedded C, PWM, ADC, SolidWorks
🔗 github.com/wiesmes/temperature-fan-controller

---

### 🔥 Industrial Drying Oven Digital Twin

Digital twin simulation platform for modeling industrial drying processes using physics-based simulation, machine learning optimization, and interactive visualization.

**Technologies:** Python, JAX, Tkinter, Matplotlib
🔗 github.com/wiesmes/Industrial-drying-oven-digital-twin

---

### 📊 Census Income Classification

Comparing a tuned logistic regression baseline against a Keras feedforward neural network on imbalanced binary classification, with leakage-safe cross-validated preprocessing.

**Technologies:** Python, Scikit-learn, TensorFlow/Keras

---

### 🔎 HawkSearch — Lehigh Agentathon (Best Value Award, April 2026)

An AI agent workflow that retrieves, analyzes, and ranks Lehigh research profiles using large language models.

**Technologies:** Python, Claude API, AI Agents

---

### 📄 SpendLens — Multimodal Document Intelligence Pipeline

A multimodal AI pipeline that extracts structured information from receipts and documents using vision-language models and automated validation workflows.

**Technologies:** Python, OpenAI API, Pandas, JSON

---

### 🏠 Smart Home Embedded System

A real-time IoT safety monitoring system integrating sensors, microcontroller programming, cloud telemetry, and data visualization.

**Technologies:** MSM430, Embedded C, ThingSpeak, C#

## ⚡ Fun Fact

⚽ I love watching soccer, but let's just say I'm a much better fan than player.
