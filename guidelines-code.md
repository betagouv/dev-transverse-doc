# Guidelines de Code

> Ces guidelines sont là pour nous simplifier la vie sur le longtemps terme.

## Concept de développement
- Utiliser un maximum de fonction pure
- Séparation des préoccupations (Separation of concerns) : https://fr.wikipedia.org/wiki/S%C3%A9paration_des_pr%C3%A9occupations
- Convention plutôt que configuration (Convention over configuration) : https://fr.wikipedia.org/wiki/Convention_plut%C3%B4t_que_configuration
- The Boy Scout Rule : "Always leave the campground cleaner than you found it." https://www.oreilly.com/library/view/97-things-every/9780596809515/ch08.html
- Les noms de variables, noms de méthodes sont en anglais(sauf les termes francais intraduisibles) et très explicite (éviter les abréviations)
- Ne faire de référence circulaire
- Penser à la loi de murphy (Si ça peut tourner mal, statistiquement ça va arriver)

## Git
- Une branche pour chaque développement 
   - feature/123-feature-name-card : Ajout d'un nouvelle fonctionnalité
   - task/234-task-name : Refactoring ou modification d'une fonctionnalité existante
   - fix/125-fix-name : Correction d'un bug
- Pull request pour chaque développement
   - On peut regrouper dans une même PR des taches ou fonctionnalités similiares
   - Une PR ne peut pas représenter plus d'une journée de boulot (sans inclure les reviews)
   - Nom de la "Nom de la fonctionnalité/tache" -> Un truc facile à mettre dans un Changelog
   - Dans le descriptif de la PR : mettre la liste des changements et des éléments à tester pour le reviewer
   - Mettre des captures d'écran pour les changements visuels
   - Demander à un membre de l'équipe non développeur de tester les nouvelles fonctionnalités
   - Avoir une review ou un go d'un autre développeur avant de merger
  
