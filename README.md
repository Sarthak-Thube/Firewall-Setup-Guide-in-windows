# Task 4: Setup and Use a Firewall on Windows

## Objective
The objective of this task is to configure and test basic firewall rules to allow or block network traffic. This guide provides instructions for both Windows and Linux environments.

## Tools
* **Windows**: Windows Defender Firewall with Advanced Security
---

## Guide: Windows Firewall

### 1. Open the Firewall Configuration Tool
* Press the **Windows key**, type "Windows Defender Firewall with Advanced Security," and press **Enter**.

### 2. List Current Rules
* Navigate to **"Inbound Rules"** to view all existing rules.

### 3. Add a Rule to Block Inbound Traffic
* Click **"New Rule..."** in the right pane.
* Select **"Port"** and click **"Next"**.
* Choose **"TCP"** and enter port **`23`** (for Telnet).
* Select **"Block the connection"**.
* Name the rule **"Block Telnet"**.

### 4. Test the Rule
* Attempt to connect to your machine on port `23` using a Telnet client from another computer on the network. The connection should fail.

### 5. Remove the Test Rule
* Find the **"Block Telnet"** rule, right-click, and select **"Delete"**.

---
## Summary: How a Firewall Filters Traffic
A firewall acts as a digital barrier, inspecting incoming and outgoing network traffic against a predefined set of security rules. It determines whether to **allow**, **deny**, or **drop** packets based on criteria like source/destination IP addresses, port numbers, and protocol types. This filtering process is essential for preventing unauthorized access and protecting a network from cyber threats.
