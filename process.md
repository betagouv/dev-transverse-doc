# Process
Ce document vise à définir des guidelines pour travailler au mieux sur nos projets en commun.
Ces guidelines sont là pour nous simplifier la vie sur le longtemps terme.

## Attribution d'une tache et PR 

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
9. demander une review à une ou plusieurs personne sur github [(voir review)](#process-de-review)
10. dès que la PR est prête, partagez la sur le channel publique du projet en pinguant le reviewer (ou sur #dinum-dev-transverse)
11. review [(voir review)](#process-de-review)
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

on attribue la review à une ou plusieurs personnes dont au moins une qui connait bien le code du projet.
On peut ajouter:
- review design par un designer si travail sur l'ux avec ce designer en amont,
- review falcultative a un autre dev (avec qui on a discuté du sujet, qui embarque sur le projet, ou qui souhaite d'avantage se l'approprier, ou autre)

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

### Gestion des taches : 

Github projet, trello, ou autre selon le projet.
On essaye de redécouper des taches en sous taches si le ticket propose divers changements avant de se lancer dessus.

- S'assigner sur les cards quand on travaille dessus
- Mettre la card dans la bonne colonne en fonction de son avancement quand on travaille dessus
- Lier les PR relatives à la card en question



