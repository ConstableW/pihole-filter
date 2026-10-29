# pihole-filter

Gepflegte Blocklisten für Pi-hole und andere DNS-Filter, nach Themen sortiert. Jede Datei in `lists/` ist eine eigene Liste im Domain-Format (eine Domain pro Zeile).

## Listen

| Liste | Inhalt |
|---|---|
| `werbung` | Werbung, Tracker, Pop-ups, Referral-Tracking |
| `malware` | Malware, Phishing, Betrug, Fake-Shops |
| `nsfw` | Pornografie und Erotik |
| `gluecksspiel` | Online-Casinos, Sportwetten, Poker |
| `smarttv` | Samsung- und andere Smart-TV-Tracker, Update-Server |
| `tiktok` | TikTok-Domains |
| `umgehung` | DoH-, VPN- und Proxy-Dienste, mit denen sich Filter umgehen lassen |
| `amazon`, `winoffice`, `xiaomi` | Geräte-Telemetrie (greift tief ein, im Zweifel prüfen) |
| `safesearch`, `spam-tlds`, `urlshortener`, `social`, `piraterie`, `dyndns`, `hoster` | Optionale Listen, die tiefer eingreifen |

Jede Datei nennt im Kopf ihre Quellen, den Stand und die Lizenz.

## Einbinden

In Pi-hole unter *Adlists* die Raw-Adresse der gewünschten Liste eintragen, zum Beispiel:

```
https://raw.githubusercontent.com/ConstableW/pihole-filter/main/lists/werbung.txt
```

Die Listen sperren nur die aufgeführten Namen, keine Subdomains. Das ist eine Eigenschaft von Pi-hole-Adlists.

## Lizenz

Das Repository steht unter GPL-3.0 (siehe `LICENSE`), weil die Listen Daten von HaGeZi und OISD (beide GPL-3.0) enthalten. Quellen, Lizenzen und vorgenommene Änderungen: `NOTICE.md`.
