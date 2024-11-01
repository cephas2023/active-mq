--ACTIVE MQ--

--CVE_2015--

-Vulnérabilité:
Cette version d'active_mq contient deux vulnérabilités assez remarquables qui sont l'absence d'une authentifiaction pour l'accès au site et le fait de pouvoir y insérer plusieurs types de données.

-Solution:
Mettre en place un système d'authentification et/ou de vérifiaction des inputs afin d'éviter les injections SQL etc...

--CVE_2016--

-Vulnérabilté:
Cette version d'active_mq ne neutralise pas ou neutralise de manière incorrecte les entrées de données par l'utilisateur avant qu'elles ne soient misent dans une sortie utilisée comme page web servie à d'autres utilisateurs.

-Solution:
Pour cette vulnérabilité, nous pouvons metrre en place un mécanisme qui vérifie les données qu'envoie l'utilisateur, cette solution rejoint un peu celle proposée pour la CVE_2015

--CVE_2022--:

-Vulnérabilité:
Cette version d'active_mq n'effectue pas une classification (Vérifiaction de la source d'une donnée) de données avant de le mettre à la dispostion d'autres utilisateurs.

-Solutions;
Utiliser un Safe Constructor : Si vous utilisez des bibliothèques comme SnakeYaml pour traiter les messages, optez pour un Safe Constructor qui limite les types d'objets qui peuvent être créés lors de la désérialisation.
Configurer les permissions : Limitez les permissions des utilisateurs et des applications qui peuvent accéder aux files d'attente pour réduire les risques d'attaques.

--CVE_2023--

-Vulnérabilité:
Controles d'accès au site

-Solutions:
La solution à cette vulnérabilité peut être la mise en place d'u système d'authentifiaction pour les différents accès.
