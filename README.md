Access-Attendance-System avec ESP32 et empreinte digitale
Description

Le Access-Attendance-System est un système de contrôle d’accès et de suivi de présence basé sur la reconnaissance d’empreintes digitales. Il utilise un microcontrôleur ESP32 pour authentifier les utilisateurs, enregistrer leurs présences et gérer l’accès aux locaux de manière sécurisée.

Ce système est idéal pour les entreprises, écoles ou clubs souhaitant moderniser leur suivi des employés ou des membres.

Fonctionnalités

Authentification biométrique via capteur d’empreintes digitales.

Enregistrement automatique de la date et de l’heure à chaque accès.

Gestion des utilisateurs et contrôle des permissions d’accès.

Notifications visuelles et sonores (LED et buzzer) pour accès autorisé ou refusé.

Affichage des informations sur un écran OLED ou LCD.

Synchronisation des données via Wi-Fi vers une base de données ou un serveur cloud.

Matériel requis

ESP32 (avec Wi-Fi intégré)

Capteur d’empreintes digitales (ex. R307, GT-521F32)

Écran OLED ou LCD (optionnel mais recommandé)

Buzzer et LED

Carte SD (optionnelle pour stockage local)

Câbles et alimentation adaptée

Installation et configuration

Connecter le capteur d’empreintes, l’écran et le buzzer à l’ESP32 selon le schéma fourni.

Installer l’IDE Arduino et ajouter le support ESP32.

Installer les bibliothèques suivantes :

Adafruit Fingerprint Sensor Library

U8g2 pour l’écran OLED

WiFi et HTTPClient pour la communication réseau

Configurer le fichier config.h avec :

Les informations Wi-Fi (SSID et mot de passe)

Les paramètres de stockage ou d’envoi vers le serveur

Téléverser le code sur l’ESP32 via l’IDE Arduino.

Utilisation

Enregistrer les empreintes des utilisateurs via l’interface de l’écran ou l’ordinateur.

À chaque passage devant le capteur, le système valide l’empreinte et enregistre l’heure et la date.

Les données peuvent être consultées sur l’écran ou récupérées depuis le serveur/cloud.

Schéma de connexion (simplifié)
ESP32
 ├─ Capteur d’empreinte → UART (RX/TX)
 ├─ OLED/LCD → I2C (SDA/SCL)
 ├─ Buzzer → GPIO
 └─ LED → GPIO

Avantages

Sécurité accrue grâce à la biométrie.

Réduction des erreurs de pointage manuel.

Historique en temps réel pour le suivi des présences.

Facile à déployer et à intégrer dans un réseau existant.
