# myOwnFirewall

Simple bash script to have an automated firewall in linux using IPTABLES.

This script is part of an articles saga that you can read in http://rolandocaldas.com (spanish blog)

- First article: [Banear IPs en linux automáticamente con IPTABLES](http://rolandocaldas.com/linux/script-para-banear-ips-en-linux-automaticamente)

## Options

### Script like service

The bash script runs like a service so it's necessary start the script to use it.

To start the service run:


```bash
/etc/myOwnFirewall/myOwnFirewall start
```

### Automatically banned ip list

The script reads a text file and bans all the ips of this file when the script starts

### Ban a new ip 

You can add a new ip to the banned ip list running the command

```bash
/etc/myOwnFirewall/myOwnFirewall ban [ip]
```

### Unban a new ip

you can remove a ip from the banned ip list running the command

```bash
/etc/myOwnFirewall/myOwnFirewall unban [ip]
```

### Stop the firewall

You can stop the firewall (and remove all their rules) if you run the command

```bash
/etc/myOwnFirewall/myOwnFirewall stop
```

### Restart the firewall

You can restart the firewall if you run the command

```bash
/etc/myOwnFirewall/myOwnFirewall restart
```

## Version info

The current version is the v0.1, the initial version.
