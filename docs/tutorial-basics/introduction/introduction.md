---
sidebar_position: 2
---

# Problématique


### AWS le premier cloud provider:

Dans un temps que les moins de 15 ans ne pouvaient pas connaitre... il existait de nombreuses problématiques pour hébergé les différents services.

La facilité de déploiement n’était pas aussi développé que maintenant. L’ajout d’un serveur était couteux puisqu’il fallait faire intervenir une action manuelle (pour les branchements, la configuration, etc…).

En 2004 Amazon annonce le lancement de AWS (https://aws.amazon.com/fr/blogs/aws/welcome/) pour un usage publique, il sera disponible aux clients vers la fin d'année 2006 (la plateforme était déjà utilisé pour les projets internes).

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">I have this old 2006 BusinessWeek framed as a reminder. The “risky bet” that Wall Street disliked was AWS, which generated revenue of more than $62 billion last year. <a href="https://t.co/ccF0nCOkhu">pic.twitter.com/ccF0nCOkhu</a></p>&mdash; Jeff Bezos (@JeffBezos) <a href="https://twitter.com/JeffBezos/status/1527003895393812480?ref_src=twsrc%5Etfw">May 18, 2022</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script> 

*La une du « BusinessWeek » de 2006 sur AWS, aujourd’hui c’est plus de 62 milliards de CA.*

Voici une liste des différents services avec les dâtes:

| Année |          Service          |   Type    |
|:------|:-------------------------:|:---------:|
| 2006  |            S3             |  Storage  |
| 2006  |            SQS            | Messaging |
| 2007  | EC2 unlimited public beta |  Compute  |


### GCP et Azure et les autres:

GCP est officiellement annoncé en 2008 avec Google App Engine en version beta. Microsoft annoncera le projet Microsoft Azure en 2008 également.

Aujourd’hui il existe beaucoup de cloud providers qui proposent le même type de service, pour en citer quelques uns:
* OVH
* AlibabaCloud
* Scaleway

## Pourquoi est-ce une évolution dans notre métier

### Rapidité
Aujourd’hui nous avons besoin de délivrer vite et d’une façon plus agile. Les projets de quelques années se font de plus en plus rare et nous souhaitons ne pas être bridé par des briques techniques trop bases. Le Cloud computing répond à cette attente:
* Les services sont facilement deployable, ce sont des objets.
* Les cloud providers proposent des services rapide à mettre en place, quasiment sans délais.
* Vous pouvez grâce à leur infrastructure déployer rapidement sur toutes les régions géographiques.

### Sécurité
Nous avons aussi besoin de sécurité, les cloud providers répondent à des normes strictes en matières de sécurité.
* La protection des Datacenter
* La protection contre des risques naturelles
  Mais ils nous permettent aussi de mieux géré la sécurité de notre infrastructure avec différentes prissions que nous verrons plus tard dans le module:
* Un utilisateur A n’a le droit que de lecture sur mes Object Storage
* Un utilisateur B bien défini peut lui modifier les propriétés
* Toutes ses règles c’est à nous de les définir. Ce qui permet de répondre à un principe de la culture DevOps : « You build it, you run it! »

### Scalabilité
Grace aux grosses infrastructures nous pouvons étendre nos services avec la croissance de l’utilisation de ceux-ci. Admettons que monsieur A à un blog, il a besoin de plus de resources car il fait des articles interessant (comme un cours sur GCP par exemple:)), alors monsieur A peut augmenter la taille de sa machine virtuelle en toute facilité et sans casser sa stack technique (cela à évidemment des limites mais concentrons nous sur un exemple simple). Grace au cloud provider, monsieur A peut:
* Rendre disponible son blog en Asie facilement
* Augmenter la taille de son infrastructure facilement
  Finalement il n’y a que très peut de limite sur la scalabilité, si ce n’est l’argent dépensé dans les cloud providers!

### Note:

Les cloud providers peuvent vous paraitre cher à premier vu quand on compare par exemple une VM Kimsuffi (VPS Starter : 4E TTC/m - 1CPU / 2GO ram) à une VM Azure de même type : Standard_A1_v2 ([[] https://azureprice.net/vm/Standard_A1_v2 ]: 31$/m HT).
Rappelez vous que les cloud providers permettent de faciliter et de disposer de l’infrastructure Azure. Kimsufi ne propose pas des services de Queues par exemple.
De plus les cloud providers sont plus à destination d’un usage professionnel.

* Combien coute une personne pour configurer la VM?
* Combien coute une personne pour configurer proprement le réseau, intégré un Firewall, avoir des updates de sécurité, avoir une infra résiliante ?

(Le Cloud computing ne correspond pas à tous les usages, il faut être contient de cela, ce n’est pas non plus une solution magique à tous vos problèmes. Un problème de performance ne sera surement pas réglé si vous migrez votre application d’OVH vers GCP avec la même taille de compute par exemple).
