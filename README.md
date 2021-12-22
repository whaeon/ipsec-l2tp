## Server
1. copy file `server/restartVPN` to dir /etc/cron.hourly
2. start docker by docker-compose

> PS: modify some parameters of vpn.env file, such as PSK, USER, PASSWORD. 

## Client
### config client connect to server
#### Precondition
- Ubuntu Desktop 18.04+
#### Connect
reference [here](https://github.com/hwdsl2/setup-ipsec-vpn/blob/master/docs/clients.md#ubuntu-linux)

> you must attention that the ca.pem file must be cover which you use.
> before you move the listen-vpn file, you need to modify the vpnserver and dev-name parameter in it. the device name was configured by reference what you input above 
1. copy file `listen-vpn.service` to dir `/etc/systemd/system`, then you can manage the listen-vpn service by `systemctl` cammand
2. copy file `listen-vpn` to dir `/usr/bin`
