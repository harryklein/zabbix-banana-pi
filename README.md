# zabbix-banana-pi

Templets zum Überwachen eines Banana-Pi mit Hilfe von Zabbix http://www.zabbix.com/ Ermittelt werden Speed der CPUs, Temperatur der CPU und Spannung und Strom der Stromversorgung.

Quelle: http://znil.net/index.php?title=Temperatur_/_Spannung_etc._des_Banana_Pi_selbst_auslesen

## CPU
Informationen zum Speed der CPUs und Temperator der CPU ermitteln

Template: server/zabbix_template_banana_pi_cpu.xml  

## Spannungsversorgung
Informationen zur Stromversurgung wie aktuelle Spannung und Stromaufnahmeermitteln.

Template: server/zabbix_template_banana_pi_power_supply.xml

# Installation
## Zabbix-Agent
1. sudoers via visudo um zabbix  `ALL=(ALL) NOPASSWD:/usr/bin/cpufreq-info` ergänzen 
2. banana_pi.conf nach /etc/zabbix/zabbix_agentd.conf.d/ kopieren 
3. Zabbix-Agent neu starten

## Zabbix-Server 
1. Beide Templates im Zabbix-Server importieren
2. Templates der Banana-Pi-Host zuweisen
3. Latest Data prüfen

