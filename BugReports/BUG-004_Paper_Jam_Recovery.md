# BUG-004: Printer Does Not Resume After Paper Jam Clearance

## Severity
Medium

## Priority
High

## Module
Hardware / Print

## Description
After clearing a paper jam, the printer does not resume the job automatically.

## Steps
1. Start print job
2. Simulate paper jam
3. Clear jam

## Expected
- Printer resumes job

## Actual
- Job remains paused
- Requires manual restart

## Impact
- User inconvenience
- Interrupted workflow

## Recommendation
- Auto-resume after error resolution