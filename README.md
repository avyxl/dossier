# dossier
# dossier

**dossier** est une plateforme de partage de texte et de « paste » entièrement sécurisée, pensée pour celles et ceux qui veulent échanger des informations sensibles sans compromis sur la confidentialité. tout y est chiffré, de bout en bout, dans un environnement fermé et maîtrisé.

---

## présentation

dossier permet de créer, stocker et partager des extraits de texte, des notes, des fragments de code, des configurations ou tout autre contenu confidentiel, via un simple lien. contrairement aux services de paste classiques, dossier part d'un principe simple : le contenu n'a pas à être lisible par qui que ce soit, hormis les personnes qui détiennent la clé.

chaque document est chiffré avant d'être enregistré. sans la clé de déchiffrement, le contenu reste illisible, même pour l'hébergeur du service.

---

## chiffrement

### aes-256

dossier utilise l'algorithme **aes-256** (advanced encryption standard, clé de 256 bits), l'un des standards de chiffrement symétrique les plus robustes et les plus largement éprouvés au monde. il est employé par les administrations, les institutions financières et les systèmes de sécurité les plus exigeants. avec une clé de 256 bits, une attaque par force brute est, en pratique, irréalisable avec les moyens de calcul actuels.

### cryptkey

au cœur du système se trouve la **cryptkey**, la clé de chiffrement associée à chaque document. elle est :

- **unique** : une cryptkey distincte est générée pour chaque paste ;
- **aléatoire** : elle est produite à partir d'une source d'entropie cryptographiquement sûre ;
- **indispensable** : sans elle, le déchiffrement est impossible ;
- **maîtrisée par l'utilisateur** : c'est à vous de décider avec qui vous la partagez.

la cryptkey fait office de véritable clé d'accès : le lien seul ne suffit pas, il faut aussi la cryptkey pour accéder au contenu.

---

## fonctionnalités principales

- **chiffrement intégral** : le contenu est protégé par aes-256 avant tout stockage.
- **partage par lien sécurisé** : partagez un document en envoyant simplement son lien et sa cryptkey.
- **environnement fermé** : l'accès aux données est strictement cloisonné, afin de limiter toute exposition inutile.
- **simplicité d'utilisation** : une interface épurée, sans inscription compliquée, pour créer un paste en quelques secondes.
- **confidentialité par conception** : aucune lecture du contenu en clair n'est nécessaire au fonctionnement du service.
- **partage de texte et de code** : notes, journaux, extraits de code, fichiers de configuration, identifiants temporaires, etc.

---

## cas d'usage

- transmettre un mot de passe ou un jeton d'accès à un collègue.
- partager un extrait de code ou un journal d'erreurs sans l'exposer publiquement.
- échanger des notes confidentielles entre plusieurs personnes.
- conserver temporairement des informations sensibles de manière sécurisée.
- remplacer les services de paste publics, là où la confidentialité n'est pas garantie.

---

## principes de sécurité

1. **le chiffrement d'abord** : aucune donnée n'est stockée sans avoir été chiffrée.
2. **la clé reste sous votre contrôle** : la cryptkey est l'unique moyen de déchiffrer un document.
3. **la minimisation des données** : dossier ne collecte que le strict nécessaire.
4. **la transparence** : le code source est ouvert à l'examen, car la confiance se construit sur la vérification.

---

## avertissement

aucun système n'est infaillible. la sécurité de vos documents dépend aussi de la manière dont vous protégez et partagez votre cryptkey. si la cryptkey est perdue, le contenu chiffré ne peut pas être récupéré. partagez-la toujours par un canal de confiance.

---

## contribuer

les contributions sont les bienvenues. si vous repérez une faille, un bogue ou une amélioration possible, n'hésitez pas à ouvrir une *issue* ou à proposer une *pull request*. pour tout signalement de vulnérabilité, merci de contacter le mainteneur de façon privée avant toute divulgation publique.

---

## licence

ce projet est distribué sous la licence de votre choix. consultez le fichier `license` pour plus de détails.

---

**dossier** : vos mots, vos données, votre clé.
