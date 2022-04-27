## Documentation GitHub CI/CD


### Intéret des tests unitaires sur le code 

  Un test unitaire permet de s'assurer du fonctionnement correct d'une partie déterminée d'une application ou d'une partie d'un programme. Il a pour objectif d'isoler le comportement de la partie de code à tester de tout facteur extérieur et de vérifier qu'il est conforme à ce qui est attendu.
  Les tests unitaires sont la base sur laquelle les autres processus de tests (tests fonctionnels, d’intégration, de régression, de performance…) doivent être construits pour assurer des fondations solides dans le cadre du développement d'une application.

 ![image](https://cdn.sanity.io/images/kjg6yd05/production/3248e3f6e9f5af465032b699544538cbbdf9b8a3-466x246.png?w=750&fit=clip)


### Tests de Sécurité

Pour les tests de sécurité, nous avons opté pour les tests Trivy, dans sa version de base, c'est à dire qu'il scan tous le repository github, sans utilisé l'outil "docker" car cela etait plus simple a mettre en place, même si en utilisant "docker", cela rendrait tous le fonctionnement plus optimiser. 

### Difficultés rencontrés

Pour mener a bien ce projet, nous avons rencontré plusieurs difficultés, notamment celles qui sont venus le plus régulièrement étaient dû a un problème d'authentification sur github, ainsi que des problèmes de droits sur le pc. Nous avons aussi rencontré des problèmes pour lier sonarcloud(tests qualité) à github car nous parvenions pas à récupérer le token que sonarclound devait créer et ne le faire apparaître afin de le lier avec le repository github. Pour finir, nous avons rencontré une dernière difficulté lorsqu'on a utilisé les tests unitaires car le le fichier "karma.conf.js" était mal configuré et nous empéchais donc de réaliser les tests unitaires.

### Types de déploiements possibles et utilisé

Ils existent une multitude de déploiement possibles, nous avons pu essayer deux d'entre, Dokku et Heroku, nous avons choisi de deployer sur Heroku car il s'agit du seul qui est gratuit. Heroku est une plateforme en tant que service basée sur le cloud. Cela permet d'envoyer une application sur un serveur qui permet de faciliter le developpement d'applications plus fiables. Heroku peut aider à se concentrer davantage sur la création et la livraison d’applications en continu, sans être distraits par l’infrastructure ou le serveur. 

### L'état de l'art d'un pipeline
