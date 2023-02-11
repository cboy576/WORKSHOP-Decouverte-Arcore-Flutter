# WORKSHOP-Decouverte-Arcore_Flutter

# dependences requise
---
- flutter ```sudo snap install flutter --classic```

si vous voulez voir vos appareil virtuel n'oublier pas de telécharger les extensions flutter et dart et d'ouvrir votre projet flutter avec votre IDE.

---

# Création du projet
---
Tout d'abord, vous allez crée un projet flutter grâce a la commande suivante(linux): ```flutter create "my_app"```

# Mise en place d'un emulator Android
---

Si vous avez un android, vous pouvez sauter cette etape et utiliser votre telephone en mode debogage en le branchant a votre PC.

Sinon, telecharger android studio afin de pouvoir crée un emulator android qui nous permettra de lancer l'application en AR.

- Une fois l'application telecharger, ouvrer l'application a l'emplacement de votre projet et cliquer sur "Device Manager" en haut a droite d'android studio.
<img src="assets/Device_Manager.png">
- Ensuite, vous devriez voir un message "Create virtual device", laissez le telephone de base (Pixel 2) et cliquez sur next.
- Choisisser l'API level 27 (Oreo) et cliquez sur next.
- allez dans "Show Advanced Settings" et verifier que votre Camera Back et bien en "VirtualScene" et vous pouver finalisez votre emulateur et on peut fermer Android Studio.
- lorsque vous allez lancez votre telephone, une barre verticale apparaitra avec une icone composer de trois point ("...").
- cliquer dessus, allez dans l'onglet settings, advanced puis modifier "autoselect" par "Renderer maximum (up to OpenGL ES 3.1)"

# Afficher des objets en AR (sphere, rectangle, triangle...)
---

Tout d'abord, vous allez avoir besoin du package ARCore pour flutter ainsi que quelque modification dans notre projet afin de le faire marcher, pour ca je vous laisse allez voir la doc du package flutter, tout ce dont vous avez besoin et dedans: https://pub.dev/packages/arcore_flutter_plugin

# Allez plus loin

Si vous voulez allez plus loin, vous pouvez accrochez vos objets (spheres, rectangle...) a un plan en AR et normalement chaque plan créera un nouvel objet.