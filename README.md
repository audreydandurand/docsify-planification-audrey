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
#### Visualisation des séquences
Projection visuelle sur le sol
![scenarimage 2024-11-02 11 17 44](https://github.com/user-attachments/assets/2c6f3cd9-2bfb-4869-9b35-e9e3fface3e2)

#### Évolution visuelle et narrative

|  Arrivé du joueur | Interactivité    |
| -------- | ------- |
| ![scenarimage-board-00002](https://github.com/user-attachments/assets/fcfcd2f9-c7f2-483a-a1d1-35155dc73658)  |  ![scenarimage-board-00003](https://github.com/user-attachments/assets/e34797f8-02fb-4ab5-bfbb-d660653a704d)  |

Les différentes possibilités lors du jeu...
| Mort  | Survie    |
| -------- | ------- |
| ![scenarimage-board-00004](https://github.com/user-attachments/assets/95a13424-7c55-4367-913a-e641d6c7f244)  |  ![scenarimage-board-00005](https://github.com/user-attachments/assets/315f251f-d9a9-4d4d-8b3f-08d84d2189ab)  | 
| ![scenarimage-board-00006](https://github.com/user-attachments/assets/51cae7c8-622a-437b-a5b2-8ed90dc9401e)  |  ![scenarimage-board-00007](https://github.com/user-attachments/assets/500612d2-9d3b-46be-a841-ffdf0cd9cc31)  |
| ![scenarimage-board-00008](https://github.com/user-attachments/assets/b28d9b48-000d-48a5-9984-3c95ac41ecc3)  |  ![scenarimage-board-00009](https://github.com/user-attachments/assets/9ea1bf11-6f07-4a65-b4d1-4f3edddbc4fb)  | 
| ![scenarimage-board-00011](https://github.com/user-attachments/assets/a28529ab-6a51-410a-b9fb-d64d54232bf2)  |  ![scenarimage-board-00012](https://github.com/user-attachments/assets/a6e7352a-33a6-4547-a3b1-5914858cfc62)  |
| ![scenarimage-board-00013](https://github.com/user-attachments/assets/0c2d897b-3824-4087-bc0a-ac5393cddcd6)  | ![scenarimage-board-00014](https://github.com/user-attachments/assets/fa1250bd-37fc-413d-a8f1-419d14b8f6d1)   | 
| ![scenarimage-board-00016](https://github.com/user-attachments/assets/3e30a571-92f9-4c53-9b81-f024902f381b)  |  ![scenarimage-board-00015](https://github.com/user-attachments/assets/23e1326f-1915-4461-8558-9d97168db4a5)  |
| ![scenarimage-board-00017](https://github.com/user-attachments/assets/99812391-4da0-4d5a-8e59-76b52d0fc547)  |  ![scenarimage-board-00018](https://github.com/user-attachments/assets/bd41b17c-5e7b-4de4-a973-fbdfa2937794)  | 
| ![scenarimage-board-00020](https://github.com/user-attachments/assets/0de2d959-3fdb-4eda-99fb-a69d9caf1779)  |  ![scenarimage-board-00022](https://github.com/user-attachments/assets/7892f765-9a1d-4851-864c-cfbbed602639)  |
| ![scenarimage-board-00024](https://github.com/user-attachments/assets/9b8e640f-ce5e-4165-83fc-8af964b1592a)  |  ![scenarimage-board-00023](https://github.com/user-attachments/assets/4fab18cf-b5d5-49e5-8eb1-cc35cfb7c88a)  | 

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
