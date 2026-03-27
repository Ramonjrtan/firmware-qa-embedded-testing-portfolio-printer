# BUG-001: Print Job Lost After Power Interruption

## Severity
High

## Priority
Critical

## Module
Print / Firmware

## Environment
- Firmware Version: v1.2.3
- Connection: USB / Network
- Device: All-in-One Printer

## Description
When a power interruption occurs during an active print job, the printer does not recover the job upon restart, resulting in data loss.

## Steps to Reproduce
1. Send a multi-page print job
2. While printing is in progress, turn off the device
3. Restart the printer

## Expected Result
- Printer resumes the print job OR
- Job is stored and reprocessed after restart

## Actual Result
- Print job is lost
- No notification or recovery attempt

## Impact
- Data loss for users
- Critical issue in business environments (e.g., reports, invoices)

## Recommendation
- Implement job persistence mechanism
- Add recovery queue after restart