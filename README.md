# pihole-filter

Gepflegte Blocklisten und Allowlists für Pi-hole und andere DNS-Filter, nach Themen sortiert. Jede Datei ist eine eigene Liste im Domain-Format (eine Domain pro Zeile).

## `deny/` – Blocklisten

| Liste | Inhalt |
|---|---|
| `werbung` | Werbung, Tracker, Pop-ups, Referral-Tracking |
| `malware` | Malware, Phishing, Betrug, Fake-Shops |
| `nsfw` | Pornografie und Erotik |
| `gluecksspiel` | Online-Casinos, Sportwetten, Poker |
| `smarttv` | Samsung- und andere Smart-TV-Tracker, Update-Server |
| `tiktok` | TikTok-Domains |
| `firetv` | Werbung, Analyse und Tracking von Amazon Fire TV |
| `umgehung` | DoH-, VPN- und Proxy-Dienste, mit denen sich Filter umgehen lassen |
| `amazon`, `winoffice`, `xiaomi` | Geräte-Telemetrie (greift tief ein, im Zweifel prüfen) |
| `safesearch`, `spam-tlds`, `urlshortener`, `social`, `piraterie`, `dyndns`, `hoster` | Optionale Listen, die tiefer eingreifen |

## `allow/` – Allowlists

Freigaben gegen Fehlblockaden, zum Beispiel für Lotto und Eurojackpot, die von der Glücksspielliste getroffen würden, oder für Dienste wie Discord. Die Allowlists sind so gebaut, dass die Domains darin in den Blocklists dieses Repos nicht mehr vorkommen.

Jede Datei nennt im Kopf ihre Quellen, den Stand und die Lizenz.

## Einbinden

In Pi-hole (ab Version 6) unter *Adlists* die Raw-Adresse eintragen. Blocklisten als „Blocklist", Allowlists als „Allowlist":

```
https://raw.githubusercontent.com/ConstableW/pihole-filter/main/deny/werbung.txt
https://raw.githubusercontent.com/ConstableW/pihole-filter/main/allow/lotto.txt
```

Die Listen enthalten nur die aufgeführten Namen, keine Subdomains. Das ist eine Eigenschaft von Pi-hole-Adlists.

## Lizenz

Das Repository steht unter GPL-3.0 (siehe `LICENSE`), weil die Listen Daten von HaGeZi und OISD (beide GPL-3.0) enthalten. Quellen, Lizenzen und vorgenommene Änderungen: `NOTICE.md`.
