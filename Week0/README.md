# 🚀 Week 0: RISC‑V SoC Tapeout Program — Foundation & Tool Setup

<div align="center">

![VLSI](https://img.shields.io/badge/VLSI-System%20Design-blue?style=for-the-badge\&logo=chip)
![Week](https://img.shields.io/badge/Week-0-orange?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-success?style=for-the-badge)

</div>

Welcome to my project repository for the **RISC‑V SoC Tapeout Program 2025**, a flagship initiative by **IIT Gandhinagar** and **VLSI System Design (VSD)**. I'm currently pursuing my **MTech** and this program is my stepping stone toward becoming **an industry-ready VLSI engineer**.

---

## 🎯 **Week 0 Objective**

Establish a robust, reproducible VLSI design environment with all the necessary open-source tools to perform RTL design, synthesis, simulation, layout, and tapeout.

---

## 💻 **System Configuration**

To ensure tool compatibility and performance, I provisioned a virtual machine with the following specs:

<div align="center">

| **Component** | **Details**      |
| ------------- | ---------------- |
| OS            | Ubuntu 20.04 LTS |
| RAM           | 6 GB             |
| Storage       | 50 GB            |
| CPUs          | 4 vCPUs          |

</div>

> ✅ This environment will support the entire ASIC design flow using Sky130 PDK and tools like Yosys, Iverilog, Magic, and more.

---

## ⚙️ **Installed Tools**

The following open-source tools were installed and verified successfully:

```bash
🧠 Yosys → 📟 Iverilog → 📊 GTKWave → ⚡ Ngspice → 🎨 Magic VLSI
```

Each tool serves a specific stage in the digital/analog IC design process. Below is a summary of installations with usage and verification steps.

---

### 🧠 Yosys – RTL Synthesis

<details>
<summary><b>🔍 About:</b> Converts RTL (Verilog) into gate-level netlists.</summary>

Yosys is a powerful synthesis tool widely used for generating and optimizing gate-level representations from Verilog designs.

</details>

```bash
# Clone and install Yosys
git clone https://github.com/YosysHQ/yosys.git
cd yosys
make
sudo make install
```

✅ **Installed Successfully!**

---

### 📟 Icarus Verilog (Iverilog) – Verilog Simulator

<details>
<summary><b>🔍 About:</b> Performs functional simulation of Verilog code.</summary>

Useful for verifying RTL before synthesis using testbenches and waveform analysis.

</details>

```bash
sudo apt-get install iverilog
```

✅ **Installed Successfully!**

---

### 📊 GTKWave – Waveform Viewer

<details>
<summary><b>🔍 About:</b> Visualizes waveform outputs from simulation (VCD format).</summary>
</details>

```bash
sudo apt install gtkwave
```

✅ **Installed Successfully!**

---

### ⚡ Ngspice – Circuit Simulator

<details>
<summary><b>🔍 About:</b> Simulates analog/mixed-signal designs at the transistor level.</summary>
</details>

```bash
sudo apt install ngspice
```

✅ **Installed Successfully!**

---

### 🎨 Magic VLSI – Layout Tool

<details>
<summary><b>🔍 About:</b> Used for IC layout design and DRC checks.</summary>
</details>

```bash
# Install dependencies
sudo apt-get install m4 tcsh csh libx11-dev tcl-dev tk-dev \
libcairo2-dev mesa-common-dev libglu1-mesa-dev libncurses-dev

# Clone and build Magic
git clone https://github.com/RTimothyEdwards/magic.git
cd magic
./configure
make
sudo make install
```

✅ **Installed Successfully!**

---

## ✅ Summary Table

| Tool       | Purpose               | Status      |
| ---------- | --------------------- | ----------- |
| Yosys      | RTL synthesis         | ✅ Installed |
| Iverilog   | Functional simulation | ✅ Installed |
| GTKWave    | Waveform viewing      | ✅ Installed |
| Ngspice    | Circuit simulation    | ✅ Installed |
| Magic VLSI | Layout and DRC        | ✅ Installed |

> 🛠️ With this setup complete, I'm ready to dive into RTL design and move toward full SoC tapeout using Sky130 PDK.

---

## 🙌 Credits

* 🏫 **IIT Gandhinagar** — Academic Partner
* 🛠️ **VLSI System Design (VSD)** — Program Organizer
* 🌐 **SkyWater & Google** — Sky130 Open PDK
* 📢 **Community** — Fellow learners & mentors

---

## 📬 Connect with Me

* 📧 Email: \[[pranavindurkar111@gmail.com](mailto:pranavindurkar111@gmail.com)]
* 💼 LinkedIn: \www.linkedin.com/in/pranav-indurkar213

---

<div align="center">

**🔧 System Ready. Time to build silicon. 🧠⚙️🚀**
**From RTL → GDSII → Tapeout — India’s Chip Design Revolution 🇮🇳**

</div>

---

Let me know:

* If you want me to generate image placeholders (`assets/`) for verification screenshots
* Want GitHub badges (stars, forks, followers) added
* Need separate `INSTALL.md` or `tool_setup.sh` script

I'll help you make this repo truly standout!
