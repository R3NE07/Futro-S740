---
title: "Hw Content"
date: 2022-11-22T23:58:53+01:00
draft: false
---

# 1 - Hardware  

## Inhalt

### 1.2 - Specs  

| Prozessor & Grafik |  |
| --- | --- |
| CPU | Intel® Celeron®-Prozessor J4105 (4x 1,5-2,5GHz; 10W TDP; 4MB Cache) |
| iGPU | Intel® UHD-Grafik 600 (max. 4096x2160 60Hz) |

| Memory |  |
| --- | --- |
| Flash | M.2 SATA 128GB / 64GB / 32GB ( / 16GB? ) |
| RAM | DDR4 2400MHz 4GB / 8GB |

| Peripherie |  |
| --- | --- |
| Ethernet | 10/100/1000 Mbit/s Realtek RTL8111G |
| WiFi | Optional: Intel Wireless-AC 9260 |
| Audio | 1x Line-Out, 1x Mikrofon, 1x Kopfhörer (Realtek ALC671) |
| USB 2.0 | 4x hinten |
| USB 3.0 | 2x vorne, Optional: 1x USB-C hinten |
| DisplayPort | 2x DP1.2a |
| Seriell (RS232) | Optional: hinten |
| Kensington-Lock | 1x hinten |

| Power |  |
| --- | --- |
| Eingang | 8V-24V, Typ. 5-15W, Max. 5A/100W |
| Stecker | 5.5x2.5 Hohlstecker (Minuspol außen) |
| Ausgeschaltet | 0,19W (WoL aus) / 1,25W (WoL an) |
| Idle | ca. 3W |
| Surfen | ca. 10W |
| Unter Last | ca. 14W |

| Maße |  |
| --- | --- |
| B x T x H | 36 x 165 x 147 mm |
| B x T x H (mit Standfuß) | 76 x 175 x 158 mm |
| Gewicht | 575g (je nach Konfiguration) |

### 1.3 - Netzteil  

Manche Geräte werden mit dem 19V/2,1A; Effizienzstufe VI (ADP-40HH), manche mit dem 20V/2,0A; Stufe V (ADP-40HP) geliefert.

### 1.4 - CPU  

Der Intel J4105 ist ein Gemini Lake SoC wie man sie auch in anderen preiswerten Mini PCs und Laptops findet.

Ausgabe aus Linux’s /proc/cpuinfo:

```
vendor_id	: GenuineIntel  
cpu family	: 6  
model		: 122  
model name	: Intel(R) Celeron(R) J4105 CPU @ 1.50GHz  
stepping	: 1  
microcode	: 0x3c  
cpu MHz      : 2014.580  
cache size	: 4096 KB  
physical id	: 0  
siblings	: 4  
core id		: 0  
cpu cores	: 4  
apicid		: 0  
initial apicid	: 0  
fpu		: yes  
fpu_exception	: yes  
cpuid level	: 24  
wp		: yes  
flags		: fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx pdpe1gb rdtscp lm constant_tsc art arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc cpuid aperfmperf tsc_known_freq pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 sdbg cx16 xtpr pdcm sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave rdrand lahf_lm 3dnowprefetch cpuid_fault cat_l2 pti cdp_l2 ssbd ibrs ibpb stibp ibrs_enhanced tpr_shadow vnmi flexpriority ept vpid ept_ad fsgsbase tsc_adjust smep erms mpx rdt_a rdseed smap clflushopt intel_pt sha_ni xsaveopt xsavec xgetbv1 xsaves dtherm ida arat pln pts umip rdpid md_clear arch_capabilities  
bugs		: cpu_meltdown spectre_v1 spectre_v2 spec_store_bypass  
bogomips	: 2995.20  
clflush size	: 64  
cache_alignment : 64  
address sizes	: 39 bits physical, 48 bits virtual  
power management:  
```

### 1.4 - PCI  

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

### 1.5 - Motherboard  

Abgespeckte Variante des Kontron D3544-S2:  
\- bestückt: COM2 (RS232), M.2-SSD, M.2-WiFi/BT, SPDIF-Pinheader, Buzzer  
\- unbestückt: COM1 (RS232/422/485), USB 2.0 header, Fan-Header, SATA-Power, 24Bit LVDS, LVDS-Backlight, LVDS Voltage Select, USB3.0 Header, SATA1, SATA0, Intrusion-Sensor, eDP, Monospeaker-Pinheader, FP Audio Pinheader

### 1.6 - Erweiterungen  

