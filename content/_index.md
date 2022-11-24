+++
title = "Home"
weight = 0
+++

General infos and picture

This page is mainly the work of https://github.com/R3NE07/Futro-S740 - i just added the hosting part and restructured the content so that it's deployable via hugo static webpage generator. Many thanks for collecting all the information

## Anmerkung:

Dieser Guide ist weder offiziell, vollständig noch fehlerfrei!  
Er ist lediglich eine Zusammenstellung von Informationen und Berichten anderer Futro Besitzer.  
Wer noch etwas Wissenswertes hat, kann mich gerne anschreiben oder ein Kommentar lassen und ich füge es hinzu.

***

### Theme reference
If you want to use fancy stuff have a look into the theme documentation here:
https://mcshelby.github.io/hugo-theme-relearn/cont/markdown/index.html

# TOC 
TODO

# Overview  

Der Futro S740 ist ein Thinclient aus 2018 mit einem mSTX D3544-A Mainboard, welcher eine abgespackte Version des Kontron D3544-S2 mit dem dazugehörigen Smartcase S500 aus gleichem Hause ist.  
Anders wie ältere Thinclients wird der Futro nicht nur vorgesehen über Fernzugriff sich mit einem Server zu verbinden, auf dem dann Software ausgeführt wird, sondern hat der Futro genug Rechenleistung um als eigenständiger Mini PC zu laufen.

## FAQ/Issues

