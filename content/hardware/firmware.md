---
title: "Firmware"
date: 2022-11-18T00:15:57+01:00
draft: false
---

# Firmware  
TODO general overview introduction sentence

## BIOS/UEFI  

Das Boot Menü (um auszuwählen von wo gebootet wird) lässt sich durch drücken von F12 beim Hochfahren erreichen, das BIOS Setup (Einstellungen) mit F2.

### Versions  

\- Platzhalter -

### BIOS/UEFI Setup  

\- Platzhalter -

### BIOS/UEFI Update  

Das BIOS lässt sich übere mehrere Wege updaten:  

\- mit dem fwupd Befehl in Linux ([1](https://www.mydealz.de/comments/permalink/37708487), [2](https://www.mydealz.de/comments/permalink/37711285))  
&nbsp;&nbsp;\- `sudo fwupdmgr refresh`  
&nbsp;&nbsp;\- `sudo fwupdmgr update`  

\- mit einem USB-Stick (ohne vorinstallierten OS) ([1](https://www.mydealz.de/comments/permalink/37708446), [2](https://www.mydealz.de/comments/permalink/37709993), [3](https://www.mydealz.de/comments/permalink/37716882), [4](https://www.mydealz.de/comments/permalink/37775352), [5](https://www.mydealz.de/comments/permalink/37792344), [6](https://www.mydealz.de/comments/permalink/37997294))  
&nbsp;&nbsp;\- Admin Pack herunterladen  
&nbsp;&nbsp;\- Inhalt der ZIP Datei auf einen leeren USB Stick kopieren (einfach per drag & drop)  
&nbsp;&nbsp;\- Den S740 hochfahren und F12 drücken  
&nbsp;&nbsp;\- Den USB Stick auswählen um von dem zu booten  
&nbsp;&nbsp;\- Alle folgenden Anweisungen einfach bestätigen bis es heißt Update fertig  

\- Automatisches Update ([1](https://www.mydealz.de/comments/permalink/37778572), [2](https://www.mydealz.de/comments/permalink/37855490)) (noch unbestätigt ob dies funktioniert)  

Download Links:  
\- [Admin Pack (V5.0.0.13 - R1.12.0 (05.07.2021))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=C5F54F71-16C4-46A8-A067-43392696090A)  
\- [Admin Pack (V5.0.0.13 - R1.13.0 (23.09.2022))](https://support.ts.fujitsu.com/IndexDownload.asp?SoftwareGuid=4949FC92-449A-4C02-A371-9486C4C0F769)  

### Standard OS  

\- eLux® RP  
\- Windows® 10 IoT Enterprise 2019 LTSC  
\- Windows® 10 IoT Enterprise 2016 LTSC  
