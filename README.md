# MS17-010-EternalBlue
EternalBlue Checker for mac!
MS17-010 Checker for macOS

This repository contains a BashBunny payload and a Python script for checking if a target system is vulnerable to the MS17-010 exploit (EternalBlue). The BashBunny payload copies the Python script to the target macOS system, executes the script, and removes the script when done.
Files

    payload.txt: BashBunny payload script for macOS.
    ms17-010_checker.py: Python script that checks if a target system is vulnerable to the MS17-010 exploit.

Usage
BashBunny Payload

    Save the payload.txt script as payload.sh on the BashBunny device in a switch folder (e.g., /payloads/switch1/payload.sh).
    Copy the ms17-010_checker.py script to the root of the BashBunny device storage (e.g., /Volumes/BashBunny/ms17-010_checker.py).
    Insert the BashBunny device into the target macOS system and wait for the payload to execute.

Python Script

The Python script can be run independently from the command line with the following arguments:

    -t, --targets: Target(s) to attack (IP addresses, IP ranges, or file containing IPs)
    -u, --user: Username to authenticate with (optional)
    -p, --password: Password for the specified user (optional)
    -d, --domain: Domain for the specified user (optional)

Example:

python ms17-010_checker.py -t 192.168.1.1/24 -u username -p password -d domain

Notes

    The payload script is designed for macOS systems.
    Ensure that the BashBunny device is in HID mode (ATTACKMODE HID STORAGE).
    Modify the target IPs in the payload script as needed.
    fuck bitches, get money.
