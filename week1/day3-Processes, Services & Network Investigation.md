
Phase 1 Week 1 Day 3

## Topics Covered
- Linux processes
- Process investigation
- Services and systemctl
- SSH service analysis
- Listening ports
- Network connections
- Login activity investigation
- Bash history analysis

Commands Used

```bash
ps aux
ps aux | grep ssh
top
systemctl list-units --type=service
systemctl status ssh
ss -tulnp
ss -tulnp | grep LISTEN
ip a
ping google.com
who
w
last
lsof -i
cat ~/.bash_history
```

What I Learned
- How to investigate running processes
- How to verify service status
- How to identify listening ports
- How to investigate active users
- How SOC analysts identify suspicious network activity
- How bash history can help incident investigations
