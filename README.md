# 🌤 Sunu Météo — L3GL ISI 2026

Application Flutter de météo en temps réel pour 5 villes sénégalaises.

## 👥 Membres du groupe

| Nom | Prénom |
|-----|--------|
| À compléter | À compléter |
| À compléter | À compléter |
| À compléter | À compléter |

---

## 📱 Fonctionnalités

- **Écran d'accueil** : Message de bienvenue + bouton de lancement
- **Jauge animée** : Progression en temps réel pendant le chargement
- **Messages dynamiques** : Messages rotatifs pendant le chargement
- **Tableau météo interactif** : Dakar, Rufisque, Thiès, Saint-Louis, Kolda
- **Détail de ville** : Infos complètes + localisation sur Google Maps
- **Gestion des erreurs** : Message d'erreur + bouton réessayer
- **Dark/Light Mode** : Thème sombre et clair
- **Bouton Recommencer** : Relance l'expérience complète

---

## 🛠 Technologies

| Technologie | Usage |
|-------------|-------|
| Flutter | Framework mobile |
| Provider | Gestion d'état |
| Retrofit + Dio | Appels API REST |
| OpenWeatherMap API | Données météo en temps réel |
| Google Maps Flutter | Carte interactive |

---

## ⚙️ Installation

### 1. Cloner le projet
```bash
git clone <URL_DU_REPO>
cd sunu_meteo
```

### 2. Configurer la clé OpenWeatherMap
Dans `lib/core/constants/api_constants.dart` :
```dart
static const String apiKey = 'TA_CLE_API_ICI';
```

### 3. Configurer Google Maps
Dans `android/app/src/main/AndroidManifest.xml` :
```xml
<meta-data
    android:name="com.google.android.geo.API_KEY"
    android:value="TA_CLE_GOOGLE_MAPS"/>
```

### 4. Installer les dépendances
```bash
flutter pub get
```

### 5. Lancer
```bash
flutter run
```

---

## 📁 Architecture

```
lib/
├── main.dart
├── core/
│   ├── constants/
│   │   ├── api_constants.dart
│   │   └── app_strings.dart
│   └── theme/
│       └── app_theme.dart
├── data/
│   ├── models/
│   │   └── weather_model.dart
│   └── services/
│       └── weather_api_service.dart
└── presentation/
    ├── providers/
    │   ├── weather_provider.dart
    │   └── theme_provider.dart
    ├── screens/
    │   ├── home_screen.dart
    │   ├── main_screen.dart
    │   └── city_detail_screen.dart
    └── widgets/
        ├── animated_gauge.dart
        └── weather_table.dart
```

---

*Examen de Développement Mobile — L3GL ISI 2026*
