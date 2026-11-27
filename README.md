# Cybersecurity & Digital Forensics Study Log

A running log of my cybersecurity learning journey, room notes, and progress milestones.

## Day 1 Takeaways (2026-11-26)

* **Security through obscurity:** Hiding a resource does not protect it once an attacker discovers its address[cite: 1].
* **Authorized ethical hacking & penetration testing:** Safely testing systems under established rules to uncover weaknesses and help defenders strengthen them[cite: 1, 2].
* **Defensive security:** Monitoring incoming alerts for early signs of an attack and neutralizing threats (such as blocking attacker IPs, slowing requests, or enabling protections) while keeping an open mindset about how attackers think[cite: 1].
* **Cybersecurity career paths:** Roles such as penetration testers and security analysts protect critical systems, work with stakeholders to review security, build security plans, and report on network security[cite: 2].

## Progress Log

| Date | Platform / Topic | Key Takeaway | Status |
| :--- | :--- | :--- | :--- |
| 2026-11-26 | TryHackMe — Intro, Defensive Security & CS Careers | Security through obscurity fails when found; defensive security spots and stops threats early; ethical hacking tests systems under clear rules[cite: 1, 2]. | Completed |

## Day 2 Takeaways — Computer Components & Boot Process (2026-11-28)

- **Motherboard:** Acts as the computer's skeleton and nervous system, housing connectors (CPU socket, RAM slots, expansion slots, and ports) so all components can connect and communicate.
  ![Motherboard Overview](assets/day02-02-motherboard-overview.png)
  ![Motherboard Role Quiz](assets/day02-01-motherboard-role-quiz.png)
- **CPU (Central Processing Unit):** The processor/brain that continuously executes instructions and performs calculations; modern CPUs use multiple cores for parallel processing and plug into the CPU socket.
  ![CPU Visual](assets/day02-04-cpu-visual.png)
  ![CPU Quiz](assets/day02-03-cpu-quiz.png)
- **RAM (Random Access Memory):** Short-term working memory that temporarily holds data the CPU needs fast access to while running; it is volatile (wiped on power loss) and uses modern standards like DDR5/DDR6.
  ![RAM Visual](assets/day02-06-ram-visual.png)
  ![RAM Quiz](assets/day02-05-ram-quiz.png)
- **Storage (SSD & HDD):** Long-term, non-volatile memory that keeps data even when powered off; **HDDs** rely on mechanical moving parts (large capacity at lower cost), whereas **SSDs** use flash memory chips with no moving parts (much faster speeds), connecting via SATA or PCI Express.
  ![Storage SSD vs HDD Visual](assets/day02-09-storage-ssd-hdd-visual.png)
  ![Storage SSD vs HDD Explanation](assets/day02-08-storage-ssd-hdd-text.png)
  ![Storage SSD vs HDD Quiz](assets/day02-07-storage-ssd-hdd-quiz.png)
- **Network Adapter:** Enables communication with other computers and networks via wired or wireless connections, either embedded on the motherboard or added as a PCI Express expansion card.
  ![Network Adapter Visual](assets/day02-11-network-adapter-visual.png)
  ![Network Adapter Quiz](assets/day02-10-network-adapter-quiz.png)
- **Input / Output (I/O) Devices:** Send data to and receive data from the system—inputs include keyboards, mice, microphones, and scanners; outputs include monitors, printers, and speakers—connected via USB, HDMI, and DisplayPort.
  ![Input/Output Devices Visual](assets/day02-13-io-devices-visual.png)
  ![Input/Output Devices Quiz](assets/day02-12-io-devices-quiz.png)
- **Power Supply Unit (PSU):** Supplies electrical power from an outlet to all system components through cables such as the main motherboard connector and Molex connectors; insufficient wattage causes system failure.
  ![Power Supply Unit Visual](assets/day02-15-psu-visual.png)
  ![Power Supply Unit Quiz](assets/day02-14-psu-quiz.png)
- **Graphics Card (GPU):** Processes visual information from the OS and programs and outputs it to a monitor via PCI Express slots.
  ![Graphics Card Visual](assets/day02-17-graphics-card-visual.png)
  ![Graphics Card Quiz](assets/day02-16-graphics-card-quiz.png)
- **Motherboard Slots & Ports (Rear I/O, SATA, PCIe):**
  - **Rear I/O ports:** External connectors on the backplate for keyboards, mice, monitors, USB devices, networking, and audio.
    ![Rear I/O Ports](assets/day02-18-rear-io-ports.png)
  - **SATA ports:** Thin L-shaped connectors for 2.5" and 3.5" SSDs and HDDs via SATA cables.
    ![SATA Ports](assets/day02-19-sata-ports.png)
  - **PCI Express x16 slots:** Long reinforced high-bandwidth slots typically used for GPUs or network/expansion cards.
    ![PCIe x16 Slot Highlight A](assets/day02-20-pcie-x16-slot-a.png)
    ![PCIe x16 Slot Highlight B](assets/day02-21-pcie-x16-slot-b.png)
    ![PCIe x16 Slot Highlight C](assets/day02-23-pcie-x16-slot-c.png)
  - **PCI Express x1 / x4 slots:** Shorter slots used for network cards, capture cards, and other expansion cards.
    ![PCIe x1 / x4 Slots](assets/day02-22-pcie-x1-x4-slots.png)
- **System Boot Process (5 Steps):**
  1. **Press Power Button:** Sends a signal to the PSU to allow power to flow.
  2. **Firmware Starts:** **UEFI** (which has largely replaced legacy **BIOS**) initializes core hardware components so they can start up.
  3. **Power-On Self Test (POST):** Firmware checks that required components are present, configured properly, and working (raising alarm signals if something fails).
  4. **Select Boot Device:** UEFI checks its prioritized boot order list to find where the bootup routine for the OS is located.
  5. **Initiate Bootloader:** Starts the bootloader on the selected boot device to transfer the OS into RAM and hand control of system components over to the OS.
  ![System Boot Flow Diagram](assets/day02-24-boot-flow-diagram.png)
  ![Boot Steps 1 to 5](assets/day02-25-boot-steps-1-to-5.png)
  ![Boot Exercise Prompt](assets/day02-26-boot-exercise-prompt.png)

## Progress Log

| Date | Platform / Topic | Key Takeaway | Status |
| :--- | :--- | :--- | :--- |
| 2026-11-26 | TryHackMe — Intro, Defensive Security & CS Careers | Security through obscurity fails when found; defensive security spots and stops threats early; ethical hacking tests systems under clear rules. | Completed |
| 2026-11-28 | TryHackMe — Computer Components & Boot Process | Covered core hardware (CPU, RAM, SSD/HDD, GPU, PSU, I/O, NIC), motherboard slots/ports (PCIe, SATA, Rear I/O), and the 5-step boot sequence. | Completed |
