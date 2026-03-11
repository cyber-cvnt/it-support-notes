# Printer Can Print But Cannot Scan

## Problem
A user is able to print documents successfully from the office printer but cannot scan documents to their computer.

## Possible Causes
- Scanner driver not installed
- Scanner service not running
- Incorrect scanning software
- Network discovery disabled

## Troubleshooting Steps

### 1. Confirm Printer Supports Scanning
Check if the printer model has scanning capability.

### 2. Install/Update Scanner Drivers
Download the latest drivers from the manufacturer's website.

Example:
HP printers require **HP Scan** or **HP Smart** software.

### 3. Check Windows Scan Service
Open: 

Services → Windows Image Acquisition (WIA)

Ensure the service is:
- Running
- Set to **Automatic**

### 4. Test Using Windows Scan
Open:

Windows Scan

Attempt to scan a document.

### 5. Reinstall Printer
If the issue persists:
- Remove printer
- Restart system
- Reinstall printer and scanner drivers

## Resolution
After installing the correct scanning drivers and restarting the WIA service, scanning functionality was restored.

## Lessons Learned
Printing and scanning use **different drivers**, so printing working does not guarantee scanning will work.
