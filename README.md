# Agar.ia 3D

Agar.ia est un jeu vidéo développé en C++ par l'association PC[i], une version de Agar.io destiné a des IA

![Build linux](https://github.com/pci-ua/Agar.ia3D/actions/workflows/c-cpp.yml/badge.svg)

## Installation

#### Linux
1. Assurez-vous d'être à jour :

    ```bash
    sudo apt update
    sudo apt upgrade
    ```

2. Installez les dépendances :

    ```bash
    sudo apt install make g++
    sudo apt install qtchooser #Inutilisée pour l'instant
    sudo apt install qt5-default qtmultimedia5-dev build-essential freeglut3-dev #Inutilisée pour l'instant
    ```

3. Compilez le programme :
     ```bash
    make
    ```

#### Windows

 En préparation


## Création de votre IA

```c++
#include "../Modele/entitee/joueur.hh"

class Indila
/*
Tourner dans le vide, vide
Tourner dans le vide, il me fait tourner
*/
  :public Joueur {
private:
double i = 0;

public:
  Indila():Joueur(Couleur(120,250,30)) {}
  double deplacement() override {
    i+=0.1;
    return i;
  }
};
```

## Contribué
Pour l'instant toutes les contributions sont limités au groupes de développeur qui y sont affecté

## License
Pour l'instant aucune utilisiation (qu'elle soit personnel ou non,commercial ou non)
