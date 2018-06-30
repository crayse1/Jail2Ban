# Jail2Ban
Fail2ban version for windows in vb.net - inspired on wail2ban - json based -> jail :)

## What project does
Jail2Ban locks IP addresses using Windows Firewall

## How it works
- Search for failed login attempts into the windows event log
- Retrives the remote endpoint ip address from the log properties
- Creates a single firewall rule if not existing (wail2ban is different in this approach)
- Adds a locked IP address
- Shows into the console the "jail" status

## Future updates:
- Create a json configuration file 
- Handle different operating systems
- Add sql server ban
- Log every failed attempt (windows log does not retain a lot of data by default setting)
- Add a redemption time
- Create a webservice (maybe REST) to share between different server an IP reputation
- Add into the webservice project a web page showing IP reputation and logs
- Publish webservice for the community (source code of webservice will be shared in this repo)
