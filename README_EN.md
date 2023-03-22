# Futro S740 - Guide/ Specs/ Information

\> Deutsche Version [hier](https://github.com/R3NE07/Futro-S740/blob/main/README.md) <  

## Inhalt

[1 - Hardware](README.md#1---hardware)  
&nbsp;&nbsp;[1.1 - Overview](README.md#11---overview)  
&nbsp;&nbsp;[1.2 - Specs](README.md#12---specs)  
&nbsp;&nbsp;[1.3 - Powersupply](README.md#13---powersupply)  
&nbsp;&nbsp;[1.4 - CPU](README.md#14---cpu)  
&nbsp;&nbsp;[1.4 - PCI](README.md#14---pci)  
&nbsp;&nbsp;[1.5 - Motherboard](README.md#15---motherboard)  
&nbsp;&nbsp;[1.6 - Expansion](README.md#16---expansion)  
&nbsp;&nbsp;[1.7 - Hard Drives / M.2 Ports](README.md#17---hard-drives--m2-ports)  
&nbsp;&nbsp;[1.8 - PoE](README.md#18---poe)  
&nbsp;&nbsp;[1.9 - RAM](README.md#19---ram)  
[2 - Firmware](README.md#2---firmware)  
&nbsp;&nbsp;[2.1 - BIOS](README.md#21---bios)  
&nbsp;&nbsp;&nbsp;&nbsp;[2.1.1 - Version](README.md#211---versionen)  
&nbsp;&nbsp;&nbsp;&nbsp;[2.1.2 - BIOS Setup](README.md#212---bios-setup)  
&nbsp;&nbsp;[2.2 - BIOS Update](README.md#22---bios-update)  
&nbsp;&nbsp;[2.3 - BIOS Recovery](README.md#23---bios-recovery)  
&nbsp;&nbsp;[2.4 - Standard OS](README.md#24---standard-os)  
[3 - Windows / Linux](README.md#3---windows--linux)  
&nbsp;&nbsp;[3.1 Server OS](README.md#31-server-os)  
&nbsp;&nbsp;[3.2 Desktop OS](README.md#32-desktop-os)  
[4 - Mods](README.md#4---mods)  
[5 - Power Consumption](README.md#5---power-consumption)  
[6 - Reportet Problems](README.md#6---reportet-problems)  
[7 - Links](README.md#7---links)  
[8 - Pictures](README.md#8---pictures) 

## Note:

This guide is neither official, complete nor flawless!  
It is merely a compilation of information and reports from other Futro owners.  

***

## 1 - Hardware  

### 1.1 - Overview  

The Futro S740 is a thin client from 2018 with an mSTX D3544-A motherboard, which is a slimmed down version of the Kontron D3544-S2 with the Smartcase S500 from the same company.  
Unlike older thin clients, the Futro is not only intended to connect remotely to a server, which then runs software, but the Futro has enough computing power to run as a standalone mini PC.  

### 1.2 - Specs  

| CPU & Graphics |  |  
| --- | --- |  
| CPU | Intel® Celeron®-Processor J4105 (4x 1,5-2,5GHz; 10W TDP; 4MB Cache) |  
| iGPU | Intel® UHD-Grafik 600 (max. 4096x2160 60Hz) |  

| Memory |  |  
| --- | --- |  
| Flash | M.2 SATA 128GB / 64GB / 32GB ( / 16GB? ) |  
| RAM | DDR4 2400MHz 4GB / 8GB |  

| Periphery |  |  
| --- | --- |  
| Ethernet | 10/100/1000 Mbit/s Realtek RTL8111G |  
| WiFi | Optional: Intel Wireless-AC 9260 |  
| Audio | 1x Line-Out, 1x Mic, 1x Headphones (Realtek ALC671) |  
| USB 2.0 | 4x back |  
| USB 3.0 | 2x front, Optional: 1x USB-C back |  
| DisplayPort | 2x DP1.2a |  
| Seriel (RS232) | Optional: back |  
| Kensington-Lock | 1x back |  

| Power |  |  
| --- | --- |  
| Input | 8V-24V, Typ. 5-15W, Max. 5A/100W |  
| Connector | 5.5x2.5 barrel jack (outer barrel negative) |  
| Turned Off | 0,19W (WoL off) / 1,25W (WoL on) |  
| Idle | ca. 3W |  
| Surfing | ca. 10W |  
| Under load | ca. 14W |  

| Dimensions |  |  
| --- | --- |  
| W x D x H | 36 x 165 x 147 mm |  
| W x D x H (with feet) | 76 x 175 x 158 mm |  
| Weight | 575g (depending on configuration) |  

### 1.3 - Powersupply  

Some devices come delivered with the 19V/2.1A; efficiency level VI (ADP-40HH), some with the 20V/2.0A; Stage V (ADP-40HP).  

### 1.4 - CPU  

The Intel J4105 is a Gemini Lake SoC, as also found in other inexpensive mini PCs and laptops.  

Output from Linux's /proc/cpuinfo:  

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

\- The S740 has neither PCIe nor mPCIe connectors  
\- The M.2 ports have PCIe interfaces, each with PCIe 2.0 x1 and a data rate of max. 5Gbit or only 500MByte/s net  

Output of Linux command "lspci":  

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

Slimmed down version of the Kontron D3544-S2:  
\- populated: COM2 (RS232), M.2-SSD, M.2-WiFi/BT, SPDIF pin header, buzzer  
\- not populated: COM1 (RS232/422/485), USB 2.0 header, fan header, SATA power, 24-bit LVDS, LVDS backlight, LVDS voltage select, USB3.0 header, SATA1, SATA0, intrusion sensor, eDP , Monospeaker pin header, FP Audio pin header  

### 1.6 - Extension    

\- USB-C Can also be retrofitted without a proprietary Fujitsu cable ([1](https://www.mydealz.de/comments/permalink/37704282), [2](https://www.mydealz.de/comments/permalink/37610315), [3](https://www.mydealz.de/comments/permalink/37656704), [4](https://www.mydealz.de/comments/permalink/37722851), [5](https://www.mydealz.de/comments/permalink/37810617), [6](https://www.mydealz.de/comments/permalink/38001225), [7](https://www.mydealz.de/comments/permalink/38291707)), [8](https://www.mydealz.de/comments/permalink/38305063), some cables only reach USB 2.0 speepds up to 480MB/s ([1](https://www.mydealz.de/comments/permalink/38046486), [2](https://www.mydealz.de/comments/permalink/38503891)])  
\- 2 additional USB 3.0 ports possible with internal header ([1](https://www.mydealz.de/comments/permalink/37745987), [2](https://www.mydealz.de/comments/permalink/37760719))  
\- 2 additional USB 2.0 ports possible with internal header (unpopulated!)    
\- Standard WiFi card: Intel 9260 (any M.2 card should fit)  
\- Retrofit WiFi card ([1](https://www.mydealz.de/comments/permalink/38263023), [2](https://www.mydealz.de/comments/permalink/38500729))  
\- M.2 WiFi port support CNVi cards only ([1](https://www.mydealz.de/comments/permalink/37455555)), non-CNVi Karten funktionieren aber auch ([1](https://www.mydealz.de/comments/permalink/37792213))  
\- There are M.2 LAN cards that provide up to 2 additional LAN sockets ([1](https://www.mydealz.de/comments/permalink/37760460), [2](https://www.mydealz.de/comments/permalink/37791852), [3](https://www.mydealz.de/comments/permalink/37793620), [4](https://www.mydealz.de/comments/permalink/37993085))  
  \- a firewall/AdBlocker can also be implemented with VLAN instead of with a 2nd LAN port  
\- With PD Dummy, a power bank can be used as power supply & UPS ([1](https://www.mydealz.de/comments/permalink/37733114))  
\- Retrofit RS232 connector ([1](https://www.mydealz.de/comments/permalink/38078623))  

### 1.7 - Hard Drives / M.2 Ports  

\- 2242, 2260, 2280 fit in the M.2 SSD port (B-Key). (eg. [Transcend TS240GMTS420S](https://www.amazon.de/Transcend-240GB-SATA-MTS420S-TS240GMTS420S/dp/B076PGM4Y5), [Kioxia KBG40ZMT128G](https://www.ebay.de/itm/265924089951), [Micron MTFDDAV256TDL](https://www.ebay.de/itm/203881734179?mkcid=1&mkevt=1&mkrid=707-53477-19255-0&campid=5337601838&toolid=10001&siteid=77&customid=1617903000))   
\- If an SSD longer than 2242 is used, the backside must be unpopulated, or you have to cover that side with adhesive tape or unsolder the spacer to prevent a short circuit ([1](https://www.mydealz.de/comments/permalink/38307933), [2](https://www.mydealz.de/comments/permalink/38320056), [3](https://www.mydealz.de/comments/permalink/39081394))  
\- a 2280 SSD AND a 2230 WiFi module fit in at the same time ([1](https://www.mydealz.de/comments/permalink/38191471))  
\- M.2 WiFi port supports PCIe, USB2.0 nut no SATA  
\- M.2 SSD port supports SATA and PCIe ([1](https://www.mydealz.de/comments/permalink/37618826), [2](https://www.mydealz.de/comments/permalink/37686863)) (that only SATA works is in the official data sheet, but it is wrong: in the data sheet of the D3544-S it is correct)  
\- Adapters can be inserted in the M.2 ports (eg. [1](https://a.aliexpress.com/_EQlO1vv), [2](https://www.aliexpress.com/item/1005004399059626.html)) for normal NVME SSDs (M-Key) or PCIe-to-SATA adapters ([1](https://www.mydealz.de/comments/permalink/37658544), [2](https://www.mydealz.de/comments/permalink/37621967), [3](https://www.mydealz.de/comments/permalink/37687162), [4](https://www.mydealz.de/comments/permalink/37801298), [5](https://www.mydealz.de/comments/permalink/37847666), [6](https://www.mydealz.de/comments/permalink/37842619), [7](https://www.mydealz.de/comments/permalink/37913510), [8](https://www.mydealz.de/comments/permalink/38072935), [9](https://www.mydealz.de/comments/permalink/38143524), [10](https://www.mydealz.de/comments/permalink/38096778), [11](https://www.mydealz.de/comments/permalink/38102548), [12](https://www.mydealz.de/comments/permalink/38127490), [13](https://www.mydealz.de/comments/permalink/38159994), [14](https://www.mydealz.de/comments/permalink/38331948), [15](https://www.mydealz.de/comments/permalink/38503891)) anschließen (JMB575 Chip ist nur Port Multiplier, JMB585 wahre PCIe zu SATA Bridge ([1](https://www.mydealz.de/comments/permalink/37733413)))  
\- 2 unpopulated SATA connectors can be soldered on (SATA1 does not work simultaneously with a SATA SSD in the M.2 SSD port) ([1](https://www.mydealz.de/comments/permalink/38114275), [2](https://github.com/R3NE07/Futro-S740/issues/11#issue-1552071065))  
\- Draw SATA power from USB adapter ([1](https://www.mydealz.de/comments/permalink/37847969), [2](https://www.mydealz.de/comments/permalink/38145355), [3](https://www.mydealz.de/comments/permalink/38331948), [4](https://www.mydealz.de/comments/permalink/38503891))  
\- Draw SATA power from the internal Power In with a self-made cable & use 12V instead of 19V power supply ([1](https://www.mydealz.de/comments/permalink/38149298), [2](https://www.mydealz.de/comments/permalink/38072259), [2](https://www.mydealz.de/comments/permalink/38663988))  
\- some have 5V & 12V on the unequipped SATA power connector, some not ([1](https://www.mydealz.de/comments/permalink/38164885), [2](https://www.reddit.com/r/homelab/comments/xmr07d/comment/iptq1g1/))  
\- 2.5” SSD with M.2 B key to SATA adapter ([1](https://www.mydealz.de/comments/permalink/37666881))  
\- How many hard drives can be supplied internally? ([1](https://www.mydealz.de/comments/permalink/37688485))  

> Useful:  
\- There are M.2 SSDs that use the PCIe interface (called NVMe SSD, mostly use M-Key or rarely also B/M-Key)  
\- Like the standard built-in SSD, there are also M.2 SSDs that still use the SATA interface (called NGFF SSD, uses B-Key or B/M-Key)  
\- B-Key & B-M-Key cards fit in a B-Key slot, M-Key & B-M-Key cards fit in an M-Key slot  
\- Normal SATA HDDs have to be supplied somehow with 5V & 12V in addition to the SATA signal cable  
\- For 2.5" SATA SSDs (usually) only 5V is sufficient  

### 1.8 - PoE  

- Proprietary Fujitsu PoE module can be bought seperately (for a lot of money)  
- Alternatively, there are external PoE splitters with a barrel connector ([1](https://github.com/R3NE07/Futro-S740/issues/16#issue-1600581355))  

### 1.9 - RAM  

\- 1x SO-DIMM Slot (non-ECC)  
\- Officially max. 8GB, with the same chipset a maximum of 2x16GB has been confirmed, 1x32GB is probably not feasible ([1](https://www.reddit.com/r/homelab/comments/flqcs6/asrock_j4105itx_32gb_success/))  
\- Apparently 16GB RAM sticks are only supported as dual rank (8 chips per side) and no single rank (4 chips per side), but single rank sticks are also supported in smaller sizes ([1](https://www.mydealz.de/comments/permalink/37675998))  
\- RAM only works up to 2400MHz (faster RAM is simply throttled) ([1](https://www.mydealz.de/comments/permalink/38262231))  

\- List of working RAM modules [>>here<<](https://github.com/R3NE07/Futro-S740/blob/main/ram_modules.md)  

## 2 - Firmware  

### 2.1 - BIOS  

The boot menu (to select where to boot from) can be reached by pressing F12 during boot, the BIOS setup (settings) with F2.  

#### 2.1.1 - Versions  

Download links for update via USB stick:  
\- [Admin Pack (V5.0.0.13 - R1.2.0 (29.03.2018))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=57E45317-A1C6-41AD-AD82-0D6CF8FD2AB8)  
\- [Admin Pack (V5.0.0.13 - R1.3.0 (02.05.2018))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=E971B802-AE66-495B-99E9-1DC8EB23D229)  
\- [Admin Pack (V5.0.0.13 - R1.5.0 (31.07.2018))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=AF6BF439-AC6C-45E4-8400-EF2941A371A4)  
\- [Admin Pack (V5.0.0.13 - R1.6.0 (02.10.2018))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=A22F863D-ACD4-498F-80EB-E6AE0CD0935E)  
\- [Admin Pack (V5.0.0.13 - R1.7.0 (08.11.2018))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=C256FAAB-9F6C-43A5-9F70-BF711A603B85)  
\- [Admin Pack (V5.0.0.13 - R1.8.0 (22.03.2019))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=221729C4-4E3D-49E8-8608-2825A7FB01AE)  
\- [Admin Pack (V5.0.0.13 - R1.10.0 (10.05.2019))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=5BB0C35F-BE7A-44A1-BD3A-032A996E9629)  
\- [Admin Pack (V5.0.0.13 - R1.11.0 (21.10.2019))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=3E511BB2-742F-4AA1-BFFF-172A587C4480)  
\- [Admin Pack (V5.0.0.13 - R1.12.0 (05.07.2021))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=C5F54F71-16C4-46A8-A067-43392696090A)  
\- [Admin Pack (V5.0.0.13 - R1.13.0 (23.09.2022))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=4949FC92-449A-4C02-A371-9486C4C0F769)  

Download links for update via Windows:  
\- [Flash BIOS Update - Desk Flash Instant (V5.0.0.13 - R1.13.0 (23.09.2022))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=1FD0DD8E-79C1-41FE-8AC5-1643B3F186EC)  

#### 2.1.2 - BIOS Setup  

\- Space Holder -


\>> Translation Work In Progress <<
