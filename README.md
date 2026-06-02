# ShieldCheck Mali - Système Anti-Vol

Application Flutter de suivi et de verrouillage de téléphones déclarés volés utilisant Supabase.

## 🚀 Installation

### 1. Configuration Supabase

Avant de compiler :

1. Accédez à [supabase.com](https://supabase.com)
2. Créez un nouveau projet ou utilisez un existant
3. Copiez vos identifiants :
   - **URL du projet** : Format `https://xxxxx.supabase.co`
   - **Clé Anon** : Clé API publique (45+ caractères)

4. Ouvrez `lib/main.dart` et remplacez :
```dart
url: 'YOUR_PROJECT_ID.supabase.co'  // ← Remplacer
anonKey: 'YOUR_ANON_KEY_HERE'       // ← Remplacer
```

### 2. Installation des dépendances

```bash
flutter pub get
```

### 3. Générer les permissions Android

```bash
cd android
./gradlew clean
cd ..
```

### 4. Compiler et lancer

```bash
# Debug
flutter run

# Release
flutter build apk --release
```

## 📋 Prérequis

- Flutter 3.0.0 ou supérieur
- Dart 3.0.0 ou supérieur
- Android SDK (pour Android)
- Xcode (pour iOS)

## 🔑 Dépendances

- `supabase_flutter: ^2.5.0` - Client Supabase
- `device_info_plus: ^9.0.0` - Information de l'appareil
- `geolocator: ^11.0.0` - Localisation GPS
- `shared_preferences: ^2.2.0` - Stockage local

## ⚙️ Configuration requise

### Android
- Minimum SDK: 21
- Target SDK: 33+
- Permissions: GPS, Localisation, Device Admin

### iOS
- Minimum iOS: 11
- Permissions: Localisation

## 📝 Notes importantes

⚠️ **REMPLACEZ VOS IDENTIFIANTS SUPABASE AVANT DE COMPILER**

Les identifiants par défaut dans le code ne fonctionneront pas.

## 📞 Support

Pour toute question, consultez la documentation Supabase : https://supabase.com/docs
