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

---
2. ### ⚙️ Data converters
#### _(exporters, processors etc.) From proprietary to standard/open formats_
* [Railway XML data to GTFS, Ruby](https://github.com/vasile/data.gov.ro-gtfs-exporter)
* [Real time railway data (train departures, delays, platform numbers updated minutely) to JSON API and WebUI - Python](https://github.com/FlashWebIT/cfr-iris-scraper)
* [Generate up-to-date GTFS files from custom local transit API used by Bucharest & Constanța (RADCOM)](https://github.com/FlashWebIT/Bucharest-GTFS-exporter)

---
3. ### 🗺️ Data visualizers
#### _(maps, apps etc.) Make it beautiful_
* [GTFS transit-map simulation](https://github.com/vasile/transit-map) - static webapp, also needs [GTFS-viz Ruby converter to GeoJSON](https://github.com/vasile/GTFS-viz)
* [Real time train information - Cordova Android app](https://github.com/BodoMinea/InfoTren)

---

### ⁉️ WTF Zone - We don't know what this is but it belongs here
* [Some attempt at an GTFS backend by GovITHub](https://github.com/gov-ithub/infotranspub-backend)

### 📥 Download center
#### 🚍 Grab some ready-made GTFS Files
* National Railway: [Download here](https://github.com/vasile/data.gov.ro-gtfs-exporter/tree/master/gtfs-out)
* Local transit, Bucharest & Constanța: [Download here](https://github.com/FlashWebIT/Bucharest-GTFS-Exporter/tree/master/output)

### 🕬 Contribute
By pull request or by opening an issue.
