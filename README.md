# Salle Opé

Prototype de jeu de régulation des secours dans le navigateur. Le joueur tient la plateforme commune de Nice et de sa région : il décroche les appels 15, 17, 18 et 112, pose les questions, qualifie l'intervention, interconnecte les services et engage les moyens sur la carte.

Tout tient dans `index.html` : il suffit de l'ouvrir dans un navigateur.

## Ce que contient le prototype

- Une carte réelle (Leaflet) avec les limites communales IGN autour de Nice.
- La zone police nationale (Nice, Saint-Laurent-du-Var, Cagnes-sur-Mer, Villefranche-sur-Mer) et la gendarmerie partout ailleurs.
- 37 bases et 57 moyens : pompiers, SAMU 06, police, 13 brigades de gendarmerie.
- 14 scénarios et un débriefing noté sur 100 : pertinence des moyens, délais, questionnement, coordination.

Le code est découpé en sections numérotées : réglages, monde, services, scénarios, état, simulation, score, interface, carte, boucle principale. Pour ajouter un scénario, recopier un bloc du tableau `SCENARIOS`.

## Limites connues

- Le réseau routier est simplifié : il ne contient pas encore les rues OpenStreetMap.
- Certaines implantations sont supposées, notamment les casernes de Cagnes, Carros, Levens, Contes et Vence. Les ambulances privées sont fictives.
- Ceci est un jeu. En cas d'urgence réelle, composez le 15, le 17, le 18 ou le 112.

## Crédits

- Limites communales : IGN Admin Express 2018, Licence Ouverte Etalab, via [france-geojson](https://github.com/gregoiredavid/france-geojson).
- Cartographie : [Leaflet](https://leafletjs.com) 1.9.4, licence BSD-2-Clause.
- Polices : Barlow Condensed, IBM Plex Sans et IBM Plex Mono (Google Fonts, SIL Open Font License).
