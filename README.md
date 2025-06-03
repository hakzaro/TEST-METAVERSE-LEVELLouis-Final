
# ✨ Retour vers le Futur ! 💫 - Scène A-Frame Interactive

Ce projet est une scène de Réalité Virtuelle interactive développée avec A-Frame, inspirée de l'univers de "Retour vers le Futur". Explorez un environnement 3D où vous pouvez interagir avec divers éléments pour déclencher des animations, des sons et des changements de texture.

## Fonctionnalités Principales

* **Exploration VR :** Naviguez dans la scène à l'aide des commandes clavier/souris (WASD + souris).
* **Objets Interactifs :** Plusieurs objets sont cliquables et déclenchent des actions spécifiques.
* **Changement de Texture :** Un écran interactif change de texture au clic, offrant deux visuels différents (une texture "Doc explose" et une texture "explosion").
* **Mouvement d'Objet :** Une sphère se déplace d'une position à une autre au clic.
* **Lecture Sonore :** Un buzzer active ou désactive un son.
* **Contrôle Vidéo :** Une télécommande permet de jouer ou de mettre en pause une vidéo intégrée dans la scène.
* **Scaling d'Objet :** Un cône peut doubler de taille au clic.
* **Lancement de Son et Animation :** La voiture DeLorean déclenche un son au clic.
* **Modèles 3D :** Intégration de modèles glTF (voiture, hoverboard, Marty, Doc) et OBJ (télécommande) pour enrichir la scène.
* **Ambiance Visuelle :** Un ciel panoramique ("fondfutur.jpg") et un sol texturé définissent l'environnement.
* **Éléments Néon :** Des panneaux d'information et des éléments interactifs utilisent des couleurs néon pour un style distinctif.

## Technologies Utilisées

* **A-Frame 1.5.0 :** Framework web pour la construction d'expériences de réalité virtuelle.
* **Composants A-Frame Externes :**
    * `aframe-event-set-component`
    * `aframe-extras` (pour `gltf-model`, `look-controls`, `wasd-controls`)
    * `aframe-super-hands-component`
* **Composants A-Frame Personnalisés :**
    * `toggle-texture` : Permet de basculer entre deux textures.
    * `move-on-click` : Déplace un objet entre deux positions.
    * `play-sound-on-click` : Joue un son au clic.
    * `toggle-video` : Contrôle la lecture d'une vidéo.
    * `toggle-sound` : Active ou désactive un son.
    * `toggle-scale` : Change la taille d'un objet au clic.

## Lancement du Projet

Pour visualiser ce projet A-Frame, ouvrez le fichier `index.html` dans un navigateur web moderne.

**Note Importante :** Pour que toutes les ressources (modèles 3D, textures, vidéos, sons) se chargent correctement, il est fortement recommandé de servir le projet via un serveur web local (par exemple, avec Python `http.server`, Node.js `serve`, ou un environnement de développement web comme XAMPP/MAMP). Ouvrir `index.html` directement depuis votre système de fichiers (`file:///`) peut entraîner des restrictions de sécurité qui empêcheront certaines ressources de s'afficher. Ou avec Visual Studio via la fonction "Live Server".

## Structure du Projet

votre_projet/
├── index.html              # Fichier principal de la scène A-Frame
└── assets/                 # Contient toutes les ressources (textures, modèles, sons, vidéos)
├── texture/            # Images pour les textures
│   ├── sol.jpg
│   ├── affiche1.jpg
│   ├── affiche2.jpg
│   ├── fondfutur.jpg   # Ciel 360
│   ├── texturedoc.jpg  # Texture de l'écran cliquable
│   └── explosion.jpg   # Seconde texture de l'écran cliquable
├── sounds/             # Fichiers audio
│   ├── son.mp3
│   └── son3.mp3
├── videos/             # Fichiers vidéo
│   └── son2.mp4
└── models/             # Modèles 3D
├── voiture.glb
├── hoverboard.glb
├── marty.glb
├── doc.glb
└── remote/         # Modèle et texture de la télécommande
├── remote.obj
└── remote.mtl

