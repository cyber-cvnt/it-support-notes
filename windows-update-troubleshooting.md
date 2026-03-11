# Windows Update Not Working

## Problem
A user is unable to install or check for Windows updates.

## Symptoms
- Windows Update fails during installation
- Update process freezes
- Error codes appear during updates

## Possible Causes
- Corrupted update files
- Windows Update service not running
- Network connectivity issues
- System restart required

## Troubleshooting Steps

### 1. Check Internet Connection
Ensure the system is connected to a stable network.

### 2. Restart the Computer
A restart may resolve temporary update errors.

### 3. Run Windows Update Troubleshooter

Navigate to:

Settings → System → Troubleshoot → Other Troubleshooters

Run:

Windows Update Troubleshooter

### 4. Restart Windows Update Services

Open Command Prompt as Administrator and run:
net stop wuauserv
net stop bits
net start wuauserv
net start bits

### 5. Check for Updates Again

Navigate to:

Settings → Windows Update → Check for Updates

## Resolution
Restarting Windows Update services and running the troubleshooter allowed the system to successfully install updates.

## Lessons Learned
Windows update failures are commonly related to service interruptions or corrupted temporary update files.
