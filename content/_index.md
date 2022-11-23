+++
title = "Home"
weight = 1
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
[hardware overview]({{< ref "hardware" >}})

[firmware]({{< ref "hardware/firmware" >}})

3 - Windows / Linux  
&nbsp;&nbsp;3.2 Desktop Betriebssysteme  
4 - Mods  
5 - Stromverbrauch  
6 - Gemeldete Probleme  
7 - Links  
8 - Bilder 


### 1.1 - Overview  

Der Futro S740 ist ein Thinclient aus 2018 mit einem mSTX D3544-A Mainboard, welcher eine abgespackte Version des Kontron D3544-S2 mit dem dazugehörigen Smartcase S500 aus gleichem Hause ist.  
Anders wie ältere Thinclients wird der Futro nicht nur vorgesehen über Fernzugriff sich mit einem Server zu verbinden, auf dem dann Software ausgeführt wird, sondern hat der Futro genug Rechenleistung um als eigenständiger Mini PC zu laufen.



## 4 - Mods  

\- Gehäuse lässt sich öffnen indem die 2 Schrauben an der IO-Blende entfernt werden, dann lässt sich die obere Gehäusehälfte nach hinten schieben & abnehmen  
\- unbestückten RS232 Seriell-Port nachlöten ([1](https://www.mydealz.de/comments/permalink/38079460))  
\- 2x unbestückte SATA Ports nachlöten (es müssen zusätzlich je 4x 0402 10nF SMD Kondensatoren nachgelötet werden) ([1](https://www.mydealz.de/comments/permalink/38114275))  

## 5 - Stromverbrauch  

Der Unterschied in Effizienzklasse rechtertigt meist nicht den Kauf eines besseren Netzteiles, allerdings hatte ich bereits Netzteile vom Vorgänger des S740 die nahezu doppelt so viel Strom verbrauchten (wahrscheinlich durch defekt wegen Alter) als sie sollten. Dann wiederum hatte ich auch ein billiges Noname 12V Netzteil das minimal sogar besser abgeschnitten hat als das Original von Fujitsu.  
Wem der Stromverbrauch wichtig ist sollte sich ein verlässliches Energiemessgerät anschaffen (PM231e, KD-203, ELV Energy Master), da billigere Varianten um mehrere Watt ungenau sind.  

> Tipp: Wer trotzdem ein neues Netzteil braucht, Leicke Netzteile sind am beliebtesten für ihre Effizienz.  

\- Liste mit gemessen Energieverbrauchswerten [>>hier<<](https://github.com/R3NE07/Futro-S740/blob/main/power_consumption.md)

## 6 - Gemeldete Probleme  

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


## 7 - Links  

\- [D3544-S Mainboard Datenblatt von Kontron](https://www.kontron.com/download/download?filename=/downloads/datasheets/d/d3544-s-mstx_20210129_datasheet.pdf&product=157718) (ähnlich dem D3544-A aus dem S740)  
\- [Fujitsu Futro S740 Datenblatt](https://manualzz.com/doc/62121610/fujitsu-futro-s740-manual)  
\- [Vergleich eines Raspberry Pi 4 VS. Intel J4105 System](https://uni.hi.is/helmut/2021/06/07/power-consumption-of-raspberry-pi-4-versus-intel-j4105-system/)  
\- [WiFi Geschwindigkeitstest](https://www.mydealz.de/comments/permalink/37694659)  
\- [passende M2 SATA SSDs auf Geizhals suchen](https://geizhals.de/?cat=hdssd&xf=252_120%7E4832_4)  
\- [Batocera auf internem Speicher installieren](https://www.mydealz.de/comments/permalink/37581112)  
\- [Proxmox Helper Scripts](https://tteck.github.io/Proxmox/)  
\- [Offizielle Downloadseite für Treiber, BIOS Update, PDFs](https://support.ts.fujitsu.com/IndexDownload.asp?lng=de&OpenTab=)  
\- [Thread über Proxmox VS. Docker](https://www.mydealz.de/comments/permalink/37675393)  
\- 3D gedruckter Standfuß ([1](https://www.thingiverse.com/thing:5529474), [2](https://www.printables.com/de/model/288427-fujitsu-futro-s740-feets), [3](https://www.printables.com/de/model/284749-base-stand-for-fujitsu-futro-s740))  
\- [3D gedruckter VESA-Mount Adapter](https://www.printables.com/de/model/287058-vesa-monitor-mount-adapter-plate-for-fujitsu-futro)  
\- [[Video] Kipper auf S740 installieren um 3D Drucker zu steuern](https://www.youtube.com/watch?v=bUENy-sOL9c)  
\- [Nextcloud mit Reverse Proxy installieren (auf Nginx/Proxmox)](https://www.schreiners-it.de/nextcloud/nextcloud-hinter-reverse-proxy-installieren/)  
\- [3D Modelle](http://sp-it.net/index.php?option=com_content&view=article&id=1566&Itemid=140&jsmallfib=1&dir=JSROOT/drivers/fujitsu/Products/Mainboards/Industrial-und-ExtendedLifetime/D3544-S_Mini-STX/Mechanics-und-3D#/div--div-download)  
\- [Jedes Linux System mit powertop & cpu-governor optimieren](https://www.mydealz.de/comments/permalink/37740815)  
\- [Liste mit Software zum selbst hosten](https://www.reddit.com/r/selfhosted/comments/bsp01i/welcome_to_rselfhosted_please_read_this_first/)  
\- [[Video] Einfach pi-Hole in Proxmox installieren](https://youtu.be/_O7kRBEu6T0)  
\- [Proxmox installieren & Backups von Containern automatisch anlegen](https://decatec.de/home-server/proxmox-ve-installation-und-grundkonfiguration/#Installation)  
\- [„M.2 for Hackers“ - Hackaday Article](https://hackaday.com/2022/10/27/m-2-for-hackers-expand-your-laptop/)  
\- [Passmark Benchmark](https://www.mydealz.de/comments/permalink/37607626)  
\- [CPU Benchmark mit anderen CPUs vergleichen](https://www.cpubenchmark.net/compare/BCM2711-vs-Intel-Celeron-J4105/4297vs3159)  
\- HardwareLuxx Threads über Stromsparende Systeme ([<30W](https://www.hardwareluxx.de/community/threads/die-sparsamsten-systeme-30w-idle.1007101/), [<10W](https://www.hardwareluxx.de/community/threads/alltagstaugliche-desktop-systeme-mit-10w-idle-verbrauch-inkl-llano-fm1-beispiel.799083/), [<6W](https://www.hardwareluxx.de/community/threads/alltagstaugliche-desktop-systeme-mit-6w-idle-verbrauch-inkl-haswell-beispiel.1001484/))  

## 8 - Bilder 

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


