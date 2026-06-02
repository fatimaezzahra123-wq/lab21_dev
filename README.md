# 📡 Sensors App

Application Android de visualisation des capteurs embarqués, développée dans le cadre du cours **Programmation Mobile : Android avec Java**.

---

## 🎥 Démo vidéo

[![Demo](https://img.shields.io/badge/YouTube-Voir%20la%20démo-red?logo=youtube)](https://youtu.be/6O1dlAUB5w4?si=quGZ1YLSTUaOj49D)

---

## 📐 Architecture du projet

```
ensa.ma.sensors
│
├── MainActivity.java              # Activité principale avec menu latéral
│
├── fragments/
│   ├── SensorsListFragment.java   # Liste de tous les capteurs disponibles
│   ├── SensorGraphFragment.java   # Graphe générique (temp, humidité, proximité, magnétique)
│   ├── MotionSensorFragment.java  # Accéléromètre, gravité, gyroscope
│   ├── StepCounterFragment.java   # Compteur de pas
│   ├── CompassFragment.java       # Boussole numérique
│   └── ActivityRecognitionFragment.java  # Reconnaissance d'activité
│
├── utils/
│   └── SensorFormatter.java       # Formatage des infos techniques des capteurs
│
└── views/
    └── LineChartView.java         # Composant graphique personnalisé
```

---

## ✨ Fonctionnalités

| Fonctionnalité | Description |
|---|---|
| 📋 Liste des capteurs | Affiche tous les capteurs avec leurs infos techniques |
| 🌡️ Température | Graphe de la température ambiante |
| 💧 Humidité | Graphe de l'humidité relative |
| 📏 Proximité | Détection d'objets proches |
| 🧲 Champ magnétique | Norme du champ magnétique |
| 📱 Accéléromètre | Axes X, Y, Z et norme |
| ⬇️ Gravité | Composante gravitationnelle |
| 🔄 Gyroscope | Taux de rotation en rad/s |
| 👟 Compteur de pas | Pas depuis le redémarrage et de la session |
| 🧭 Boussole | Direction en degrés (Nord, Sud, Est, Ouest) |
| 🏃 Reconnaissance d'activité | Marche, saut, position stable |

---

## 🛠️ Technologies utilisées

| Technologie | Rôle |
|---|---|
| SensorManager | Accès aux capteurs Android |
| SensorEventListener | Réception des mesures en temps réel |
| Fragment | Organisation modulaire de l'interface |
| Navigation Component | Navigation entre les fragments |
| Canvas / Path | Dessin du graphe personnalisé |
| Handler | Simulation des capteurs indisponibles |

---

## 📊 Informations techniques affichées

Pour chaque capteur :
- **Id** — identifiant unique
- **Name** — nom du capteur
- **Vendor** — fabricant
- **Version** — version
- **Type** — type textuel
- **Int Type** — type entier
- **Resolution** — résolution
- **Power** — consommation en mA
- **Maximum Range** — plage maximale
- **Min Delay** — délai minimal en µs

---

## 🚀 Lancer le projet

1. Clone le repo :
```bash
git clone https://github.com/fatimaezzahra123-wq/lab21_dev.git
```

2. Ouvre dans **Android Studio**

3. Sync Gradle et lance **Run ▶️**

> Min SDK : 24 — Target SDK : 34 — Java 17

---

## 🧪 Tests réalisés

| Test | Résultat |
|---|---|
| Liste des capteurs | ✅ |
| Température (simulation) | ✅ |
| Humidité (simulation) | ✅ |
| Proximité | ✅ |
| Champ magnétique | ✅ |
| Accéléromètre | ✅ |
| Gravité | ✅ |
| Gyroscope | ✅ |
| Compteur de pas | ✅ |
| Boussole | ✅ |
| Reconnaissance d'activité | ✅ |

---



## 👩‍💻 Auteur
FATIMAEZZAHRA ENNASSIRI
