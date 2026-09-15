# Wahapedia mirror

A copy of the CSV tables Wahapedia publishes, one directory per game system. Each directory holds the
tables under the names the export uses (`Datasheets.csv`, `Stratagems.csv` and the rest), plus a
`meta.json` recording when they were fetched and where they came from.

The copy exists so a browser can read them. `wahapedia.ru` sends no `Access-Control-Allow-Origin`
header, and `raw.githubusercontent.com` does.

## Attribution

Powered by Wahapedia — https://wahapedia.ru

The tables are Wahapedia's own export, passed through unchanged. The rules, points and names in them
are copyright Games Workshop. Wahapedia asks that the line above travels with the data, so it is
repeated in every copy of this dataset.

## How it is refreshed

Weekly, by `.github/workflows/wahapedia.yml` in [Grimstat](https://github.com/N041M/Grimstat),
which runs `pnpm cli mirror` and pushes the result here. Nothing else is committed to this
repository by hand.
