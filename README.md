## Server
1. copy file `server/restartVPN` to dir /etc/cron.hourly
2. start docker by docker-compose

> PS: modify some parameters of vpn.env file, such as PSK, USER, PASSWORD. 

## Client
> PS: you must attention that the ca.pem file must be cover which you use.
1. copy file `listen-vpn.service` to dir `/etc/systemd/system`
2. copy file `listen-vpn` to dir `/usr/bin`

### config client connect to server
#### Precondition
- Ubuntu Desktop 18.04+
#### Connect
reference [here](https://github.com/hwdsl2/setup-ipsec-vpn/blob/master/docs/clients.md#ubuntu-linux)
