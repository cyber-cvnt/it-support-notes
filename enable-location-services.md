# Location Services Disabled on Windows

## Problem
A user is unable to use applications that require location access because Windows location services are disabled.

## Symptoms
- Applications cannot detect location
- Maps or weather apps fail to load location data
- Location settings appear turned off

## Possible Causes
- Location services disabled in system settings
- Group policy restrictions
- Privacy settings preventing app access

## Troubleshooting Steps

### 1. Open Location Settings

Navigate to:

Settings → Privacy & Security → Location

### 2. Enable Location Services

Turn on:

Location Services

### 3. Allow Apps to Access Location

Ensure the option:

Allow apps to access your location

is enabled.

### 4. Enable Location for Specific Apps

Scroll down and confirm that the application needing location access is turned on.

### 5. Restart the Application

Close and reopen the application to apply the new settings.

## Resolution
After enabling location services and allowing application access, the user was able to successfully use location-based features.

## Lessons Learned
Privacy settings can restrict application functionality. Always verify location permissions when troubleshooting location-based issues.
