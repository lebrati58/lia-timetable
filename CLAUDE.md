# CLAUDE.md — המערכת של ליה

Petit emploi du temps scolaire, **mobile, en hébreu RTL**. Il affiche les matières, les professeurs et les salles de chaque jour (du dimanche au vendredi, 9 heures de cours).

## Fichiers
- `index.html` : la page.
- `schedule.js` : les données (`BASE_SCHEDULE` par jour, `PERIOD_TIMES` pour les horaires).
- `app.js` : l'affichage et l'éditeur. Les modifications sont enregistrées **sur le téléphone seulement** (localStorage `liaScheduleOfficialNov2026V2`) et ne sont pas synchronisées.
- `manifest.webmanifest` : installation sur l'écran d'accueil.

Le site est statique et sans build, publié par GitHub Pages depuis `main` : https://lebrati58.github.io/lia-timetable/

## Règles de travail
- Les données ont été recopiées à la main depuis une photo. Certaines salles et certains cours de groupe sont incertains : ne présente jamais l'appli comme l'emploi du temps officiel de l'école.
- Si tu modifies la structure de `BASE_SCHEDULE`, **change la clé localStorage**. Sinon les anciennes modifications enregistrées sur le téléphone écrasent les nouvelles données.
- Tout texte reste en hébreu simple, en gros caractères, lisible sur un téléphone.
- Vérifie l'affichage en largeur téléphone (375 px) avant de publier. « **yallah** » veut dire : fusionne dans `main`, puis vérifie la publication.
