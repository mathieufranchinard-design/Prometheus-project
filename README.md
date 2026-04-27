TP prometheus

 # Projet d'observabilité – Prometheus / Docker / Python API

## Présentation

Ce projet avait pour objectif de mettre en place une stack d'observabilité simple avec Prometheus, Docker Compose, Node Exporter et une API Python instrumentée avec `prometheus_client`.

J'ai configuré Prometheus pour scraper plusieurs services, mis en place du service discovery avec `file_sd_configs`, créé des règles Prometheus et connecté l'ensemble des conteneurs sur un même réseau Docker.

## Difficultés rencontrées

Je me suis heurté à pas mal de murs pendant ce projet, notamment sur la configuration de Docker Compose, la gestion des volumes, les erreurs YAML dans Prometheus, le réseau entre conteneurs et la configuration des targets.

J'ai aussi eu plusieurs blocages sur mon application Python, entre les dépendances manquantes, l'exposition des métriques et le bon paramétrage pour que Prometheus puisse la scraper correctement.

## Utilisation de l'IA

Je me suis aidé de l'IA à plusieurs moments pour débloquer certaines erreurs techniques, mieux comprendre le fonctionnement de Docker, de Prometheus et corriger des problèmes de configuration. Ça m'a surtout servi de support pour avancer plus efficacement et comprendre mes erreurs.

## Bilan

Projet parfois frustrant, mais très formateur. Il m'a permis de mieux comprendre l'observabilité, l'instrumentation d'une application et le fonctionnement global d'une stack de monitoring moderne.

J’ai bloqué sur l’indentation, j’avais jamais testé d’appeler un yaml dans un docker-compose.
J’ai demandé à chat gpt de m’aider à comprendre comment utiliser les commandes et j’ai revu les volumes pour remplacer le yaml du conteneur par le mien.  
 
Docker a du mal à lire les wildcard, j’ai mis le nom des fichiers en dur dans le prometheus.yml.
