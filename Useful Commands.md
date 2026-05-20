*Upgrades shell and breaks out of restricted bash*
```
python3 -c 'import pty; pty.spawn("/bin/bash")'
**OR**
python -c 'import pty; pty.spawn("/bin/bash")'
export PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/tmp
export TERM=xterm-256color
alias ll='ls -lsaht --color=auto'


# Keyboard Shortcut: Ctrl + Z (Background Process.) 
# On host
stty raw -echo ; fg ; reset 
stty columns 200 rows 200
```

*Update `/etc/hosts` file*
```
echo "192.168.1.100 myhost.local" | sudo tee -a /etc/hosts
```