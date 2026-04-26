# Day 4 – Log Searching Investigation

## 🚨 Alert Summary

Multiple failed SSH login attempts detected in /var/log/auth.log for user 'fakeuser'.

## 🔍 Investigation Notes

* Command used: `grep "Failed password" auth.log`
* Observed three failed login attempts
* Attempts originated from 127.0.0.1 (localhost)
* Attempts occurred within a short timeframe
* No successful authentication observed

## 🕒 Timeline

* Step 1: SSH login attempts initiated
* Step 2: Three failed password attempts recorded
* Step 3: No successful login observed

## ✅ Decision

True Positive

Reason:
Repeated failed login attempts from the same source indicate potential brute-force behaviour.

## 📈 Escalation Note

Yes – escalate to Level 2 SOC

Reason:
Activity matches brute-force attack patterns and requires further investigation and monitoring.

## 📘 Playbook Reference

Brute-force login detection playbook

