---
title: "PCI & Motherboard"
date: 2022-11-22T23:58:53+01:00
draft: false
---

# PCI Connection 
\- Der S740 besitzt weder PCIe noch mPCIe Stecker
\- Dafür haben die M.2 Ports PCIe Schnittstellen mit jeweils PCIe 2.0 x1 und einer Datenrate von max. 5Gbit bzw. Netto nur 500MByte/s

Ausgabe von Linux Befehl „lspci“:

```
00:00.0 Host bridge: Intel Corporation Gemini Lake Host Bridge (rev 03)
00:00.1 Signal processing controller: Intel Corporation Celeron/Pentium Silver Processor Dynamic Platform and Thermal Framework Processor Participant (rev 03)
00:00.3 System peripheral: Intel Corporation Device 3190 (rev 03)
00:02.0 VGA compatible controller: Intel Corporation UHD Graphics 605 (rev 03)
00:0f.0 Communication controller: Intel Corporation Celeron/Pentium Silver Processor Trusted Execution Engine Interface (rev 03)
00:12.0 SATA controller: Intel Corporation Device 31e3 (rev 03)
00:13.0 PCI bridge: Intel Corporation Gemini Lake PCI Express Root Port (rev f3)
00:13.2 PCI bridge: Intel Corporation Gemini Lake PCI Express Root Port (rev f3)
00:13.3 PCI bridge: Intel Corporation Gemini Lake PCI Express Root Port (rev f3)
00:14.0 PCI bridge: Intel Corporation Gemini Lake PCI Express Root Port (rev f3)
00:14.1 PCI bridge: Intel Corporation Gemini Lake PCI Express Root Port (rev f3)
00:15.0 USB controller: Intel Corporation Device 31a8 (rev 03)
00:16.0 Signal processing controller: Intel Corporation Celeron/Pentium Silver Processor Serial IO I2C Host Controller (rev 03)
00:16.1 Signal processing controller: Intel Corporation Celeron/Pentium Silver Processor Serial IO I2C Host Controller (rev 03)
00:16.2 Signal processing controller: Intel Corporation Device 31b0 (rev 03)
00:16.3 Signal processing controller: Intel Corporation Device 31b2 (rev 03)
00:17.0 Signal processing controller: Intel Corporation Device 31b4 (rev 03)
00:17.1 Signal processing controller: Intel Corporation Device 31b6 (rev 03)
00:17.2 Signal processing controller: Intel Corporation Device 31b8 (rev 03)
00:17.3 Signal processing controller: Intel Corporation Device 31ba (rev 03)
00:19.0 Signal processing controller: Intel Corporation Celeron/Pentium Silver Processor Serial IO SPI Host Controller (rev 03)
00:19.1 Signal processing controller: Intel Corporation Celeron/Pentium Silver Processor Serial IO SPI Host Controller (rev 03)
00:19.2 Signal processing controller: Intel Corporation Celeron/Pentium Silver Processor Serial IO SPI Host Controller (rev 03)
00:1f.0 ISA bridge: Intel Corporation Device 31e8 (rev 03)
00:1f.1 SMBus: Intel Corporation Celeron/Pentium Silver Processor Gaussian Mixture Model (rev 03)
02:00.0 Ethernet controller: Realtek Semiconductor Co., Ltd. RTL8111/8168/8411 PCI Express Gigabit Ethernet Controller (rev 0c)
```

# Motherboard  

Abgespeckte Variante des Kontron D3544-S2:  
\- bestückt: COM2 (RS232), M.2-SSD, M.2-WiFi/BT, SPDIF-Pinheader, Buzzer  
\- unbestückt: COM1 (RS232/422/485), USB 2.0 header, Fan-Header, SATA-Power, 24Bit LVDS, LVDS-Backlight, LVDS Voltage Select, USB3.0 Header, SATA1, SATA0, Intrusion-Sensor, eDP, Monospeaker-Pinheader, FP Audio Pinheader

## Extensions  

\- USB-C Lässt sich auch ohne proprietärem Fujitsu Kabel nachrüsten ([1](https://www.mydealz.de/comments/permalink/37704282), [2](https://www.mydealz.de/comments/permalink/37610315), [3](https://www.mydealz.de/comments/permalink/37656704), [4](https://www.mydealz.de/comments/permalink/37722851), [5](https://www.mydealz.de/comments/permalink/37810617), [6](https://www.mydealz.de/comments/permalink/38001225)), erreicht aber nur USB 2.0 Geschwindigkeiten >480MB/s ([1](https://www.mydealz.de/comments/permalink/38046486)]  
\- 2 weitere USB 3.0 Ports mit internem Header möglich ([1](https://www.mydealz.de/comments/permalink/37745987), [2](https://www.mydealz.de/comments/permalink/37760719))  
\- 1 weiterer USB 2.0 Port mit internem Header (unbestückt!) möglich  
\- Standard WiFi Karte: Intel 9260 (jede M.2 Karte sollte passen)  
\- M.2 WiFi Port soll CNVi only sein ([1](https://www.mydealz.de/comments/permalink/37455555)), non-CNVi Karten funktionieren aber auch ([1](https://www.mydealz.de/comments/permalink/37792213))  
\- Es gibt M.2 LAN-Karten die bis zu 2 weitere LAN-Buchsen hergeben (1, 2, 3, 4, 5, 6, 7, )  
  \- eine Firewall/AdBlocker lässt sich statt mit einem 2. LAN Port auch mit VLAN umsetzen  
\- Mit PD Dummy kann eine Powerbank als Stromversorgung & USV eingesetzt werden ([1](https://www.mydealz.de/comments/permalink/37733114))  
\- RS232 Stecker nachrüsten ([1](https://www.mydealz.de/comments/permalink/38078623))  

###  Mods  

\- Gehäuse lässt sich öffnen indem die 2 Schrauben an der IO-Blende entfernt werden, dann lässt sich die obere Gehäusehälfte nach hinten schieben & abnehmen  
\- unbestückten RS232 Seriell-Port nachlöten ([1](https://www.mydealz.de/comments/permalink/38079460))  
\- 2x unbestückte SATA Ports nachlöten (es müssen zusätzlich je 4x 0402 10nF SMD Kondensatoren nachgelötet werden) ([1](https://www.mydealz.de/comments/permalink/38114275))  

### PoE   

Das proprietäre Fujitsu PoE-Modul ist optional erhältlich.

### WoL

TODO