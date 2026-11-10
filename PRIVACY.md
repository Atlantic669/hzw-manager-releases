# Confidentialité

Horizon Wallpaper ne collecte rien sur vous. Il n'y a ni compte, ni publicité, ni statistiques d'utilisation. Tout ce que fait l'application reste sur votre PC, à l'exception des quelques connexions listées plus bas, qui ont toutes une raison précise.

## Ce qui est enregistré sur votre PC

Tout se trouve dans `%APPDATA%\Horizon Wallpaper\` :

| Fichier | Contenu |
| --- | --- |
| `config.json` | Vos réglages, vos ambiances et la liste de vos fonds (avec le chemin de vos fichiers). Contient aussi votre clé Pixabay, si vous en avez ajouté une, **chiffrée avec le coffre de Windows** : seule votre session Windows peut la relire. |
| `library\` | Les fonds que vous avez téléchargés depuis l'onglet Explorer. |
| `horizon.log` | Les erreurs techniques, pour aider à corriger un problème (256 Ko au maximum). Il ne contient ni vos recherches ni ce que vous écoutez. |

Vos propres images et vidéos ne sont jamais copiées ni modifiées. L'application lit seulement les fichiers que vous avez ajoutés à la bibliothèque, et rien d'autre.

## Les fonctions qui touchent à vos données

Celles qui concernent le son et la musique sont **désactivées par défaut**.

**Réaction à la musique et visualiseur audio.** L'application écoute le son de votre PC grâce à la boucle locale de Windows, comme le ferait un égaliseur. Le son est analysé en mémoire sous forme de niveaux (graves, médiums) pour animer le fond. Il n'est **jamais enregistré, conservé ni envoyé**. L'écoute s'arrête dès que les deux options sont désactivées, ou quand l'application est en pause.

**Lecture en cours.** L'application lit, auprès de Windows, le titre, l'artiste et la pochette de la musique qui joue (Spotify, navigateur…). Ces informations s'affichent sur votre fond, et c'est tout : elles ne sont ni enregistrées ni envoyées.

**Parallaxe à la souris.** La position de votre curseur est lue sur votre PC pour faire bouger le fond. Elle ne sort pas de l'application.

**Pause en plein écran.** L'application vérifie si la fenêtre au premier plan recouvre l'écran, à partir de sa taille et de son type. Elle ne lit ni son titre ni son contenu.

## Les connexions à internet

L'application ne se connecte qu'à ces services. Chacun voit votre adresse IP, comme pour n'importe quelle page web.

| Service | Quand | Ce qui est envoyé |
| --- | --- | --- |
| **GitHub** | Au démarrage puis toutes les 4 h (version installée uniquement) | Une demande de la dernière version disponible |
| **Wallhaven** | Quand vous cherchez des fonds fixes dans Explorer | Votre recherche |
| **Wikimedia Commons** | Quand vous cherchez des fonds animés sans clé Pixabay | Votre recherche |
| **Pixabay** | Quand vous cherchez des fonds animés avec votre clé | Votre recherche et votre clé |
| `w.wallhaven.cc`, `upload.wikimedia.org`, `cdn.pixabay.com` | Quand vous cliquez sur « Ajouter » | Le téléchargement du fond choisi |

Les miniatures de l'onglet Explorer sont chargées depuis ces mêmes services. Les requêtes portent un identifiant générique (`HorizonWallpaper/1.0`), sans aucune information sur vous.

## Tout effacer

1. Désinstallez Horizon Wallpaper (Paramètres Windows › Applications).
2. Supprimez le dossier `%APPDATA%\Horizon Wallpaper\`.

Il ne reste alors plus aucune trace de l'application.

## Une question ?

Ouvrez une discussion sur [le dépôt des versions](https://github.com/Atlantic669/horizon-wallpaper-releases/issues).
