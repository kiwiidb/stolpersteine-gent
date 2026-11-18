# Struikelstenen van Gent — Stolpersteine of Ghent

A full-screen, map-based memorial for the **Stolpersteine** (*struikelstenen*) of Ghent, Belgium.

Each small brass cobblestone is laid in front of the last freely chosen home of a person
persecuted by the Nazi regime — resistance fighters, political prisoners and Jewish
neighbours who were deported and murdered between 1940 and 1945. Tap any stone on the map
to see a photograph and read who lived there, and what became of them.

## Features

- Full-screen OpenStreetMap (Leaflet + CARTO Voyager tiles) tinted in a sombre
  WW2-resistance / noir aesthetic.
- 35 Stolpersteine across Ghent and its *deelgemeenten* (Drongen, Mariakerke, Zwijnaarde,
  Ledeberg …).
- Brass "stone" markers with the person's initials; click/tap to open a side panel with
  a photograph, a short biography, and the original Dutch inscription rendered as a plaque.
- Fully static — no build step, no backend.

## Data & attribution

- Stolpersteine list, inscriptions and photographs: **Wikipedia** ("Lijst van Stolpersteine
  in Vlaanderen") and **Wikimedia Commons**, available under their respective licences.
- Coordinates geocoded from street addresses via **OpenStreetMap / Nominatim**.
- Base map tiles: **OpenStreetMap** contributors & **CARTO**.

Biographical summaries are generated from the Dutch inscriptions on the stones. The data may
be incomplete — the Stolpersteine project is ongoing.

## Develop locally

```bash
python3 -m http.server 8000 --directory public
# open http://localhost:8000
```

## Deploy

Static site served from `public/`. Deploys to Vercel out of the box.

---

*“A person is only forgotten when their name is forgotten.”*
