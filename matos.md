# découpe vinyle


Vos fichiers doivent:
* avoir été créés sur un logiciel de dessin vectoriel (Illustrator, Corel, Inkscape, etc.)
* tenir dans la largeur du rouleau (vérifier avec l’opérateur)
* attention, tous les traits seront découpés. Pensez à combiner les formes que vous voulez faire et à vectoriser les polices et les tracés. Si vous êtes sur Illustrator, vous pouvez voir les tracés en pressant Ctrl+Y. Si vos traits sont séparés, vous pouvez les combiner en utilisant la commande ‘pathfinder’.
* travaillez une couleur à la fois.
* ne pas faire de découpe trop petite. Les textes en dessous de 5mm de haut seront très fastidieux à mettre en place
* économisez de la matière!


# Imprimante 3D Zortrax m200
Volume maximum d’impression : 200 x 200 x 180 mm

**impression 3D**

* Les imprimantes Solidoodle et Ultimaker fonctionnent par dépôt de fil chaud. Elle déposent un filament plastique couche par couche. Les volumes démoulables sont donc les plus simple à imprimer.

* Vos fichiers doivent être:
* créés sur un logiciel de modélisation 3D (Rhinoceros, Blender, Sketchup, etc.) ou téléchargés d’une bibliothèque ligne (thingiverse, google 3D warehouse, etc.)
* exportés en format .STL (pour stéréolithographie)
* le fichier doit tenir dans un volume 200x200x200mm. (sinon, prévoir de l’assemblage soit par collage soit mécanique)
* Les volumes doivent être totalement fermés.
* Les dépouilles doivent faire au maximum 110°.
De toutes façons, en discuter avec l’opérateur des machines pour évaluer la faisabilité et le temps machine.


**Sous Windows**

* Installer Pronterface
* Installer Sl3cer
* Installer driver*

Cas de la pièce originale
Modeliser le fichier 3D (Solidworks, Sketch’up, Rhinoceros)
Exporter en stl >> options ASCII (fichier moins lourd)
Nom du fichier sans accent ni caractères spéciaux.

Export faisable sous Solidworks ou Rhinoceros
Avantage Rhino temps de compilation 3D>STL puis STL>Gcode mais fichier moins précis.
Avantage Solidworks fichier STL fidèle au modèle 3D temps de compilation 3D>STL très long STL>Gcode encore plus long.

Ouvrir Pronterface

image....

Vérifier le port com04 ou 06
     la vitesse 250000
Cliquer sur le bouton «connect»
Complèment à droite, il y a une sorte de journal qui affiche toute les informations en directe venant de la machine.
Cocher la case «monitor»
Cela active les graphique de température complètement en bas à gauche.
Régler la température de la buse à 200° et du plateau à 95°.
Cliquer sur «On» pour activer la montée en température.
Pour créer le Gcode pour l’impression:
Cliquer sur «Fichier>Slicing Setting»
    La fenêtre de Sl3cer s’ouvre, chaque onglet correspond aux réglagles machines (remplissage, nombre de contour, dimensions du plateaux).
Cliquer sur Ouvrir, aller chercher le fichier stl.

image 2


image 3

# Imprimante papier A3

# Station de soudure

# Stylo 3d
