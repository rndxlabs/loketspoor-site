Taak: loketspoor-site

# CLAUDE.md

Statische website voor loketspoor.nl. Gewone HTML en CSS in `public/`, zonder build-stap en zonder `package.json`. Hosting via Netlify; instellingen, doorverwijzingen en beveiligingsheaders staan in `netlify.toml`.

## Vaste regels

- Geen scripts, cookies, tracking of analytics, en geen formulieren.
- Geen externe bronnen: geen lettertypen, scripts, stylesheets of afbeeldingen van andere websites. Alleen de mailto-links en de link naar de Autoriteit Persoonsgegevens gaan naar buiten.
- Alle opmaak staat in `public/style.css`. Geen `style=`-attributen en geen `<style>`- of `<script>`-blokken: de Content-Security-Policy blokkeert die.
- Geen prijzen, geen klantnamen, geen inlogknop en geen links naar omgevingen van klanten.
- Geen functies noemen die nog niet live zijn.
- Dit is een openbare repo: niets interns. Geen geheimen, geen persoonlijke paden, geen verwijzingen naar interne repo's, issues of documenten.
