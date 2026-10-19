# Obstacles d'observés

- Emilien DUCIEL
- Samuel MARTINEZ

## 1. Ouverture impossible

**Problème** : 
- Le bouton "Réserver" était un div avec la classe fakebutton

**Impact** :
- Non focusable au clavier, aucun tab ne l'atteint
- Non activable avec Entrée/Espace
- Aucune lecture par voiceover

=> Utilisateurs clavier et lecteurs d'écran exclus de la réservation

---

## 2. Nom accessible du modal

**Problème** :
- Le modal n'avait pas de role="dialog" ni de lien vers son titre

**Impact** :
- Le voiceover ne lit pas le titre du modal
- L'utilisateur ne sait pas où il se trouve ni le contexte
- Utilisateur est perdu dans la page

=> Modal inaccessible aux voiceover et aux claviers

---

## 3. Focus et fermeture

**Problème** :
- Le focus ne rentrait pas dans le modal à l'ouverture
- Impossible de fermer avec Échap
- Le bouton de fermeture n'avait pas de label et n'était pas focusable
- Le focus ne revenait pas au site après fermeture

**Impact** :
- L'utilisateur clavier reste bloqué à l'ouverture du modal
- Impossible de naviguer ou fermer sans souris
- Perte de contexte après fermeture si voiceover ou clavier
- Le contenu derrière reste tabulable quand ouvert