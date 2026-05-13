# Calculateur de type de compresseur — Diagramme Ns-Ds

Ce projet est un outil Python simple permettant de faire un pré-dimensionnement de compresseur à partir du diagramme Ns-Ds.

L’objectif est de calculer la vitesse spécifique Ns, d’identifier le type de compresseur le plus adapté et, si le diamètre de roue est connu, de calculer le diamètre spécifique Ds.

## Fonctionnalités

- Calcul du rapport de pression PR
- Calcul du travail adiabatique de compression
- Calcul de la vitesse spécifique Ns
- Identification automatique du type de compresseur recommandé
- Calcul du diamètre spécifique Ds si le diamètre de roue est connu
- Affichage et sauvegarde du diagramme Ns-Ds

## Formules utilisées

Travail adiabatique :

    Delta_H_ad = gamma * R * T1 / (gamma - 1) * [ (P2/P1)^((gamma - 1)/gamma) - 1 ]

Vitesse spécifique :

    Ns = N * sqrt(Q) / H_ad^(3/4)

Diamètre spécifique :

    Ds = D * H_ad^(1/4) / sqrt(Q)

## Données d’entrée

Le programme demande :

- le débit volumique Q en m3/s ;
- la pression d’entrée P1 en bar ;
- la pression de sortie P2 en bar ;
- la température d’entrée T1 en K ;
- la vitesse de rotation N en tr/min ;
- le gaz utilisé.

## Gaz disponibles

- Air
- Hélium
- CO2
- Azote N2
- Gaz personnalisé

## Types de compresseurs considérés

Le programme classe le point de fonctionnement dans l’une des familles suivantes :

- compresseur volumétrique : piston, scroll, vis ;
- compresseur centrifuge ou radial ;
- compresseur mixte ou hélico-centrifuge ;
- compresseur axial ;
- soufflante ou ventilateur axial.

## Utilisation

Installer les dépendances :

    pip install numpy matplotlib

Lancer le programme :

    python compressor_ns_ds.py

Le programme peut générer une image du diagramme :

    compressor_ns_ds.png

## Remarque importante

Cet outil est destiné à l’apprentissage et au pré-dimensionnement.

Il ne remplace pas un dimensionnement industriel complet. Pour un design réel, il faut aussi prendre en compte les pertes, le rendement réel, les contraintes mécaniques, le nombre d’étages, les limites de Mach et la validation CFD.
