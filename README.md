<p align="center">
  <h1 align="center">Edge Dominant Hierarchical Intelligence (EDHI)</h1>
  <p align="center">
    Real-Time • Edge-Native • Hierarchical AI Architecture for Autonomous Systems
  </p>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Architecture-Edge--Native-blue">
  <img src="https://img.shields.io/badge/Focus-Humanoid%20Robotics-black">
  <img src="https://img.shields.io/badge/Latency-Real--Time-green">
  <img src="https://img.shields.io/badge/License-MIT-orange">
</p>

---

<h2>Overview</h2>

<p>
Edge Dominant Hierarchical Intelligence (EDHI) is an open-source framework engineered for
<strong>low-latency, energy-efficient, fully autonomous AI systems</strong> operating entirely at the edge.
</p>

<p>
EDHI implements a tightly coupled intelligence stack across:
</p>

<ul>
  <li><strong>Perception</strong> — sensor fusion, semantic understanding</li>
  <li><strong>Planning</strong> — decision-making, trajectory generation</li>
  <li><strong>Control</strong> — real-time actuation and feedback stabilization</li>
</ul>

<p>
Unlike conventional architectures, EDHI enforces <strong>deterministic execution, local intelligence, and cross-layer coupling</strong>.
</p>

---

<h2>Core Architecture</h2>

<pre>
+-----------------------------+
|        Planning Layer       |
|  Task reasoning, policies   |
+-------------+---------------+
              ↓
+-----------------------------+
|      Perception Layer       |
|  Sensor fusion, semantics   |
+-------------+---------------+
              ↓
+-----------------------------+
|       Control Layer         |
|  Actuation, feedback loops  |
+-----------------------------+
</pre>

<table>
<tr><th>Layer</th><th>Frequency</th><th>Responsibility</th></tr>
<tr><td>Perception</td><td>10–60 Hz</td><td>Scene understanding, state estimation</td></tr>
<tr><td>Planning</td><td>1–10 Hz</td><td>Task decisions, trajectory generation</td></tr>
<tr><td>Control</td><td>100–1000 Hz</td><td>Motor commands, stabilization</td></tr>
</table>

---

<h2>System Flow</h2>

<pre>
Sensors → Perception → World Model → Planner → Controller → Actuators
                ↑            ↓             ↑
                +------------+-------------+
                   Feedback and State Sync
</pre>

---

<h2>Design Principles</h2>

<ul>
<li><strong>Edge Dominance</strong> — all intelligence loops run locally</li>
<li><strong>Real-Time Determinism</strong> — bounded latency execution</li>
<li><strong>Hardware Awareness</strong> — optimized for CPU, GPU, NPU</li>
<li><strong>Hierarchical Decomposition</strong> — multi-layer intelligence</li>
<li><strong>Cross-Layer Feedback</strong> — adaptive closed-loop system</li>
</ul>

---

<h2>Module Breakdown</h2>

<strong>Perception Engine</strong>
<ul>
<li>Multi-modal fusion (RGB, Depth, IMU, LiDAR)</li>
<li>State estimation (EKF, factor graphs)</li>
<li>Semantic understanding</li>
</ul>

<strong>World Model</strong>
<ul>
<li>Dynamic environment representation</li>
<li>Spatial + semantic fusion</li>
</ul>

<strong>Planning Engine</strong>
<ul>
<li>Hierarchical planning (task + motion)</li>
<li>Policy-based decision systems</li>
</ul>

<strong>Control Engine</strong>
<ul>
<li>Whole-body control (WBC)</li>
<li>Model Predictive Control (MPC)</li>
<li>Real-time stabilization</li>
</ul>

<strong>Runtime Orchestrator</strong>
<ul>
<li>Task scheduling</li>
<li>Low-latency IPC</li>
<li>Resource allocation</li>
</ul>

---

<h2>Technology Stack</h2>

<table>
<tr><th>Component</th><th>Support</th></tr>
<tr><td>Languages</td><td>C++, Python</td></tr>
<tr><td>Middleware</td><td>ROS2, custom runtime</td></tr>
<tr><td>AI Frameworks</td><td>PyTorch, TensorFlow Lite, ONNX</td></tr>
<tr><td>Acceleration</td><td>CUDA, TensorRT, OpenVINO</td></tr>
<tr><td>OS</td><td>Linux, PREEMPT-RT</td></tr>
</table>

---

<h2>Installation</h2>

<pre>
git clone https://github.com/your-org/edhi.git
cd edhi

./scripts/setup.sh

mkdir build && cd build
cmake ..
make -j$(nproc)
</pre>

---

<h2>Quick Start</h2>

<pre>
./bin/perception_node
./bin/planner_node
./bin/controller_node

./scripts/run_full_stack.sh
</pre>

---

<h2>Performance Targets</h2>

<table>
<tr><th>Metric</th><th>Target</th></tr>
<tr><td>Latency</td><td>&lt; 10–20 ms</td></tr>
<tr><td>Control Frequency</td><td>Up to 1 kHz</td></tr>
<tr><td>Power</td><td>&lt; 50W</td></tr>
<tr><td>Reliability</td><td>Fault-tolerant autonomy</td></tr>
</table>

---

<h2>Roadmap</h2>

<ul>
<li>Unified world model API</li>
<li>Multi-robot coordination</li>
<li>Learning-based control</li>
<li>Digital twin simulation</li>
<li>Safety verification</li>
</ul>

---

<h2>Contribution</h2>

<ol>
<li>Fork repository</li>
<li>Create feature branch</li>
<li>Commit with documentation</li>
<li>Submit pull request</li>
<li>Pass all tests</li>
</ol>

---

<h2>License</h2>

MIT License

---

<h2>Vision</h2>

<p>
EDHI establishes a paradigm where intelligence is:
</p>

<ul>
<li>Local (not cloud-dependent)</li>
<li>Hierarchical (not monolithic)</li>
<li>Deterministic (not best-effort)</li>
</ul>

<p align="center">
<strong>Goal: General-purpose autonomous machines operating reliably in real-world environments.</strong>
</p>
