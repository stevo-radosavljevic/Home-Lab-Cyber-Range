## Lab Infrastructure & Hardware
To simulate a realistic enterprise environment, I utilize a hybrid hardware setup. This allows for the testing of modern security controls against legacy system vulnerabilities.

### Node 01: Core Virtualization & Research (Dell Powerhouse)
*   **Specifications:** 32GB RAM | 1TB NVMe SSD
*   **Primary Role:** Serves as the Type-2 Hypervisor host (VMware/VirtualBox).
*   **Lab Function:**
    *   Hosting a **Windows Server 2022 Domain Controller** (Active Directory Research).
    *   Running **Kali Linux** for offensive operations and vulnerability research.
    *   Simulating **Kubernetes clusters** and Dockerized environments to mirror my work in DevSecOps.

### Node 02: Legacy Target & Hardware Research (Toshiba Repurposed)
*   **Specifications:** Upgraded SSD/RAM (2011 Chassis)
*   **Primary Role:** Dedicated Physical Target / Linux Server.
*   **Lab Function:**
    *   **Legacy OS Simulation:** Used to host older, vulnerable operating systems to practice exploitation of unpatched vulnerabilities (CVE research).
    *   **Resource Optimization:** Rebuilt with an SSD and expanded RAM to serve as a dedicated **SIEM collector (Wazuh/ELK)** or a **Hardware Firewall (pfSense)** node.
    *   **Environmental Realism:** Represents the "Technical Debt" often found in IT/OT environments, allowing for realistic Incident Response drills.

## Why this setup?
In Cybersecurity, understanding the interaction between modern high-performance systems and older, legacy infrastructure is critical. This lab is designed to bridge that gap, focusing on **Lateral Movement** and **Protocol Analysis** between different hardware generations.
