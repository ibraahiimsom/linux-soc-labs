Phase 1 Week 1 Day 1

## Topics Covered
- Linux filesystem navigation
- Viewing logs
- SSH failed login analysis
- grep usage
- awk basics
- Counting log events
- Git initialization

Commands Used

```bash
pwd
ls
ls -la
cd /var/log
tail auth.log
sudo grep "Failed password" auth.log
sudo grep "Failed password" auth.log | wc -l
sudo grep "Failed password" auth.log | awk '{print $11}'
sudo grep "Failed password" auth.log | awk '{print $11}' | sort | uniq -c
```

What I Learned
- Linux logs are critical for SOC investigations
- auth.log stores authentication activity
- grep is used to search security events
- awk can extract attacker IP addresses
- SOC analysts use logs to investigate brute-force attacks
- Repeated IP analysis helps identify attackers
