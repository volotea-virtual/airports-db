# ✈️ Public airports database

GitHub based API service

[![DB Update](https://github.com/Haugaland-Flyklubb/airports-db/actions/workflows/node.js.yml/badge.svg)](https://github.com/Haugaland-Flyklubb/airports-db/actions/workflows/node.js.yml)

This is a JSON database of airports which contains about 56k airports with their runways, communication frequencies,
navaids, countries, and regions information. The database is not 100% accurate because can have older data, so do not use it for a real flight or very sensitive applications.
But it works well to get basic information about the airport.

## How to use it? 🤔

> John F Kennedy International Airport [KJFK](https://github.com/Haugaland-Flyklubb/airports-db/blob/master/icao/KJFK.json)

The main idea of this repository is to get the `JSON` data about the airport by using its ICAO code.
Every airport has its own JSON file placed in [icao](https://github.com/Haugaland-Flyklubb/airports-db/tree/master/icao) directory.

So, to get the information about the airport use the following url:

`https://raw.githubusercontent.com/Haugaland-Flyklubb/airports-db/master/icao/<enter your ICAO>.json`

> ICAO code must be in uppercase

For example

```bash
  curl https://raw.githubusercontent.com/Haugaland-Flyklubb/airports-db/master/icao/KJFK.json
```

If airport is not found, the 404 status code is returned.

Have ideas on how to improve it? Feel free to share it on the [GitHub Issues](https://github.com/Haugaland-Flyklubb/airports-db/issues).

Data is based on [ourairports.com](https://ourairports.com/) database. You can download the raw CSV files from [raw](https://github.com/Haugaland-Flyklubb/airports-db/tree/master/raw) directory.
The repository will be updated automatically every day at 7:00 UTC. You can get the latest CSV files here: [https://ourairports.com/data/](https://ourairports.com/data/)