\- USB-C Lässt sich auch ohne proprietärem Fujitsu Kabel nachrüsten ([1](https://www.mydealz.de/comments/permalink/37704282), [2](https://www.mydealz.de/comments/permalink/37610315), [3](https://www.mydealz.de/comments/permalink/37656704), [4](https://www.mydealz.de/comments/permalink/37722851), [5](https://www.mydealz.de/comments/permalink/37810617), [6](https://www.mydealz.de/comments/permalink/38001225)), erreicht aber nur USB 2.0 Geschwindigkeiten >480MB/s ([1](https://www.mydealz.de/comments/permalink/38046486)]  
\- 2 weitere USB 3.0 Ports mit internem Header möglich ([1](https://www.mydealz.de/comments/permalink/37745987), [2](https://www.mydealz.de/comments/permalink/37760719))  
\- 1 weiterer USB 2.0 Port mit internem Header (unbestückt!) möglich  
\- Standard WiFi Karte: Intel 9260 (jede M.2 Karte sollte passen)  
\- M.2 WiFi Port soll CNVi only sein ([1](https://www.mydealz.de/comments/permalink/37455555)), non-CNVi Karten funktionieren aber auch ([1](https://www.mydealz.de/comments/permalink/37792213))  
\- Es gibt M.2 LAN-Karten die bis zu 2 weitere LAN-Buchsen hergeben (1, 2, 3, 4, 5, 6, 7, )  
  \- eine Firewall/AdBlocker lässt sich statt mit einem 2. LAN Port auch mit VLAN umsetzen  
\- Mit PD Dummy kann eine Powerbank als Stromversorgung & USV eingesetzt werden ([1](https://www.mydealz.de/comments/permalink/37733114))  
\- RS232 Stecker nachrüsten ([1](https://www.mydealz.de/comments/permalink/38078623))  

### 1.7 - Festplatten / M.2 Ports  

\- im M.2 SSD Port (B-Key) passen 2242, 2260, 2280 rein (Bsp: [Transcend](https://www.amazon.de/Transcend-240GB-SATA-MTS420S-TS240GMTS420S/dp/B076PGM4Y5))   
\- es passen gleichzeitig eine 2280 SSD UND ein 2230 WiFi Modul rein ([1](https://www.mydealz.de/comments/permalink/38191471))  
\- M.2-WiFi Port unterstützt PCIe-Schnittstelle, USB2.0 und KEIN SATA  
\- M.2-SSD Port unterstützt SATA UND PCIe ([1](https://www.mydealz.de/comments/permalink/37618826), [2](https://www.mydealz.de/comments/permalink/37686863)) (das nur SATA funktioniert steht im Offiziellen Datenblatt, ist aber falsch: im Datenblatt des D3544-S steht es richtig)  
\- in den M.2 Ports lassen sich Adapter (Bsp: [1](https://a.aliexpress.com/_EQlO1vv), [2](https://www.aliexpress.com/item/1005004399059626.html)) für normale NVME-SSDs (M-Key) oder PCIe-zu-SATA-Adapter ([1](https://www.mydealz.de/comments/permalink/37658544), [2](https://www.mydealz.de/comments/permalink/37621967), [3](https://www.mydealz.de/comments/permalink/37687162), [4](https://www.mydealz.de/comments/permalink/37801298), [5](https://www.mydealz.de/comments/permalink/37847666), [6](https://www.mydealz.de/comments/permalink/37842619), [7](https://www.mydealz.de/comments/permalink/37913510), [8](https://www.mydealz.de/comments/permalink/38072935), [9](https://www.mydealz.de/comments/permalink/38143524), [10](https://www.mydealz.de/comments/permalink/38096778), [11](https://www.mydealz.de/comments/permalink/38102548), [12](https://www.mydealz.de/comments/permalink/38127490), [13](https://www.mydealz.de/comments/permalink/38159994)) anschließen (JMB575 Chip ist nur Port Multiplier, JMB585 wahre PCIe zu SATA Bridge ([1](https://www.mydealz.de/comments/permalink/37733413)))  
\- 2 unbestückte SATA Stecker lassen sich nachlöten (SATA1 funktioniert nicht gleichzeitig mit einer SATA SSD im M.2-SSD Port) ([1](https://www.mydealz.de/comments/permalink/38114275))  
\- SATA Power von USB Adapter beziehen ([1](https://www.mydealz.de/comments/permalink/37847969), [2](https://www.mydealz.de/comments/permalink/38145355))  
\- SATA Power mit selbstgebastelten Kabel vom internen Power In beziehen & 12V statt 19V Netzteil benutzen ([1](https://www.mydealz.de/comments/permalink/38149298), [2](https://www.mydealz.de/comments/permalink/38072259))  
\- am unbestückten SATA Power Stecker liegen bei manchen 5V & 12V an, bei manchen nicht ([1](https://www.mydealz.de/comments/permalink/38164885), [2](https://www.reddit.com/r/homelab/comments/xmr07d/comment/iptq1g1/))  
\- 2,5” SSD mit M.2 B-Key zu SATA Adapter ([1](https://www.mydealz.de/comments/permalink/37666881))  
\- Wieviele Festplatten können Intern versorgt werden? ([1](https://www.mydealz.de/comments/permalink/37688485))  

> Nützliches:  
\- Es gibt M.2 SSDs, die benutzen die PCIe-Schnittstelle (genannt NVMe SSD, benutzen meist 
M-Key oder selten auch B/M-Key)  
\- Wie die Standard verbaute SSD, gibt es aber auch M.2 SSDs, die benutzen noch die SATA-Schnittstelle (genannt NGFF SSD, benutzt B-Key oder B/M-Key)  
\- Normale SATA HDDs muss man neben dem SATA-Kabel auch irgendwie mit 5V & 12V versorgen  
\- Für 2,5“ SATA SSDs reicht (meistens) nur 5V

### 1.8 - PoE  

Das proprietäre Fujitsu PoE-Modul ist optional erhältlich.

### 1.9 - RAM  

\- 1x SO-DIMM Slot (non-ECC)  
\- Offiziell max. 8GB, mit selbem Chipsatz wurden maximal 2x16GB bestätigt, 1x32GB ist wohl nicht machbar ([1](https://www.reddit.com/r/homelab/comments/flqcs6/asrock_j4105itx_32gb_success/))  
\- Von 16GB RAM Riegeln wird scheinbar nur Dual Rank unterstützt (8 Chips pro Seite) und kein Single Rank (4 Chips pro Seite), von kleineren Größen werden wohl aber auch Single Rank Riegel unterstützt ([1](https://www.mydealz.de/comments/permalink/37675998))  

\- Liste mit funktionierenden RAM Modulen {{< ref "ram_modules.md" >}} [>>oderhier<<](https://github.com/R3NE07/Futro-S740/blob/main/ram_modules.md)
