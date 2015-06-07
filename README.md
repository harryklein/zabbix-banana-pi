# zabbix-banana-pi

Templets zum Überwachen eines Banana-Pi mit Hilfe von Zabbix http://www.zabbix.com/

Quelle: 

## CPU
Informationen 
zabbix_template_banana_pi_cpu.xml  

## Spannungsversorgung
Informationen zur Stromversurgung: Aktuelle Spannung und Stromaufnahme

zabbix_template_banana_pi_power_supply.xml

# Installation
## Zabbix-Agent
1. sudoers via visudo um zabbix  `ALL=(ALL) NOPASSWD:/usr/bin/cpufreq-info` ergänzen 
2. banana_pi.conf nach /etc/zabbix/zabbix_agentd.conf.d/ kopieren 
3. Zabbix-Agent neu starten

## Zabbix-Server 
1. Beide Templates im Zabbix-Server importieren
2. Templates des Banana-Pi-Host zuweisen
3. Ltestest Data prüfen

