### all files under the /etc directory whose names begin with rc
`find /etc -name "rc*"`

### all regular files belonging to you; put the result in the file /tmp/findme and errors in/dev/null,
`find / -type f -user hasna -exec ls -l {} + > /tmp/findme 2> /dev/null`
### all subdirectories of /etc
`find /etc -type d`
### all regular files under your home directory that haven't been modified in the last 10 days
`find ~ -type f -mtime +10`
### The 10 largest file in your computer
`find / -type f -exec du -Sh {} + | sort -rh | head -n 10
`
