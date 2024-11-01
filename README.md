# Glacial par Audrey Dandurand
## Concept
#### Objectif
L'objectif est de sensibiliser le public face aux enjeux du réchauffement climatique et de la perte de faune.

#### Idée
Glacial est une installation interactive formée de projections vidéos sur les murs et sur le plancher. Celle-ci représente l'environnement glacial de l'Antartique et elles sont formées d'animations 3D.

Il n'y a aucun moyen de gagner le jeu.

La salle a une ambiance bleutée durant l'expérience.


| ![projection_sol](https://github.com/user-attachments/assets/ebdf8362-4514-4275-83ae-6b5cdadec939)  | ![projection_mur_01](https://github.com/user-attachments/assets/fb2e7732-cef2-4c6e-bc01-7646b46cde0a)    |
| -------- | ------- |

|  ![experience-board-00001](https://github.com/user-attachments/assets/284c73e5-7a77-4c94-8029-a476dcf472c2) |  ![experience-board-00002](https://github.com/user-attachments/assets/01a23ccd-6344-4e7a-8572-1ab854449b30)   |
| -------- | ------- |


#### Références visuelles
Une palette de couleur bleutée a été choisie pour soutenir le thème de la fonte des glaciers. Celle-ci va s'appliquer autant à la lumière que les animations 3D.

Les images visuelles auront un aspect plus réaliste pour sensibiliser davantage le public cible.

![planche_inspiration](https://github.com/user-attachments/assets/01781df8-59d5-48ff-80be-104d2bf0c87a)

Les expériences interactives présentées démontrent la projection à 360 degrés ainsi que la projection sur le sol. Dans les images d'exposition interactive, nous pouvons apercevoir sur le sol une vue du dessus et sur le mur, une vision de face. Ce principe est ce qui est voulu pour l'oeuvre Glacial.

#### Références sonores
Les ambiances permettent de bien représenter le milieu dans lequel sont plongés le public.

<iframe width="560" height="315" src="https://www.youtube.com/embed/xdWXvurWb2U?si=Y4n-GHaK9mWUAcEd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/ltkhJhNo6a8?si=_nwkhdPDrkjOinOO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Scénario interactif

Un glacier est présenté sur le sol par une projection et une ambiance sonore est jouée dans la salle. Le visiteur est amené à se déplacer dans l'espace et à survivre face à la fonte des glaces. Tout d'abord, il sera amené à se placer sur le glacier. Après un certain moment, la glace craquera et le visiteur devra se déplacer pour survivre. Les déclenchements de la fonte de glace seront effectués par la position des visiteurs dans l'espace et ceux-ci seront accompagnés de plusieurs sons. Tant que le visiteur ne sera pas dans un espace ciblé, il restera en vie sur le glacier. S'il sort du glacier, ce sera la fin pour lui. À ce moment, une lumière s'allumera et teintera la pièce d'un rouge foncé durant quelques secondes. 

Dès que les visiteurs sont tous morts, la projection du sol devient de plus en plus foncée comme si l'animal coulait au fond de l'eau. Les lumières deviennent elles aussi bleu foncé. Un message apparait sur les murs pour sensibiliser le public face au réchauffement climatique.

```mermaid
graph TD;
    Interaction-->Lumières;
    Interaction-->Vidéos;
    Interaction-->Audio;
    Lumières-->AmbianceLumineuse[Ambiance lumineuse];
    Audio-->AmbianceBase[Ambiance de base];
    Craquement-->Glace[Audio de la glace];
    Vidéos-->Craquement[Craquement de la glace];
    Vidéos-->Stable[Glacier];
    Stable-->Interaction;
    Glace-->Placement[Placement du joueur];
    AmbianceLumineuse-->Placement[Placement du joueur];
    AmbianceBase-->Placement[Placement du joueur];
    Placement-->| Dans l'eau |Mort;
    Placement-->| Sur le glacier |Survie;
    Survie-->Interaction;
    Mort-->Veille[Mode de veille];
```

## Scénarimage


## Synoptique
#### Schéma technique
```mermaid
graph TD;
    Ordinateur[Contrôle central - Ordinateur]-->DMX[USB DMX];
    Ordinateur[Contrôle central - Ordinateur]-->CarteSon[Carte de son];
    Ordinateur[Contrôle central - Ordinateur]-->HDMI;
    Ordinateur[Contrôle central - Ordinateur]-->Kinect[Kinect - Capteur];
    Kinect[Kinect - Capteur]-->Ordinateur[Contrôle central - Ordinateur];
    DMX[USB DMX]-->Lumière;
    CarteSon[Carte de son]-->Haut-parleur;
    Haut-parleur-->Audio[Sortie audio];
    HDMI-->Projecteurs;
    Projecteurs-->Projection[Projection vidéo];
   
```

Les différents signaux:
- Audio (MIDI)
- Vidéo (HDMI)
- Lumières (DMX)

| Système de communication  | Logiciel    | Interaction |
| -------- | ------- |------- |
| Protocole MIDI  |  LoopMidi  | QLC+ et Plugdata  |
| Protocole DMX  |  QLC+  | Lumiere et logiciel  |

#### Flux de données

## Plantation

#### Emplacement des dispositifs
![materiel](https://github.com/user-attachments/assets/03bff45a-1860-4130-9377-fe791c721f28)

#### Circulation des visiteurs

#### Gestion des câblages

## Support médiatique
Divers médias sont utilisés pour cette installation.

| Type de médias    | Intégration |
| -------- | ------- |
| Projections d'animation 3D  | Elles sont présentes sur tous les murs et le plafond du début à la fin de l'expérience.    |
| Audio | Une ambiance de base joue durant l'expérience et plusieurs sons y sont ajoutés.     |
| Lumières DMX    | Ces lumières apportent une ambiance bleautée à l'expérience.    |
| Capteur de mouvement    |  Celui-ci permet l'interactivité de Glacial.    |

## Matériel

| Matériel  | Raison |
| -------- | ------- |
| 1 Kinect  |     |
| 6 Lumières American DJ 5p Hex | Ambiance lumineuse  |
| 5 Projecteurs | Projections visuelles sur les 4 murs et le sol  |
| 4 Haut-parleurs    |  Sortie de l'audio à chaque coin de la salle  |


## Logiciel

| Logiciel    | Technique |
| -------- | ------- |
| Touch designer  | Rassemble le son et la 3d pour effectuer la projection    |
| Reaper | Montage sonore     |
| Maya    | Animation 3D    |
| QLC+    | Création des scènes lumineuses    |
| Plugdata    | Création d'un lfo pour modifier les couleurs des lumières    |


## Références
- [Pinterest](https://www.pinterest.com/)
- [Funky Forest](https://www.design-io.com/projects/funkyforest)
- [Frameless](https://frameless.com/the-experience/the-world-around-us/)
- [teamLab](https://www.teamlab.art/fr/e/lavillette/)
