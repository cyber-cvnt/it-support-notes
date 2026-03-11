# Trust Relationship Between Workstation and Domain Failed

## Problem
A workstation displays the error:

"The trust relationship between this workstation and the primary domain failed."

This prevents the user from logging into the domain.

## Cause
The secure channel between the workstation and the Active Directory domain controller has been broken.

This may happen when:
- Computer password mismatch occurs
- System was restored from backup
- Machine was offline from domain for long period

## Troubleshooting Steps

### 1. Log in Using Local Administrator Account
Use:

.\Administrator

Or a local admin account to access the machine.

### 2. Remove Computer From Domain

Navigate to:

System Properties → Computer Name → Change

Switch from **Domain** to **Workgroup**.

Restart the computer.

### 3. Rejoin Domain

After restart:

1. Go back to **Computer Name settings**
2. Select **Domain**
3. Enter domain name
4. Provide domain administrator credentials

Restart the computer again.

### 4. Test Login
User should now be able to log in using domain credentials.

## Resolution
Rejoining the workstation to the domain re-established the trust relationship.

## Lessons Learned
Domain trust errors typically require removing and rejoining the system to the domain.
