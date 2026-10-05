*This project has been created as part of the 42 curriculum by mrojouan.*

# NetPractice

## Description

NetPractice is a pedagogical project from the 42 common core focused on
computer networking fundamentals. The goal is to configure a set of small,
simulated networks made up of hosts, switches, and routers so that all
machines can communicate correctly with one another.

Each of the 10 levels presents a network topology with missing or incorrect
parameters (IP addresses, subnet masks, gateways, routing tables, etc.).
The objective is to fill in the blanks so that every host in the topology
can successfully reach every other host, without any conflicts or unused
address ranges. The project is entirely done through a web-based training
interface — no code needs to be written — but it requires a solid
understanding of IP addressing and routing logic.

## Instructions

### Running the training interface

The training interface is provided as a set of static web files. To launch
it locally, run the provided script from the root of the repository:

```bash
./run.sh
```

This starts a local web server and opens the NetPractice interface in your
default browser (usually at `http://localhost:8080` — check the script
output for the exact address/port).

If `run.sh` is not executable, make it so first:

```bash
chmod +x run.sh
```

### Working through a level

1. Select a level (1 to 10) from the interface.
2. Read the topology: hosts, switches, routers, and links.
3. Fill in the missing fields (IP address, subnet mask, network/broadcast
   address, gateway, routing table entries, etc.).
4. Use the "Check" / "Test" button in the interface to validate connectivity
   between all hosts.
5. Once a level is fully validated (all connections green), export the
   configuration.

### Exporting configurations

Each validated level can be exported as a configuration file directly from
the interface (usually via an "Export" or "Save" button). The exported file
must be renamed/placed according to the submission requirements below.

### Submission requirements

- **10 exported configuration files (one per level) must be placed at the
  root of the repository.**
- Each file should correspond to exactly one level and be clearly
  identifiable (e.g. `level1.txt`, `level2.txt`, ... `level10.txt`).
- Make sure every level is fully validated (100% correct) before exporting,
  since partial/incorrect configurations will not be accepted.

## Resources

### Networking concepts studied

- TCP/IP addressing (IPv4)
- Subnet masks and CIDR notation
- Network and broadcast addresses
- Subnetting and address range calculation
- Default gateways
- Routers and switches, and their role in a network
- Static routing tables
- OSI model layers (in particular Layer 2 - Data Link and Layer 3 - Network)
- Broadcast domains vs collision domains

### Documentation / articles / tutorials

- [Subnetting made easy - Cisco](https://www.cisco.com/)
- [IPv4 - Wikipedia](https://en.wikipedia.org/wiki/IPv4)
- [Subnet Calculator](https://www.subnet-calculator.com/)
- [OSI Model explained - Cloudflare Learning Center](https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/)
- 42 NetPractice subject PDF (provided by the school)

### AI usage

AI (ChatGPT / Claude) was used during this project for the following tasks:

- Clarifying theoretical concepts (e.g. how subnet masks affect broadcast
  domains, how routing tables are used to forward packets between subnets).
- Proofreading and formatting this README.md file.
- Generating example subnetting exercises to practice outside of the
  official interface.

No AI tool was used to solve the actual levels of the training interface;
all configurations were worked out manually to ensure the networking
concepts were properly understood.