INC-001 — Internet Connectivity Issue

Project: Caponi IT Lab
Category: Network Troubleshooting
Priority: Medium
Status: Open — Investigation in progress
Environment: Windows 11
Case type: Lab simulation

1. User Report

A user reports that their Windows 11 computer cannot access the internet.

The user can access the desktop and open applications, but websites do not load in the browser.

2. Initial Assessment

The objective is to identify whether the problem is related to:

* The physical or wireless network connection.
* IP address configuration.
* The default gateway.
* DNS resolution.
* The router or internet connection.
* Windows network configuration.

No changes will be made until the initial checks have been completed.

3. Troubleshooting Procedure

Step 1 — Check the Network Connection

Verify whether the computer is connected through Wi-Fi or Ethernet.

Check the Windows network status and confirm whether the connection is active.

Step 2 — Inspect the IP Configuration

Open Command Prompt and run:

ipconfig /all

Review the following information:

* IPv4 Address
* Subnet Mask
* Default Gateway
* DNS Servers

Record the results and check for an unexpected or missing IP configuration.

Step 3 — Test the Network Connection

Run the following commands:

ping 127.0.0.1
ping <default-gateway>

Replace <default-gateway> with the actual gateway address shown by ipconfig.

These tests help check the local TCP/IP stack and connectivity to the default gateway.

Step 4 — Test External Connectivity

Run:

ping 1.1.1.1

Record whether replies are received or packets are lost.

Note that a failed ping does not, by itself, prove that internet access is unavailable because some networks block ICMP traffic.

Step 5 — Test DNS Resolution

Run:

nslookup example.com

Check whether the hostname resolves to an IP address.

If external connectivity appears to work but name resolution fails, investigate DNS configuration.

4. Root Cause

Pending investigation.

The root cause will be documented only after the test results have been reviewed.

5. Resolution

Pending investigation.

Any corrective action will depend on the evidence collected during troubleshooting.

6. Customer Communication

The user should receive a clear explanation of the problem, the troubleshooting performed, and the outcome.

If the issue cannot be resolved immediately, communicate the next steps and any escalation requirements.

7. Prevention and Lessons Learned

The final documentation will include any relevant preventive measures, such as checking network configuration, validating DNS settings, or escalating a suspected router or ISP issue.

8. Evidence and Results

The actual commands, outputs, findings, and final resolution will be added after the lab investigation.

Important: This is a lab simulation. No real customer incident is being claimed, and no troubleshooting results have been recorded yet.
