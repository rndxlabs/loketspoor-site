# loketspoor-site

De website op [loketspoor.nl](https://loketspoor.nl): een korte pagina over Loketspoor, CRM-software van RNDX Labs BV voor ondernemersloketten, ondernemersverenigingen en gemeenten, met een privacyverklaring.

Gewone HTML en CSS in `public/`, zonder build-stap. De site gebruikt geen scripts, cookies, tracking of externe bronnen.

## Lokaal bekijken

```sh
python3 -m http.server -d public
```

Open daarna http://localhost:8000.

## Deploy via Netlify

Netlify is gekoppeld aan deze repo en publiceert elke push naar `main`. Er is geen build-commando: Netlify publiceert de map `public`. In `netlify.toml` staan verder de doorverwijzingen (`www.loketspoor.nl` en het netlify.app-adres gaan met een 301 naar `https://loketspoor.nl`) en de beveiligingsheaders.

## security.txt verlengen

`public/.well-known/security.txt` verloopt op 30 september 2027 (het veld `Expires`). Zet vóór 2027-09-30 een nieuwe datum, hoogstens een jaar vooruit, en push de wijziging.
