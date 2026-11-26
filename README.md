# RVDIOVCTIVE site (review build)

The RVDIOVCTIVE public site: landing page, photo archive, events, label and merch.
It's a static site with no build step. Open `index.html` through any web server and it runs.

## What's in here

| Path | What it is |
|---|---|
| `index.html` | The whole site: layout, styles and code |
| `data.json` | Nights in the photo archive (event, date, venue, city, photo list) |
| `rel.json` | Label releases (from the LabelWorx export) |
| `f/` | One flyer per night |
| `tp/`, `lp/` | Photos, packed one file per night (`tp` = grid size, `lp` = large) |
| `rel/` | Release artwork |

## Social links

The Instagram, Beatport and Resident Advisor links live in one place near the top of the script in `index.html` (`const LINKS`). Leave one empty and its icon disappears.

## Still to do before launch

- Final photo selection from the Photo Vault (replaces `data.json`, `tp/`, `lp/`)
- Missing label artwork and Beatport links
- Real events (the three upcoming parties are samples, toggled in the top bar)
- Real merch photos, prices and store links (currently demo items)
- Remove the `noindex` line in `index.html`, and switch the preview-image URLs to the real domain

## Preview locally

```
python3 -m http.server 8000
```
then open http://localhost:8000
