+++ 
title = "SSD Drives" 
weight = 13 
+++

# SSD/HDD & M.2 Ports  

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

## Usable Drives

### BRAND 1
### BRAND N

### !Unasable Drives!

### BRAND 1 Not working
### BRAND N Not working
