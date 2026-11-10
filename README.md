# Tool library pour Carbide Create

Ces réglages ont été pour réalisés pour la CNC TwoTrees TTC-H40.

Les fraises sélectionées sont:
 - End mill SpeTool SP1F-D6-L22
 - End mill SpeTool SP-D6-H6-D
 - End mill SpeTool SP-D4-L22-D
 - Ball nose Dreanique R0.5-20.5-D4-HSi
 - Ball nose Dreanique R1.0-20.5-D4-HSi
 - Surfacing bit XCAN 4T 6x25.4x45mm

## Utilisation

Il faut sélectionner la bonne fraise, avec la bonne matière et pour la bonne opération.
Par exemple le réglage `SP-D6-H6-D [CP Bouleau] | Poche` correspond à la fraise Down Cut 2F 6mm dans du contre plaqué bouleau et est adapté à l'opération Pocket.

Le réglage `SP1F-D6-L22 [MDF] | Détourage | Molette 3` correspond à la fraise Up cut 1F 6mm pour usiner du MDF sur une opération de détourage. Comme j'ai pris le réglage pour la Makita, je dois la régler sur la molette 3 (17k RPM).

## Remarques

Il vaut mieux utiliser la SP-D4-L22-D pour éviter de trop grosses contraintes sur les axes de la CNC.
Idéalement, il faut mettre une rampe pour entrer dans la matière.

## Usinage 3D
L'ébauche 3D (Roughing) : Utiliser la fraise SP-D4 (4mm). Elle va retirer le plus gros de la matière rapidement en faisant des paliers (marches d'escalier). On laisse une surépaisseur de 0,5 mm.
La finition 3D (Finishing) : Changer d'outil pour la Ball Nose. Elle va suivre fidèlement les courbes du relief. L'usinage sera long (parfois plusieurs heures), mais le résultat au sortir de la machine est spectaculaire. Utiliser la fraise de 0.5mm pour avoir un rendu parfait.
