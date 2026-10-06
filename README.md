# IT VirtualBox Lab Infrastructure

A structured, hands-on virtualized laboratory environment designed for network isolation, systems administration testing, and infrastructure experiments using VirtualBox.

---

## 📐 Design & Architecture Decisions

### Why a Virtualized Lab?
Virtualization allows safe experimentation with operating systems, network topologies, and security configurations without exposing the host system or local home network to risk.

### Why VirtualBox?
- **Accessibility:** Free, open-source, and cross-platform hypervisor suitable for rapid local prototyping.
- **Networking Flexibility:** Supports internal networks, NAT Networks, Host-Only adapters, and bridged interfaces to simulate real-world enterprise topographies.

### Key Architecture Choices & Troubleshooting
1. **Graphics Controller Adjustment (VBoxVGA → VMSVGA):** Resolved boot black-screen issues by aligning display drivers with VirtualBox 7.0 requirements.
2. **Network Diagnostics:** Manual installation of `net-tools` (`ifconfig`) and Guest Additions to ensure dynamic display scaling and proper adapter connectivity.
3. **Resource Optimization:** Configured optimal RAM and CPU allocation for Ubuntu 22.04 LTS to run smoothly alongside host workloads.

---

## 🛠 Lab Capabilities & Demonstrated Skills

- **Virtualization Deployment:** OS installation, ISO configuration, and guest resource management.
- **Systems Administration:** Package management, Linux command-line utilities (`htop`, `df`, `free`), and user account management (`adduser`, `usermod`).
- **Networking & Diagnostics:** Verification of connectivity and interfaces using `ip addr`, `ping`, and network adapter configuration.
- **Technical Documentation:** Comprehensive step-by-step documentation with visual evidence in `/documentacion/`.

---

## 🚀 Quick Setup & Usage

### Prerequisites
- [Oracle VirtualBox 7.0+](https://www.virtualbox.org/) installed.
- Ubuntu 22.04 LTS ISO image.

### Getting Started
1. Create a new VM in VirtualBox allocating at least 2 CPUs and 2048 MB RAM.
2. Set display controller to **VMSVGA** and attach the Ubuntu 22.04 ISO.
3. Install **VirtualBox Guest Additions** post-installation for full display integration.
4. Detailed documentation and screenshots are available in the [`/documentacion`](./documentacion/) directory.