\- BIOS kann nur EFI Systeme booten, nicht Legacy & Festplatte muss als GPT nicht MBR formatiert sein ([1](https://www.mydealz.de/comments/permalink/37726414), [2](https://www.mydealz.de/comments/permalink/38141002))  
\- Booten von externem USB nicht möglich ([1](https://www.mydealz.de/comments/permalink/37545092))  
\- Booten von TrueNAS nicht möglich ([1](https://www.mydealz.de/comments/permalink/37545132))  
\- Manche DP zu HDMI Adapter können an manchen Monitoren Probleme bringen: kein Bild, nur 1080p, kein Audio ([1](https://www.mydealz.de/comments/permalink/37718448), [2](https://www.mydealz.de/comments/permalink/37770939), [3](https://www.mydealz.de/comments/permalink/37800456), [4](https://www.mydealz.de/comments/permalink/37820943), [5](https://www.mydealz.de/comments/permalink/37862572), [6](https://www.mydealz.de/comments/permalink/37955579), [7](https://www.mydealz.de/comments/permalink/37994093), [8](https://www.mydealz.de/comments/permalink/38035070))  
\- Rattelndes Geräusch: Unter einer der 4 Schrauben die den CPU Kühlkörper festhalten ist eine Unterlegscheibe die zu groß ist - macht aber nichts ([1](https://www.mydealz.de/comments/permalink/37583467))  
\- Bei manchen liegt ein loses „Aluröhrchen“ im PC - das ist eine Art Polster die sonst im inneren des Gehäuses geklebt ist und gegen das I/O Shield drücken würde aus ESD Gründen ([1](https://www.mydealz.de/comments/permalink/37627200), [2](https://www.mydealz.de/comments/permalink/38046826))  
\- Je nach mitgeliefertem Netzteil kommt es zu fiepen im PC ([1](https://www.mydealz.de/comments/permalink/37607473), [2](https://www.mydealz.de/comments/permalink/37634161))  
\- USB-Stick wird nicht als Boot Option aufgelistet ([1](https://www.mydealz.de/comments/permalink/37570172))  
\- Linux bootet nicht? Booteintrag muss manuell angelegt werden ([1](https://www.mydealz.de/comments/permalink/37643719), [2](https://www.mydealz.de/comments/permalink/37612394), [3](https://www.mydealz.de/comments/permalink/37581112), [4](https://www.mydealz.de/comments/permalink/37594025), [5](https://www.mydealz.de/comments/permalink/37765918), [6](https://www.mydealz.de/comments/permalink/38138143))  
\- USB Stick bootet nicht? Secure Boot im BIOS-Setup deaktivieren ([1](https://www.mydealz.de/comments/permalink/37570618))  
\- Nach HomeAssistant Installation wird SSD nicht als Bootoption aufgelistet ([1](https://www.mydealz.de/comments/permalink/37574050), [2](https://www.mydealz.de/comments/permalink/37592239), [3](https://www.mydealz.de/comments/permalink/37765918))  
\- Bei HomeAssistant muss sda1, nicht sda angegeben werden ([1](https://www.mydealz.de/comments/permalink/37599273))  
\- Nach pfSense / OPNsense Installation wird SSD nicht als Bootoption aufgelistet ([1](https://www.mydealz.de/comments/permalink/37671080), [2](https://www.mydealz.de/comments/permalink/38189753))  
\- Nach Ubuntu Installation wird SSD nicht als Bootoption aufgelistet ([1](https://www.mydealz.de/comments/permalink/37621105))  
\- Alpine Linux hat nicht gebootet ([1](https://www.mydealz.de/comments/permalink/37677089))  
\- Batocera bootet nicht von SSD ([1](https://www.mydealz.de/comments/permalink/37733091))  
\- LibreElec bootet nicht von SSD ([1](https://www.mydealz.de/comments/permalink/37798683), [2](https://www.mydealz.de/comments/permalink/38137111))  
\- Schaltet nach paar Sekunde wieder aus ohne etwas zu booten ([1](https://www.mydealz.de/comments/permalink/37580346), [2](https://www.mydealz.de/comments/permalink/37589012), [3](https://www.mydealz.de/comments/permalink/37986129))  
\- Fehlende Treiber unter Windows ([1](https://www.mydealz.de/comments/permalink/37637491), [2](https://www.mydealz.de/comments/permalink/37656540), [3](https://www.mydealz.de/comments/permalink/37899015), [4](https://www.mydealz.de/comments/permalink/38101894))  
\- SSD Schraube lässt sich nicht lösen ([1](https://www.mydealz.de/comments/permalink/37621349), [2](https://www.mydealz.de/comments/permalink/37824521), [3](https://www.mydealz.de/comments/permalink/37959613))  
\- Von 16GB RAM Riegeln wird scheinbar nur Dual Rank unterstützt (8 Chips pro Seite) und kein Single Rank (4 Chips pro Seite), von kleineren Größen werden wohl aber auch Single Rank Riegel unterstützt ([1](https://www.mydealz.de/comments/permalink/37675998))  
\- Wildwiedergabe unter Windows 11 sehr langsam ([1](https://www.mydealz.de/comments/permalink/37691439))  
\- WiFi USB Dingle funktionieren nicht unter Chrome OS Flex ([1](https://www.mydealz.de/comments/permalink/37699063))  
\- SATA Adapter funktioniert nicht im M2 Port ([1](https://www.mydealz.de/comments/permalink/37687195))  
\- WoL funktioniert nicht ([1](https://www.mydealz.de/comments/permalink/37712773), [2](https://www.mydealz.de/comments/permalink/37716676))  
\- Adguard Home funktioniert nicht ([1](https://www.mydealz.de/comments/permalink/37713825))  
\- BIOS Version aktualisiert sich nicht nach Update ([1](https://www.mydealz.de/comments/permalink/37764927))  
\- Schlechte Audioqualität ([1](https://www.mydealz.de/comments/permalink/37765045), [2](https://www.mydealz.de/comments/permalink/37974674))  
\- iGPU lässt sich nicht mit Windows VM in Proxmox benutzen ([1](https://www.mydealz.de/comments/permalink/37779177))  
\- EndeavourOS flackernder Bildschirm ([1](https://www.mydealz.de/comments/permalink/37814055))  
\- LAN-Karte im M.2 WiFi Port (A/E-Key) funktioniert nicht ([1](https://www.mydealz.de/comments/permalink/37791852))  
\- Win10 IOT „bitte warten“ Schleife, Apps funktionieren nicht ([1](https://www.mydealz.de/comments/permalink/37847344))  
\- ConBee USB Zigbee Stick disconnected stündlich in Proxmox & Debian ([1](https://www.mydealz.de/comments/permalink/37856049))  
\- Ethernet funktioniert nicht mehr ([1](https://www.mydealz.de/comments/permalink/37873460))  
\- Proxmox Meldung "You do not have a valid Subscription" ([1](https://www.mydealz.de/comments/permalink/37898869))  
\- Batocera stürzt ab wenn Monitor ohne Lautsprecher angeschlossen ist ([1](https://www.mydealz.de/comments/permalink/37959699))  
\- Netzwerkprobleme unter Debian 11 ([1](https://www.mydealz.de/comments/permalink/37987037))  
\- 1Gbit LAN-Karte wird als 100Mbit Karte angezeigt ([1](https://www.mydealz.de/comments/permalink/38133018))  
\- interner USB-C Header wird unter Proxmox nicht erkannt ([1](https://www.mydealz.de/comments/permalink/38032107))  
\- Netzwerkprobleme unter Proxmox ([1](https://www.mydealz.de/comments/permalink/38016672))  
\- Wifi funktioniert nicht unter Proxmox ([1](https://www.mydealz.de/comments/permalink/38029244))  
\- Linux bootet nach BIOS Update (14.10.2022) nicht ([1](https://www.mydealz.de/comments/permalink/38054730))  
\- BIOS Update von USB Stick findet keine Datei ([1](https://www.mydealz.de/comments/permalink/38076547))  
\- Audio gibt nur Stereo aus ([1](https://www.mydealz.de/comments/permalink/38065001))  
\- Audio Passthrough funktioniert nicht ([1](https://www.mydealz.de/comments/permalink/38075215))  
\- USB Festplatten gehen nicht auf Standby unter Proxmox ([1](https://www.mydealz.de/comments/permalink/38085198))  
\- K3OS bootet nicht ([1](https://www.mydealz.de/comments/permalink/38132574))  
\- Video/Audio Passthrough funktioniert in Proxmox (mit Libreelec/Kodi) nicht ([1](https://www.mydealz.de/comments/permalink/38190848))  
\- Windows 11 USB Stick bootet nicht ([1](https://www.mydealz.de/comments/permalink/38202930))  


## Pictures 

\- [Innenleben](https://www.mydealz.de/comments/permalink/37555659)  
\- [2280 SSD mit 2230 WiFi-Karte gleichzeit eingebaut](https://www.mydealz.de/comments/permalink/37562446)  
\- [Mainboard Layout & interne Anschlüsse](https://www.mydealz.de/comments/permalink/37574631) (manche davon sind nicht bestückt!)  
\- [2,5“ SSD im Gehäuse untergebracht](https://www.mydealz.de/comments/permalink/37666881)  
\- [4-fach SATA Adapter in M.2 Slot](https://www.mydealz.de/comments/permalink/37880720)  
\- WiFi Antennen nachrüsten ([1](https://www.mydealz.de/comments/permalink/37705901), [2](https://www.mydealz.de/comments/permalink/37812712))  
\- [PowerDelivery Powerbank als USV](https://www.mydealz.de/comments/permalink/37733114)  
\- [Stifte auf denen M2 Module geschraubt sind, sind gelötet, nicht geschraubt](https://www.mydealz.de/comments/permalink/37737490)  
\- [2. LAN-Buchse anstelle des RS232-Ports eingebaut](https://www.mydealz.de/comments/permalink/37993363)  
\- [USB-C nachgerüstet](https://www.mydealz.de/comments/permalink/38001225)  
\- [Platzierung des bei manchen „abgefallenem Aluröhrchen“](https://www.mydealz.de/comments/permalink/38049356)  
\- [Zweite M.2 SSD mit Adapter im M.2 WiFi Slot](https://www.mydealz.de/comments/permalink/38096778)  
\- [Zwei 2,5“ SSDs außen angebracht](https://www.mydealz.de/comments/permalink/38159297)  
\- [nachgelöteter SATA Port](https://imgur.com/a/TAmADFS)  


