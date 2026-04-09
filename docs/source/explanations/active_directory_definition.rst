.. _active_directory_definition:

Qu'est ce qu'Active Directory ?
===============================

Définition
----------

Active Directory est le service d'annuaire développé par Microsoft depuis 1999 pour les environnements Windows Server. Il fournit une structure centralisée permettant de gérer les identités, les ordinateurs et les ressources réseau au sein d'une organisation.

Dans une entreprise moderne, il y a presque toujours Active directory. 

Rôles principaux
----------------

L'Active Directory remplit plusieurs fonctions vitales :

* **Gestion des utilisateurs** : Centralisation des comptes et des identités.
* **Contrôle des accès** : Gestion fine des connexions au réseau.
* **Administration des machines** : Gestion du parc informatique (postes et serveurs).
* **Définition des permissions** : Attribution des droits sur les ressources.

Le défi de la sécurité moderne
------------------------------

Conçu il y a plus de vingt ans, le système a été pensé dans un contexte où les enjeux de cybersécurité étaient très différents. Si les menaces ont radicalement évolué, les configurations d'Active Directory restent souvent inchangées, favorisant parfois la facilité d'utilisation au détriment de la sécurité.

Les vulnérabilités courantes
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* **Progression latérale** : Les attaquants exploitent les relations entre les éléments du système pour atteindre les ressources critiques comme les contrôleurs de domaine.
* **Gestion des accès privilégiés** : Des utilisateurs intermédiaires disposent souvent de droits sensibles sans réelle maîtrise globale.
* **Accès en lecture par défaut** : Le système permet souvent d'accéder à des informations sensibles qui aident un attaquant à cartographier le réseau.

Le risque lié aux listes de contrôle d'accès (ACL)
-------------------------------------------------

Les ACL sont souvent complexes et mal configurées. Cela crée des chemins indirects vers des privilèges élevés :

* Un utilisateur non-administrateur peut posséder des permissions lui permettant de devenir administrateur.
* **Exemple type** : Un compte support technique capable de réinitialiser le mot de passe d'un compte critique.



Ainsi, la sécurité d’Active Directory ne dépend pas uniquement de la protection des comptes les plus sensibles, mais de l’ensemble des relations et des permissions qui structurent le système. Cette complexité rend difficile l’identification des failles et explique pourquoi Active Directory reste une cible majeure pour les cyberattaques.

----

**Source :** *Darren Mar-Elia, d'après les analyses publiées sur Semperis.*
`<https://www.semperis.com/fr/blog/tools-attacking-active-directory/>`_