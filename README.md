# WORKSHOP-Decouverte-Arcore_Flutter

# Dépendences requises
---
- flutter ```sudo snap install flutter --classic```

Si vous voulez voir vos appareils virtuels n'oubliez pas de télécharger les extensions flutter et dart et d'ouvrir votre projet flutter avec votre IDE.

---

# Création du projet
---
Tout d'abord, vous allez créer un projet flutter grâce a la commande suivante (linux): ```flutter create "my_app"```

# Mise en place d'un emulateur Android
---

Si vous avez un android, vous pouvez sauter cette étape et utiliser votre téléphone en mode débogage en le branchant à votre PC.

Sinon, téléchargez Android Studio afin de pouvoir créer un emulateur android qui nous permettra de lancer l'application en AR.

- Une fois l'application télechargée, ouvrez l'application à l'emplacement de votre projet et cliquez sur "Device Manager" en haut à droite d'Android Studio.
<img src="assets/Device_Manager.png">

- Ensuite, vous devriez voir un message "Create virtual device", laissez le téléphone de base (Pixel 2) et cliquez sur next.

- Choisissez l'API level 27 (Oreo) et cliquez sur next.

- Allez dans "Show Advanced Settings" et vérifiez que votre "Camera Back" soit bien en "VirtualScene" et vous pouvez finaliser votre émulateur et on peut fermer Android Studio.

- Lorsque vous allez lancer votre téléphone, une barre verticale apparaîtra avec une icône composée de trois point ("...").

- Cliquez dessus, allez dans l'onglet "settings", ensuite dans "advanced" puis modifiez "autoselect" par "Renderer maximum (up to OpenGL ES 3.1)"

# Afficher des objets en AR (sphères, rectangle, triangle...)
---

Tout d'abord, vous allez avoir besoin du package ARCore pour flutter ainsi que quelques modifications dans notre projet afin de le faire marcher. Pour cela je vous laisse aller voir la doc du package flutter. Tout ce dont vous avez besoin est dedans: https://pub.dev/packages/arcore_flutter_plugin

# Aller plus loin

Si vous voulez aller plus loin, vous pouvez accrocher vos objets (sphères, rectangle...) à un plan en AR et normalement chaque plan créera un nouvel objet.