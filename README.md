# Projet5_ROBVIS
# PACO Mobile Platform - Simulation in CoppeliaSim
Ce projet repose sur un robot mobile à roues Mecanum, équipé d'une plateforme élévatrice. Deux versions sont disponibles :

### Auteur：Siyi LIN, Xudong YANG, Yujia ZHANG, Ruying JI

### 1. Version manuelle avec interface utilisateur (Version2.ttt)
Contrôle par boutons via une interface graphique.


### 2. Version autonome (Version_Complete.ttt)
Cette version exécute automatiquement une séquence d’actions dès le lancement de la simulation, sans intervention de l'utilisateur. Elle est conçue pour tester le déplacement, le contrôle proportionnel (P) et le mouvement de la plateforme élévatrice.

#### Séquence automatique :
1. Avancer de **1 mètre en ligne droite** (avec régulation proportionnelle)
2. **Se déplacer latéralement vers la gauche sur 1 mètre**
3. **Rotation horaire sur place de 90°** (avec intégration angulaire)
4. **Mouvement holonomique** : vx = 0.8, vy = 0.8, omega = 0.5 pendant 20 secondes
5. **Élévation de la plateforme à 0,15 mètre** (avec contrôle proportionnel de vitesse)
6. Arrêt complet du robot

Chaque phase inclut une vérification de la stabilité (position/angle/vitesse) avant d’enchaîner sur la suivante.


## Instructions d’utilisation

### Version manuelle :
1. Ouvrir `Version2.ttt`
2. Lancer la simulation (▶️)
3. Utiliser l’interface graphique pour commander le robot et la plateforme

### Version autonome :
1. Ouvrir `Version_Complete.ttt`
2. Démarrer la simulation, le scénario démarre automatiquement

