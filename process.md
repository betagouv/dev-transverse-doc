# Process
Ce document vise à définir des guidelines pour travailler au mieux sur nos projets en commun.
Ces guidelines sont là pour nous simplifier la vie sur le longtemps terme.

## Process Attribution d'une tache et PR 

Quel est le processus pour travailler sur la tache ?
1. S'assurer que la tache est bien définie
1. on s'assigne la tache (sur github/trello)
2. on la déplace dans le board en `doing` (a voir quel outils utilisés)
3. on crée une branche (definir des conventions de nommage) - qu'on peut déjà pousser sur github même si toujours en brouillon (mettre en draft)
4. on code (définir l'approche sur le refacto, le tdd)
5. les tests en local doivent passer (TDD for the win)
6. on push, et on fait une pull request (peut être aussi fait au tout début - même si il n'y a aucune modif)
7. si les test CI passent, faire sa propre relecture de code, en ajoutant les explications qui nous ont fait prendre des décisions (lien stackoverflow, documentation, ...) si besoin dans l'optique de la review pour éviter un aller retour inutile
8. Pour les modifications apportées au front-end Web ou à l'application mobile, joindre des captures d'écran ou de courtes vidéos montrant l'application avant et après les modifications. (Cela simplifie la révision sans avoir à exécuter le code localement)
9. demander une review à une ou plusieurs personne sur github [(review)](#process-de-review)
10. dès que la PR est prête, partagez la sur le channel publique du projet en pinguant le reviewer (ou sur #dinum-dev-transverse)
11. review (voir ##  Process de review )
12. le merge peut se faire selon le sujet au choix:
- Le reviewer peut merger directement, ou
- ou il ping le `pull requester` ou un autre dev
    
### Lisibilité
- utiliser le français pour les pull requests et l'anglais pour le code et les commentaires dans le code, pour la contribution au logiciel libre universel
 

### Convention
- feature/123-feature-name-card : Ajout d'un nouvelle fonctionnalité
- task/234-task-name : Refactoring ou modification d'une fonctionnalité existante
- fix/125-fix-name : Correction d'un bug
    
## Process de review

### Qui review
Si la pull request est minime, typo, fix de documentation, on peut merge directement. On se fait confiance.

Sinon: 

on attribue la review à une ou plusieurs personnes dont au moins une qui connait bien le code projet.
- review design par un designer si travaille sur l'ux avec ce designer en amont,
- review falcultative a un autre dev (avec qui on a discuté du sujet, qui embarque sur le projet, ou qui souhaite d'avantage se l'approprier, ou autre, up to la personne qui fait la PR ?)

Le reviewer peut lui même demander une contre review, ou "passer" sa review, à une autre personne auquel cas il le mentionne sur la PR, et lui fait une request de review. 

### Temps de reviews
En terme de temps, la review devrait être faites dans le jour ouvré suivant la PR : 
    - dès que la PR est prête, partagez la sur le channel publique du projet en pinguant le reviewer (ou sur #dinum-dev-transverse)
    - Ne pas hésiter à pinger le reviewer si une demi journée s'est déjà écoulée. 
    - le reviewer peut assigner une autre personne si il ne peut pas respecter un délai respectable
    
### Role du reviewers 

Le reviewers peut fait des commentaires (facultatif), peut demander des changements, ou approuver la pull request.
Le reviewers peut faire des commentaires mineurs, de simples suggestions, mais quand même approuver la pull request.
Si des changements plus majeurs sont à faire, on reprends l'entièreté du processus de review.

[Conférence sur la relecture de code](https://www.youtube.com/watch?v=vyFHWS8rtDg), qui est une vraie compétence qui s'apprend comme coder.

### Le but/Process de la review:
- comprendre les motivations de la PR
- comprendre comment les changements ont été testés.
- célébrer les morceaux de codes qui vous inspirent (retours positifs)
- inviter à la discussion (slack/visio) pour accélerer la prise de décision si demande de clarifications
- Ils ne trouvent pas de défaut majeur dans les choix de conception technique.
- Ils trouvent les changements conformes aux pratiques habituelles de la communauté ou de l'équipage. 
- Ils ne voient aucune erreur évidente dans la mise en œuvre.
- Ils trouvent le code facile à comprendre dans la mesure du possible.
- Ils pourraient enquêter sur les problèmes liés au code, si quelque chose ne va pas.

### Gestion des taches : 

Un seul outil : github ou trello.

3 - Qu'utilise t-on pour le board ?

Savoir ou est le board. Pas d'outils définie, mais utilisé.
Trello ? Github Project ? 

On peut mettre ça dans le board de pipe.

Mettre un lien vers la carte trello dans la PR ? 



### Les autres outils :

### Qualité de code : 
# TDD

## Lucas
- scinder les board discussions et tache dev, imho ça apporterait de la clarté
- utiliser l'outils de discussions github pour ce qui est idées/etc... > transformer en issue quand la feature est définie

## Paul
- Lisibilité 
    - utiliser le français pour les pull requests / anglais pour le code (sauf commentaire ?)
    - se concentrer sur le pourquoi plutôt que le comment (selon nos bagages, ce n'est parfois pas évident pour tous)
    - ne pas craindre de dire : ce code n'est pas clair pour moi
    - faire sa propre relecture de code, en ajoutant les explications qui nous ont fait prendre des décisions (lien stackoverflow, documentation, ...)
- Outils repertoires github : couverture de code / qualité de code / mise à jour dépendance
    - Documenter nos [pratiques dans nos projets via CONTRIBUTING.md](https://github.com/github/docs/blob/main/CONTRIBUTING.md)
    - Mettre un [template de PR vers le lien vers nos pratiques](https://docs.github.com/en/free-pro-team@latest/github/building-a-strong-community/creating-a-pull-request-template-for-your-repository)
    - couverture de code : https://github.com/marketplace/codecov (à valider pour l'activer sur l'orga beta)
    - qualité de code : codacy.com (à valider pour l'activer sur l'orga beta)
    - dépendance: dependentBot (outil de base de github à activer il me semble, déjà actif sur secretariat par ex)
    - utiliser les badges (build passing etc.) de ces outils sur le readme pour les mettre en avant

## Emeline
- proposition review: assigner l'equipe Dev transverse aux reviews
    - histoire de pouvoir poser des questions sur le code et jeter un oeil.
    - la review n'est pas obligatoire si la personne n'est pas interessée.
    - Il faudrait au moins la review du lead assigné (a voir si il y en a un/plusieurs et qui c'est sur chaque projet).
- Pour les taches, 
    - choisir ensemble un seul outil de suivi (actions github, trello ou autre)
    - Bien s'assigner quand on commence une tache pour ne pas reprendre une tache déjà commencée 


## Julien

### Suggestions
- Découpage des taches à la demi-journée pour simplifier l'implémentation et la review (une tache trop longue vont demander beaucoup de coordinations et mettre beaucoup de temps à être mergé)
- Avant de dev : préparer les taches complexes en amont, en décrivant ce que l'on pense faire avec une petite liste d'action
    - Inclut la spec base de donnée s'il y a une nouvelle table ou modification
    - Demander un avis externe sur la spec
    - Développer après avis
- Suivant la taille de la PR 
    - Modification mineur (changement de texte, correction d'un mini bug) -> une seul personne peut review et l'un ou l'autre peut merger si c'est bon
    - Modification importante
        - Review design par un designer
        - Review par un dev aillant une bonne connaissance de ce morceau de code
        - Merge si'tout 
- Suggestion : Définir un lead par produit (la personne aillant la meilleur connaissance technique du produit)
    - Le lead voit s'il faut prendre plus d'avis ou pas
    - Son rôle est que la PR soit mergé le plus rapidement possible sans mettre en cause le produit
    - Le lead peut changer au cours du temps
- Ajouter un outil de couverture de code comme https://www.codacy.com/
- Dans la review, indiquer ce qui est bloquant pour merge de ce qui fait faire l'objet d'étude/modification ultérieur
- Trouver des grands principes, un ensemble de régle peut être difficile à appréhender. En réduisant à quelques principes avec des exemples, ça peut être plus facile.
- J'ai vu ça dans ma timeline ce matin, mais je n'ai pas encore lu : https://medium.com/alan/how-we-do-code-reviews-at-alan-eeeeef0a8d4f 

### Questions 
- Comment gérer un ensemble de tache sur plusieurs produits ? tout sur github ?

### Exemples
Voici un exemple de ce que je faisais sur A+ : 
- Guidline de code/dev https://github.com/betagouv/aplus/blob/master/docs/guidelines-code.md
- Design (faite par la designeuse du produit) https://github.com/betagouv/aplus/blob/master/docs/guidelines-design.md




