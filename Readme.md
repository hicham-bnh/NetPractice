*This project has been created as part of the 42 curriculum by mobenhab.*

# NetPractice

## Description

NetPractice is a practical networking project from the 42 curriculum. The goal is to configure small-scale simulated networks by solving 10 progressively challenging exercises. Each level presents a non-functioning network diagram that must be repaired by correctly setting IP addresses, subnet masks, and default gateways until all devices can communicate as intended.

Through this project, you will develop a solid understanding of how TCP/IP addressing works, how routers and switches interconnect devices, and how traffic is routed across different network segments.

## Instructions

### Running the training interface

1. Download and extract the project files provided on the project page.
2. Navigate into the extracted folder and run the launch script:

```bash
  ./run.sh
```

This will start a local web server and open the training interface in your browser automatically.

> **Alternative (if `run.sh` doesn't work):** Run the server manually with Python, then open `http://localhost:49242` in your browser:


### Using the interface

- Enter your **42 login** in the provided field before starting — this is required for the configuration to be personalized.
- Use the **"evaluation"** tab to generate a random configuration suitable for peer-evaluations.
- For each level:
  - Modify the unshaded fields until the network is correctly configured.
  - Click **[Check again]** to verify your configuration.
  - Once a level is validated, click **[Get my config]** to export your configuration file **before** moving to the next level.

### Exporting and submitting configurations

- Export one configuration file per level using the **[Get my config]** button.
- Place all **10 exported configuration files** at the **root of your Git repository**.
- Submit by pushing to your repository as usual. Only files present in the repository will be evaluated.

### Peer-evaluation

During the defense, you will be asked to successfully complete **3 random levels** within a limited time. No external tools are allowed — a basic calculator (e.g., `bc`) is the only exception.

## Resources

### Networking concepts studied

- **TCP/IP addressing** — understanding IPv4 addresses, their structure, and how they are assigned to devices
- **Subnet masks** — determining network and host portions of an address, calculating valid address ranges
- **CIDR notation** — expressing subnet masks in prefix length format (e.g., `/24`)
- **Default gateways** — the role of a gateway in routing traffic outside a local network
- **Routers** — how they forward packets between different networks using routing tables
- **Switches** — how they operate at Layer 2 to connect devices within the same network
- **OSI model** — understanding the layers (particularly Layer 2 and Layer 3) to reason about network behavior
- **IP routing** — how packets travel from source to destination across multiple hops

### Useful references

- [Cisco Networking Basics – TCP/IP](https://www.cisco.com/c/en/us/solutions/small-business/resource-center/networking/networking-basics.html)
- [Subnet Calculator](https://www.subnet-calculator.com/)
- [Subnetting Practice – SubnettingPractice.com](https://www.subnettingpractice.com/)
- [Computer Networking: A Top-Down Approach – Kurose & Ross](https://gaia.cs.umass.edu/kurose_ross/index.php)
- [RFC 791 – Internet Protocol](https://www.rfc-editor.org/rfc/rfc791)
- [Wikipedia – Classless Inter-Domain Routing (CIDR)](https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing)

### AI usage

AI was used during this project for the following tasks:

- **Concept clarification**: asking for plain-language explanations of subnet masks, CIDR notation, and routing table logic when documentation felt unclear.
- **Verification**: double-checking manual subnet calculations (network address, broadcast address, valid host range) to catch arithmetic errors.
- **README drafting**: generating an initial structure for this README, which was then reviewed, adjusted, and completed manually.

All AI-generated content was reviewed and validated before use. Networking concepts were verified against official documentation and cross-checked with peers.