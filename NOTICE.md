# Lizenzen und Quellen

Die Listen in `deny/` sind zusammengefuehrte, deduplizierte und angepasste Fassungen fremder Blocklisten, ergaenzt um eigene Eintraege und bereinigt um freigestellte Domains. Die Allowlists in `allow/` sind eigene Zusammenstellungen. Jede Datei nennt im Kopf ihre Quellen und den Stand der Aenderung.

Weil die Listen Daten von HaGeZi (GPL-3.0) enthalten, steht dieses Repository insgesamt unter der **GNU General Public License v3.0** (siehe `LICENSE`). Eigene Aenderungen: ConstableW.

## Quellen, die in `lists/` eingeflossen sind

| Quelle | Lizenz | Inhalt |
|---|---|---|
| [HaGeZi DNS Blocklists](https://github.com/hagezi/dns-blocklists) | GPL-3.0 | Werbung, Malware, NSFW, Glücksspiel, Smart-TV, TikTok, Umgehung und optionale Listen |
| [OISD](https://oisd.nl) | GPL-3.0 (laut oisd.nl/faq und LICENSE im Repo sjhgvr/oisd) | OISD big |
| [StevenBlack/hosts](https://github.com/StevenBlack/hosts) | MIT | Unified Hosts, Porn-only |
| [Perflyst/PiHoleBlocklist](https://github.com/Perflyst/PiHoleBlocklist) | MIT | SmartTV-Liste |
| [oneoffdallas/dohservers](https://github.com/oneoffdallas/dohservers) | MIT | DoH-Server |

Vorgenommene Aenderungen: Zusammenfuehren je Thema, Entfernen von Duplikaten, Entfernen freigestellter Domains, Ergaenzung eigener Eintraege.

## Quellen, die bewusst NICHT gespiegelt werden

Diese Quellen sind nicht Teil der Listen. Ihre Lizenz erlaubt die Weitergabe in dieser Form nicht, deshalb steht ihr Inhalt nicht in diesem Repository.

| Quelle | Grund |
|---|---|
| Firebog RPiList-Malware | Quelle RPiList/specials steht unter CC BY-NC 4.0; die Nicht-kommerziell-Klausel ist mit GPL-3.0 nicht vereinbar |
| wassname Samsung-Smart-TV-Gist | Gist ohne Lizenzangabe, keine Weitergabe erlaubt |

## MIT-Lizenztexte der eingeflossenen Quellen

### StevenBlack/hosts

```
The MIT License (MIT)

Copyright © 2026 Steven Black

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the “Software”), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do
so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

```

### Perflyst/PiHoleBlocklist

```
MIT License

Copyright (c) 2018 Perflyst

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```

### oneoffdallas/dohservers

```
MIT License

Copyright (c) 2019 Dallas Haselhorst

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

```
