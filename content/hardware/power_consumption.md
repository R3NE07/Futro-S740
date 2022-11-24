---
title: "Power consumption"
date: 2022-11-18T00:15:57+01:00
draft: false
---
# Power consumption

Der Unterschied in Effizienzklasse rechtertigt meist nicht den Kauf eines besseren Netzteiles, allerdings hatte ich bereits Netzteile vom Vorgänger des S740 die nahezu doppelt so viel Strom verbrauchten (wahrscheinlich durch defekt wegen Alter) als sie sollten. Dann wiederum hatte ich auch ein billiges Noname 12V Netzteil das minimal sogar besser abgeschnitten hat als das Original von Fujitsu.  
Wem der Stromverbrauch wichtig ist sollte sich ein verlässliches Energiemessgerät anschaffen (PM231e, KD-203, ELV Energy Master), da billigere Varianten um mehrere Watt ungenau sind.  

> Tipp: Wer trotzdem ein neues Netzteil braucht, Leicke Netzteile sind am beliebtesten für ihre Effizienz.  

\- Liste mit gemessen Energieverbrauchswerten [>>hier<<](https://github.com/R3NE07/Futro-S740/blob/main/power_consumption.md)


## Offizielles Datenblatt:  
\- long idle 5.01 W  
\- sleep mode power 1.25 W (WoL enabled)  
\- off mode power 0.19 W (WoL disabled)  

***

## Von Benutzern gemessene Werte:  

[8GB RAM, 256GB SSD, Proxmox, PiHole, ioBroker](https://www.mydealz.de/comments/permalink/37566282):  
\- Idle: 2,9W – 3,7W  

[Windows 11](https://www.mydealz.de/comments/permalink/37575538):  
\- Idle: 4W  

[Windows 11](https://www.mydealz.de/comments/permalink/37588489):  
\- Vollast: 14W  
\- Surfen: 9W  

[Vergleich](https://www.mydealz.de/comments/permalink/37588992):  
\- S740 mit Debian 11: 3,4W  
\- Raspberry Pi 4 mit USB-SSD: 5,0W  

[Vergleich](https://www.mydealz.de/comments/permalink/37593024):  
\- S740 mit Fedora 36: 3,3W  
\- Raspberry Pi: 3,7W  

[Linux Mint](https://www.mydealz.de/comments/permalink/37610016):  
\- Idle: 4,5W  
\- Surfen: 10W  

[HomeAssistantOS](https://www.mydealz.de/comments/permalink/37612394):  
\- Idle: 4,6W  

[Proxmox mit allerlei Containern & USB-Geräten](https://www.mydealz.de/comments/permalink/37606163):  
\- 6,5W  

[Ubuntu Server, Nextcloud, ADP-40HH 19V Netzteil](https://www.mydealz.de/comments/permalink/37686884):  
\- Idle: 2,7W  
\- Last: 13,1W  

[Mit angeschlossenem Monitor, Peripherie, ADP-40HP 20V Netzteil](https://www.mydealz.de/comments/permalink/37687812):  
\- 6,5W  
Proxmox, Headless:  
\- 3,3W  
Mit powertop optimiert]:  
\- 2,9W  

[Windows](https://www.mydealz.de/comments/permalink/37689549):  
\- Durchschnitt im Alltagsgebrauch (Office, Surfen): 12W  

[Vergleich](https://www.mydealz.de/comments/permalink/37707039):  
\- S740, Proxmox, 1TB, 4GB RAM: 2,8W  
\- Raspi 3, Debian, piHole: 2,6W  

[S740, Proxmox](https://www.mydealz.de/comments/permalink/37714795):  
\- Idle: 2,8W  
\- Standby: 0,6W  

[S740, Proxmox](https://www.mydealz.de/comments/permalink/37736092):  
\- mit 4GB RAM: ca. 3W  
\- mit 16GB RAM: ca. 6,5W  

[S740, Proxmox](https://www.mydealz.de/comments/permalink/37675240):  
\- mit 4GB RAM: ca. 6W  
\- mit 16GB RAM: ca. 10W  

[S740, Proxmox, 16GB RAM](https://www.mydealz.de/comments/permalink/37747947):  
\- Labornetzteil 19 V: ca. 4,8 W  
\- Labornetzteil 12 V: ca. 4,6 W  
\- Labornetzteil 9 V: ca. 4,5 W  
\- Steckernetzteil 12 V/1,5 A, Effizienzstufe V: ca. 7 W  
\- Futro-Nezteil 19V/2,1 A, Effizienzstufe VI: ca. 7,2 W  

[S740, 8GB RAM, Labornetzteil](https://www.mydealz.de/comments/permalink/37758713):  
\- Idle im Netzwerk: 2,3W  
\- Suspended: 0,4W  
Mit 16GB RAM2:  
\- Idle über Netzwerk: 2,3W  
\- Während memtest: 8,0W  

[S740, Proxmox, 12V Labornetzteil](https://www.mydealz.de/comments/permalink/37840567):  
\- mit Micron 8GB 2666Mhz RAM: 2,2W  
\- mit Crucial 16GB 2400Mhz RAM: 4,6W  

[Proxmox, 7 Container, 8GB RAM](https://www.mydealz.de/comments/permalink/37821524):  
\- Idle: ca. 3W  

[ioBroker, Deconz, piHole](https://www.mydealz.de/comments/permalink/37834024):  
\- 4-6W  

[Proxmox, 120GB SSD, 8GB RAM](https://www.mydealz.de/comments/permalink/37965374):  
\- Idle: 2,5W  
\- mit WLAN ModuL +1W  
\- Zigbee Stick +0W  
\- DP Monitor angeschlossen +1W  
\- Tastatur angeschlosse +0,5W  
\- mit PiHole Container +0W  
\- mit HomeAssistant OS +1,25W  
\- mit OpenMediavault Container +0W  
\- mit powertop alle Prozesse auf „good“ getweaked -0,5W  

[Proxmox]():  
\- Fujitsu ADP-40HH A 19V/2,1A Netzteil: 2,8W - 3,5W  
\- Noname 12V/2A Netzteil: identisch mit dem Fujitsu  

[S740](https://www.mydealz.de/comments/permalink/38082473):  
\- mit USB Festplatten: 10W – 12W  
\- ohne USB Platten: 3W – 4W  
