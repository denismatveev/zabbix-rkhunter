# zabbix-rkhunter

## Install

copy directory scripts in `/etc/zabbix/`
import template to Zabbix GUI

## Checking

To check just run `zabbix_sender -c /etc/zabbix/zabbix_agentd.conf -k custom.rkhunter -o 0`
and read logs, if in servers logs you see that key became supported, it's OK.
Also you can run rkhunter in scripts/rkhunter and `tail -f /var/log/rkhunter/rkhunter.log` to watch what's going on.

Of cause you should configure rkhunter before install these scripts for Zabbix.


