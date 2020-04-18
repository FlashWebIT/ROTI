# 🚇🚞🚌 Romanian Open Transit Initiative 🚋🚈🚡
## 📝 Project and resource list

1. ### 📎 Data sources
####  _(structured / processable data) There has to be a starting point :)_
* [Passenger railway operators static timetable, published anually, XML format](https://data.gov.ro/organization/sc-informatica-feroviara-sa)
* [Iași urban transit: GPS positions in real-time, JSON](https://gps.sctpiasi.ro/json)
* [Bucharest urban transit: lines, stations, departures in real time, timetables, GPS positions](https://info.stbsa.ro/rp/api/lines/)
<details>
  <summary>Details</summary>
  
  ```
  https://info.stbsa.ro/rp/api/lines/
  https://info.stbsa.ro/rp/api/lines/:line_id/
  https://info.stbsa.ro/rp/api/lines/:line_id/direction/:direction_id
  https://info.stbsa.ro/rp/api/lines/:line_id/stops/:stop_id?lang=:lang_code
  https://info.stbsa.ro/rp/api/lines/:line_id/vehicles/:direction_id
  https://info.stbsa.ro/rp/api/notifications
  ```
  
  segment_path line shape is to be decoded with https://github.com/jieter/Leaflet.encoded
</details>

  * [Constanța urban transit: lines, stations, departures in real time, timetables, GPS positions](https://info.ctbus.ro/rp/api/lines/)

<details>
  <summary>Details</summary>
  
  ```
  https://info.ctbus.ro/rp/api/lines/
  https://info.ctbus.ro/rp/api/lines/:line_id/
  https://info.ctbus.ro/rp/api/lines/:line_id/direction/:direction_id
  https://info.ctbus.ro/rp/api/lines/:line_id/stops/:stop_id?lang=:lang_code
  https://info.ctbus.ro/rp/api/lines/:line_id/vehicles/:direction_id
  https://info.ctbus.ro/rp/api/notifications
  ```
  
  segment_path line shape is to be decoded with https://github.com/jieter/Leaflet.encoded
</details>

* [Sibiu local urban transit operator GTFS (Official)](https://www.tursib.ro/trasee/gtfs)

---
2. ### ⚙️ Data converters
#### _(exporters, processors etc.) From proprietary to standard/open formats_
* [Railway XML data to GTFS, Ruby](https://github.com/vasile/data.gov.ro-gtfs-exporter) - also includes a very handy [GeoJSON file of all Romanian railway stations with names and GPS positions](https://raw.githubusercontent.com/vasile/data.gov.ro-gtfs-exporter/master/cfr.webgis.ro/stops.geojson)
* [Real time railway data (train departures, delays, platform numbers updated minutely) to JSON API and WebUI - Python](https://github.com/FlashWebIT/cfr-iris-scraper)
* [Generate up-to-date GTFS files from custom local transit API used by Bucharest & Constanța (RADCOM)](https://github.com/FlashWebIT/Bucharest-GTFS-exporter)
* [GTFS Realtime protocol buffer vehicle positions converter for Iași](https://github.com/FlashWebIT/Iasi-GTFS-Realtime-Vehicle-Positions)
* [GTFS Realtime protocol buffer vehicle positions converter for Bucharest & Constanța](https://github.com/FlashWebIT/Bucharest-Constanta-GTFS-Realtime-Vehicle-Positions)
* _[Static GTFS exporter for Iași](https://github.com/FlashWebIT/Iasi-GTFS-exporter)_ - This is still a work in progress and **currently only exports frequency-based  routes and is buggy**.

---
3. ### 🗺️ Data visualizers
#### _(maps, apps etc.) Make it beautiful_
* [GTFS transit-map simulation](https://github.com/vasile/transit-map) - static webapp, also needs [GTFS-viz Ruby converter to GeoJSON](https://github.com/vasile/GTFS-viz)
* [Real time train information - Cordova Android app](https://github.com/BodoMinea/InfoTren)

---

### ⁉️ WTF Zone - We don't know what this is but it belongs here
* [Some attempt at an GTFS backend by GovITHub](https://github.com/gov-ithub/infotranspub-backend)
<details>
  <summary>Historical?</summary>
  Not relevant as data or install guides anymore, but interesting study materials on past projects:
  * https://github.com/cnicules/OTP-Buh/wiki (also check the code!)
</details>

### 📥 Download center
#### 🚍 Grab some ready-made GTFS Files
* National Railway (converted): [Download here](https://github.com/vasile/data.gov.ro-gtfs-exporter/tree/master/gtfs-out)
* Local transit, Bucharest & Constanța (generated/converted): [Download here](https://github.com/FlashWebIT/Bucharest-GTFS-Exporter/tree/master/output)
* Local transit, Iași (generated/converted): [Download here](https://github.com/FlashWebIT/Iasi-GTFS-Exporter/tree/master/output)
* Local transit, Sibiu (official): [Download here](https://www.tursib.ro/trasee/gtfs)

### 🕬 Contribute
By [pull request](CONTRIBUTING.md) or by [opening an issue](https://github.com/FlashWebIT/ROTI/issues/new).

### 📧 Get in touch
Email the maintainer at bogdan@transportpublic.ro

### 📅 Milestones
- [ ] Get a few other developers onboard (2-3 for this year)
- [ ] [Roll out](https://digitransit.fi/en/developers/) our own instance of the beautiful [Digitransit](https://github.com/HSLdevcom/digitransit/blob/master/Installation.md) trip-planning webapp, fully open source Finnish software which [works for them in production](https://reittiopas.hsl.fi/) and also [at nation-level](https://opas.matka.fi/)
<details>
  <summary>Get a sneak peek</summary>  

![Screenshot](https://github.com/FlashWebIT/Bucharest-GTFS-Exporter/raw/master/OTP.png "Screenshot")
![Screenshot](https://github.com/FlashWebIT/Bucharest-GTFS-Exporter/raw/master/OTP2.png "Screenshot")
</details>
