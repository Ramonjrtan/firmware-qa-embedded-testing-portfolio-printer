# BUG-002: Print Job Fails Without Retry on Network Disconnect

## Severity
High

## Priority
High

## Module
Network / Print

## Description
When network connection is lost during print job transmission, the system fails immediately without retrying.

## Steps
1. Send print job via WiFi
2. Disable WiFi during transmission

## Expected
- System retries sending job
- OR queues job until network is restored

## Actual
- Job fails instantly
- No retry mechanism

## Impact
- Poor user experience
- Failed print operations in unstable networks

## Recommendation
- Implement retry logic
- Add job queue buffering