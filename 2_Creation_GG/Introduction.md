# INTRODUCTION

---

Dans la gestion d’un système d’information structuré, la création des groupes globaux (GG) constitue une étape essentielle pour organiser les habilitations et assurer une administration cohérente des accès. Les groupes globaux permettent de regrouper les utilisateurs partageant les mêmes besoins fonctionnels ou appartenant au même service, tout en facilitant l’application du modèle AGDLP mis en place dans l’infrastructure Active Directory. Grâce à cette approche, les droits ne sont plus attribués individuellement, mais de manière centralisée et homogène, ce qui renforce la sécurité et simplifie la maintenance du domaine.

La création des groupes globaux s’inscrit directement dans la continuité de la gestion des comptes utilisateurs. Une fois les collaborateurs intégrés dans l’annuaire, il devient indispensable de les associer à des groupes correspondant à leurs rôles, leurs responsabilités ou leurs accès métiers. Cette méthode permet d’éviter les erreurs d’attribution, de garantir une traçabilité claire et d’assurer une évolution simple des habilitations en cas de changement de poste ou d’arrivée d’un nouvel utilisateur.

---

## Procédure création des GG :

La procédure utilisée est la suivante  :

1. Aller dans : OU_Groupes → GG 

2. Clic droit → Nouveau → Groupe 

3. Renseigner : 

- Nom du Groupe Global (ex : GG_RH) 

- Portée : Global 

- Type : Sécurité 

4. Valider. 

---

## Tableau récapitulatif :

| Services              | OU_Groupes  | GG         |
|-----------------------|-------------|------------|
| Ressources Humaines   | GG          | GG_RH      |
| Informatique          | GG          | GG_INF     |
| Comptabilité          | GG          | GG_CP      |

---

## Procédure ajout des utilisateurs :

La procédure utilisée est la suivante :

1. Aller dans l’OU contenant l’utilisateur (ex : Utilisateur_RH) 

2. Clic droit sur l’utilisateur (ex : Placide) 

3. Sélectionner Ajouter au groupe 

4. Entrer le groupe global (ex : GG_RH)

---

## Tableau récapitulatif :

| Services              | OU_Groupes   | OU_Utilisateurs   | Utilisateur  |
|-----------------------|--------------|-------------------|--------------|
| Ressources Humaines   | GG_RH        | Utilisateur_RH    |  Placide     |
| Informatique          | GG_INF       | Utilisateur_INF   |  Fortuné     |
| Comptabilité          | GG_CP        | Utilisateur_CP    |  Hugues      |

