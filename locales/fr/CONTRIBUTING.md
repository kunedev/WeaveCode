# Contribuer à Weavy

Nous sommes ravis que vous soyez intéressé à contribuer à Weavy. Que vous corrigiez un bug, ajoutiez une fonctionnalité ou amélioriez notre documentation, chaque contribution rend Weavy plus intelligent ! Pour maintenir notre communauté dynamique et accueillante, tous les membres doivent adhérer à notre [Code de Conduite](CODE_OF_CONDUCT.md).

## Rejoindre Notre Communauté

Nous encourageons fortement tous les contributeurs à rejoindre notre [communauté Discord](https://discord.gg/roocode) ! Faire partie de notre serveur Discord vous aide à :

- Obtenir de l'aide et des conseils en temps réel sur vos contributions
- Vous connecter avec d'autres contributeurs et membres de l'équipe principale
- Rester informé des développements et priorités du projet
- Participer aux discussions qui façonnent l'avenir de Weavy
- Trouver des opportunités de collaboration avec d'autres développeurs

## Signaler des Bugs ou des Problèmes

Les rapports de bugs aident à améliorer Weavy pour tout le monde ! Avant de créer un nouveau problème, veuillez [rechercher parmi les existants](https://github.com/RooVetGit/Roo-Code/issues) pour éviter les doublons. Lorsque vous êtes prêt à signaler un bug, rendez-vous sur notre [page d'issues](https://github.com/RooVetGit/Roo-Code/issues/new/choose) où vous trouverez un modèle pour vous aider à remplir les informations pertinentes.

<blockquote class='warning-note'>
     🔐 <b>Important :</b> Si vous découvrez une vulnérabilité de sécurité, veuillez utiliser <a href="https://github.com/RooVetGit/Roo-Code/security/advisories/new">l'outil de sécurité Github pour la signaler en privé</a>.
</blockquote>

## Décider Sur Quoi Travailler

Vous cherchez une bonne première contribution ? Consultez les issues dans la section "Issue [Unassigned]" de notre [Projet Github Weavy Issues](https://github.com/orgs/RooVetGit/projects/1). Celles-ci sont spécifiquement sélectionnées pour les nouveaux contributeurs et les domaines où nous aimerions recevoir de l'aide !

Nous accueillons également les contributions à notre [documentation](https://docs.roocode.com/) ! Qu'il s'agisse de corriger des fautes de frappe, d'améliorer les guides existants ou de créer du nouveau contenu éducatif - nous aimerions construire un référentiel de ressources guidé par la communauté qui aide chacun à tirer le meilleur parti de Weavy. Vous pouvez cliquer sur "Edit this page" sur n'importe quelle page pour accéder rapidement au bon endroit dans Github pour éditer le fichier, ou vous pouvez plonger directement dans https://github.com/RooVetGit/Roo-Code-Docs.

Si vous prévoyez de travailler sur une fonctionnalité plus importante, veuillez d'abord créer une [demande de fonctionnalité](https://github.com/RooVetGit/Roo-Code/discussions/categories/feature-requests?discussions_q=is%3Aopen+category%3A%22Feature+Requests%22+sort%3Atop) afin que nous puissions discuter si elle s'aligne avec la vision de Weavy. Vous pouvez également consulter notre [Feuille de route du projet](#feuille-de-route-du-projet) ci-dessous pour voir si votre idée s'inscrit dans notre orientation stratégique.

## Feuille de route du projet

Weavy dispose d'une feuille de route de développement claire qui guide nos priorités et notre orientation future. Comprendre notre feuille de route peut vous aider à :

- Aligner vos contributions avec les objectifs du projet
- Identifier les domaines où votre expertise serait la plus précieuse
- Comprendre le contexte derrière certaines décisions de conception
- Trouver de l'inspiration pour de nouvelles fonctionnalités qui soutiennent notre vision

Notre feuille de route actuelle se concentre sur six piliers clés :

### Support des fournisseurs

Nous visons à prendre en charge autant de fournisseurs que possible :

- Support plus polyvalent pour "OpenAI Compatible"
- xAI, Microsoft Azure AI, Alibaba Cloud Qwen, IBM Watsonx, Together AI, DeepInfra, Fireworks AI, Cohere, Perplexity AI, FriendliAI, Replicate
- Support amélioré pour Ollama et LM Studio

### Support des modèles

Nous voulons que Roo fonctionne aussi bien que possible avec autant de modèles que possible, y compris les modèles locaux :

- Support des modèles locaux via des prompts système personnalisés et des flux de travail
- Évaluations de benchmarking et cas de test

### Support des systèmes

Nous voulons que Roo fonctionne bien sur l'ordinateur de chacun :

- Intégration de terminal multiplateforme
- Support solide et cohérent pour Mac, Windows et Linux

### Documentation

Nous voulons une documentation complète et accessible pour tous les utilisateurs et contributeurs :

- Guides utilisateur et tutoriels étendus
- Documentation API claire
- Meilleure orientation pour les contributeurs
- Ressources de documentation multilingues
- Exemples interactifs et échantillons de code

### Stabilité

Nous voulons réduire considérablement le nombre de bugs et augmenter les tests automatisés :

- Interrupteur de journalisation de débogage
- Bouton de copie "Informations machine/tâche" pour l'envoi avec les demandes de support/bug

### Internationalisation

Nous voulons que Roo parle la langue de tous :

- 我们希望 Weavy 说每个人的语言
- Queremos que Weavy hable el idioma de todos
- हम चाहते हैं कि Weavy हर किसी की भाषा बोले
- نريد أن يتحدث Weavy لغة الجميع

Nous accueillons particulièrement les contributions qui font progresser nos objectifs de feuille de route. Si vous travaillez sur quelque chose qui s'aligne avec ces piliers, veuillez le mentionner dans la description de votre PR.

## Configuration de Développement

1. **Clonez** le dépôt :

```sh
git clone https://github.com/RooVetGit/Roo-Code.git
```

2. **Installez les dépendances** :

```sh
npm run install:all
```

3. **Démarrez la vue web (application Vite/React avec HMR)** :

```sh
npm run dev
```

4. **Débogage** :
   Appuyez sur `F5` (ou **Exécuter** → **Démarrer le débogage**) dans VSCode pour ouvrir une nouvelle session avec Weavy chargé.

Les modifications apportées à la vue web apparaîtront immédiatement. Les modifications apportées à l'extension principale nécessiteront un redémarrage de l'hôte d'extension.

Vous pouvez également créer un fichier .vsix et l'installer directement dans VSCode :

```sh
npm run build
```

Un fichier `.vsix` apparaîtra dans le répertoire `bin/` qui peut être installé avec :

```sh
code --install-extension bin/roo-cline-<version>.vsix
```

## Écrire et Soumettre du Code

Tout le monde peut contribuer avec du code à Weavy, mais nous vous demandons de suivre ces directives pour vous assurer que vos contributions puissent être intégrées en douceur :

1. **Gardez les Pull Requests Ciblées**

    - Limitez les PRs à une seule fonctionnalité ou correction de bug
    - Divisez les changements plus importants en PRs plus petites et liées
    - Divisez les changements en commits logiques qui peuvent être examinés indépendamment

2. **Qualité du Code**

    - Toutes les PRs doivent passer les vérifications CI qui incluent à la fois le linting et le formatage
    - Résolvez toutes les alertes ou erreurs ESLint avant de soumettre
    - Répondez à tous les retours d'Ellipsis, notre outil automatisé de revue de code
    - Suivez les meilleures pratiques TypeScript et maintenez la sécurité des types

3. **Tests**

    - Ajoutez des tests pour les nouvelles fonctionnalités
    - Exécutez `npm test` pour vous assurer que tous les tests passent
    - Mettez à jour les tests existants si vos changements les affectent
    - Incluez à la fois des tests unitaires et d'intégration lorsque c'est approprié

4. **Directives pour les Commits**

    - Écrivez des messages de commit clairs et descriptifs
    - Référencez les issues pertinentes dans les commits en utilisant #numéro-issue

5. **Avant de Soumettre**

    - Rebasez votre branche sur la dernière main
    - Assurez-vous que votre branche se construit avec succès
    - Vérifiez à nouveau que tous les tests passent
    - Revoyez vos changements pour détecter tout code de débogage ou logs de console

6. **Description du Pull Request**
    - Décrivez clairement ce que font vos changements
    - Incluez des étapes pour tester les changements
    - Listez tous les changements incompatibles
    - Ajoutez des captures d'écran pour les changements d'interface utilisateur

## Accord de Contribution

En soumettant une pull request, vous acceptez que vos contributions soient sous licence selon la même licence que le projet ([Apache 2.0](../LICENSE)).
