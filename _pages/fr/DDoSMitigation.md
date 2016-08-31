---
layout: page
title: "Réponse aux attaques par déni de service distribué (DDoS)"
author: RaReNet
summary: " Cette section du Kit de premier secours numériques vous indique des mesures de base pour diagnostiquer les éventuels problèmes. Si votre site subit une attaque par déni de service, des possibilités d'action immédiates sont suggérées."
date: 2015-08
redirect_from: /fr/DDoSMitigation/
permalink: /fr/AttaquesDDoS/
parent: /fr/
---

# Réponse aux attaques par déni de service distribué (DDoS)

De nombreux journalistes, sites d'information et blogueurs indépendants sont confrontés à la menace de se voir baillonnés parce que leur site internet est désactivé ou vandalisé. Dans bien des cas, il peut s'agir d'un problème agaçant mais innocent mais parfois, cela peut être dû à une attaque «&nbsp;par déni de service&nbsp;» ou un piratage de site. Cette section du Kit de premier secours numériques vous indique des mesures de base pour diagnostiquer les éventuels problèmes. Si votre site subit une attaque par déni de service, des possibilités d'action immédiates sont suggérées.

D'une manière générale, il est important de savoir qu'il existe de nombreuses raisons expliquant que votre site internet ne fonctionne pas. Le plus souvent, c'est dû à des erreurs de programmation ou à des problèmes techniques rencontrés par l'entreprise hébergeant le site. Parfois, d'autres éléments comme des procédures judiciaires peuvent aussi amener un hébergeur à désactiver un site. Identifier le problème et les solutions possibles aux difficultés de votre site internet peut être compliqué si vous ne disposez pas de connaissances en matière d'hébergement. Par conséquent, quand c'est possible, la meilleure première réaction est de contacter une personne de confiance qui peut vous aider (votre webmaster, les personnes qui vous ont aidé à créer votre site, des employés si vous en avez et l'entreprise qui héberge votre site ou si aucune de ces options n'est disponible, [demandez de l'aide à une organisation en laquelle vous avez confiance](https://github.com/CIRCL/circl.lu/blob/master/web/circl/content/pub/dfak/SecureCommunication.md#seeking-and-providing-remote-help)).

Il est de bonne pratique de _contacter votre webmaster et l'hébergeur du site_ après vous être renseigné sur les difficultés fréquentes ci-dessous&nbsp;! Le problème que vous rencontrez peut ne pas avoir été signalé sur sa page d'état des services, peut être temporaire ou l'hébergeur peut ne pas être au courant du problème. Il est précieux d'entretenir de bonnes relations avec vos fournisseurs de service&nbsp;: soyez clair et poli et faites part des résultats de vos investigations en utilisant ces questions pour leur permettre d'identifier rapidement le problème.

Commencez par répondre à quelques questions simples&nbsp;:

Informations de base

- .Qui a créé votre site internet&nbsp;? Peuvent-ils vous aider&nbsp;?&nbsp;
- .Qui est votre hébergeur web&nbsp;? Il s'agit de l'entreprise fournissant le serveur sur lequel se trouve votre site web. Si vous ne savez pas, vous pouvez utiliser un outil comme http://www.whoishostingthis.com/.&nbsp;
- .Disposez-vous des informations de connexion ou de compte pour cet hébergeur&nbsp;?&nbsp;
- .Où avez-vous acheté votre nom de domaine&nbsp;? Dans certains cas, c'est aussi votre hébergeur web mais il peut s'agir d'une autre société.&nbsp;
- .Disposez-vous des informations de connexion pour le service de nom de domaine&nbsp;? Si ce n'est pas le cas, les retrouver constitue le premier pas pour récupérer votre site.&nbsp;
- .Qui d'autre a connaissance de ces informations de compte ou peut y avoir accès&nbsp;?&nbsp;

Informations de diagnostic

Il existe différentes raisons pour lesquelles votre site internet peut être indisponible&nbsp;: problème de réseau, problème lié aux règles de fonctionnement, problème d'hébergement, de blocage, de logiciel, de défacement ou de performance. La section ci-dessous explique ce qu'est chacun de ces problèmes et comment diagnostiquer celui que vous rencontrez.

- .Votre hébergeur web fonctionne mais votre site est indisponible&nbsp;? Vérifiez sur http://www.isup.me/&nbsp;: il se peut que votre site fonctionne mais que vous ne puissiez pas le voir. Ceci est un problème de réseau. Votre propre connexion internet peut dysfonctionner ou bloquer votre accès au site. Ceci peut aussi indiquer que votre compte a été désactivé&nbsp;: vous voyez un message de votre fournisseur d'hébergement internet&nbsp;? Votre site a pu être mis hors ligne pour des raisons de facturation, légales, des questions de droit d'auteur et de copyright ou d'autres raisons. Ceci est un problème lié aux règles de fonctionnement. Tout d'abord, assurez-vous que vos informations de facturation sont à jour et qu'il n'y a pas de sommes impayées sur votre compte d'hébergement ou votre nom de domaine. Si le message est dû à un problème juridique, les ressources diffusées par EFF, bien qu'elles se concentrent sur la législation de copyright des États-Unis, sont une source précieuse d'informations&nbsp;: https://www.eff.org/issues/bloggers/legal/liability/IP.&nbsp;
- .Votre site ne se charge pas du tout&nbsp;? Il se peut que votre hébergeur rencontre des problèmes, auquel cas votre problème est un problème d'hébergement. Pouvez-vous consulter le site internet de votre hébergeur&nbsp;? Veuillez noter qu'il ne s'agit pas du panneau d'administration de votre propre site mais de celui de l'entreprise ou de l'organisation qui héberge votre site. Cherchez sur un blog «&nbsp;d'état&nbsp;» (ex. status.dreamhost.com). Regardez aussi sur twitter.com si d'autres utilisateurs parlent d'indisponibilité de l'hébergeur&nbsp;: une simple recherche comme «&nbsp;(nom de l'entreprise) down&nbsp;» peut parfois révéler si d'autres personnes rencontrent le même problème.&nbsp;
- .Pouvez-vous consulter d'autres sites au contenu similaire au vôtre&nbsp;? Essayez de consulter des sites liés au vôtre ou traitant des mêmes sujets. Essayez aussi Tor (https://www.torproject.org/projects/gettor.html) ou Psiphon (https://psiphon.ca/products.php) pour accéder à votre site. Si ça marche, vous avez un problème de blocage&nbsp;: vous êtes toujours en ligne pour le reste du monde mais êtes censuré dans votre propre pays.&nbsp;
- .Vous voyez des messages d'erreur&nbsp;? Il peut s'agir d'un problème logiciel. Réfléchissez à tout changement récent que vous ou votre équipe avez effectué et contactez votre webmaster. Lui envoyer une capture d'écran, le lien vers la page avec laquelle vous avez des soucis et tout message d'erreur que vous voyez l'aidera à comprendre la cause possible du problème. Vous pouvez aussi copier les messages d'erreur et faire une recherche pour voir s'il existe une solution simple.&nbsp;
- .Vous voyez un site internet qui n'est pas le vôtre&nbsp;? Vous recevez un avertissement de votre navigateur internet concernant un logiciel malveillant (malware) sur votre site&nbsp;? Il peut s'agir d'un problème de défacement. Voir ci-dessous la marche à suivre&nbsp;: vous devrez collaborer avec votre fournisseur de service d'hébergement et consulter la section Piratage de compte.&nbsp;
- .Votre site ne se charge que par intermittence ou anormalement lentement&nbsp;? Il se peut que votre site soit dépassé par le nombre et la vitesse des requêtes de page qu'il reçoit. C'est un problème de performance. Cela peut être une «&nbsp;bonne nouvelle&nbsp;» dans la mesure où votre site est plus populaire et nécessite seulement des améliorations pour réagir à plus de lecteurs&nbsp;: cherchez dans les données d'analyse de fréquentation du site si vous voyez une tendance à long terme à la hausse. Demandez conseil à votre webmaster ou votre hébergeur. De nombreuses plateformes populaires de blog ou de gestion de contenu (Joomla, Wordpress, Drupal et autres) disposent de modules d'extension (plug-in) permettant de mettre votre site en cache localement et intègrent des CDN qui peuvent améliorer de façon spectaculaire la performance et la résilience du site. Beaucoup des solutions ci-dessous peuvent aussi contribuer à résoudre les problèmes de performance.&nbsp;

Premières mesures à prendre pour répondre au problème&nbsp;:

Quand vous êtes victime d'une attaque par déni de service

Si les diagnostics ci-dessus ne vous sont d'aucune utilité (ou que vous souffrez d'un _problème de performance_ grave), il se peut que votre site soit victime d'une _attaque «&nbsp;par déni de service&nbsp;»_ où un utilisateur malveillant (ou plusieurs) essaie d'accéder au site de façon répétée et rapide (grâce à des outils automatisés) et, ce faisant, bloque les utilisateurs légitimes. Parfois, un seul «&nbsp;attaquant&nbsp;» essaie cette stratégie contre votre site, ce qui ne pose habituellement pas trop problème, à moins que vous ne payiez pour la bande passante. Plus fréquente, l'attaque par déni de service «&nbsp;distribué&nbsp;» (DDoS) où l'attaquant utilise des milliers de machines sous son contrôle pour attaquer un site.

- .Étape 1&nbsp;: Contactez une personne de confiance qui peut vous aider (votre webmaster, les personnes qui vous ont aidé à créer votre site, des employés si vous en avez et l'entreprise qui héberge votre site).&nbsp;
- .Étape 2&nbsp;: En collaboration avec l'entreprise auprès de laquelle vous avez acheté votre domaine (comme EasyDNS, Network Solutions, GoDaddy), optez pour un Time to Live (TTL) d'1&nbsp;heure. Ceci peut aider à rediriger votre site beaucoup plus vite une fois qu'il est attaqué (la valeur par défaut est 72&nbsp;heures, soit trois jours). Ce paramètre se trouve souvent dans les propriétés «&nbsp;avancées&nbsp;» pour votre domaine, parfois dans l'enregistrement SRV ou enregistrement de service.&nbsp;
- .Étape 3&nbsp;: Déplacez votre site sur un service d'atténuation d'attaque DDoS. Voir https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-services pour une liste complète. Pour commencer&nbsp;: &nbsp;
  - .Deflect.ca&nbsp;
  - .Projet Shield de Google&nbsp;
  - .Projet Galileo de CloudFlare&nbsp;

- .Étape 4&nbsp;: Dès que vous avez repris le contrôle, réfléchissez à ce dont vous avez besoin et décidez soit d'adopter un fournisseur d'hébergement sécurisé soit de continuer simplement avec votre service d'atténuation d'attaque DDoS.&nbsp;

Quand vous êtes victime d'un défacement de site internet

- .Étape 1&nbsp;: Vérifiez qu'il s'agit d'un piratage malveillant de votre site. Une pratique désagréable mais légale consiste dans le fait d'acheter des noms de domaine récemment arrivés à expiration pour «&nbsp;pirater&nbsp;» leur fréquentation à des fins publicitaires. Il est très important de veiller au paiement à jour de votre nom de domaine.&nbsp;
- .Étape 2&nbsp;: Si votre site internet a subi un défacement, commencez par reprendre le contrôle de votre compte d'accès au site internet et par changer le mot de passe. Voir la section Piratage de compte.&nbsp;
- .Étape 3&nbsp;: Faites une sauvegarde du site vandalisé qui pourra être utilisée ensuite pour l'enquête sur le défacement.&nbsp;
- .Étape 4&nbsp;: Désactivez temporairement le site. Utilisez une simple page d'accueil ou une page «&nbsp;parking&nbsp;».&nbsp;
- .Étape 5&nbsp;: Déterminez comment votre site a été piraté. Votre hébergeur peut être en mesure de vous y aider. Parmi les problèmes fréquents, des parties anciennes de votre site sur lesquelles tournent des scripts ou outils personnalisés, des systèmes de gestion de contenu obsolètes et les programmes personnalisés contenant des failles de sécurité.&nbsp;
- .Étape 6&nbsp;: Restaurez l'original à partir de vos sauvegardes. Si ni vous ni votre hébergeur ne possédez de sauvegarde, il se peut que vous deviez recommencer de zéro la construction de votre site internet&nbsp;! Remarquez aussi que si vos seules sauvegardes sont chez votre hébergeur, il est possible qu'un attaquant réussisse à les effacer en prenant le contrôle de votre site.&nbsp;
- .Étape 7&nbsp;: Passez à un service d'atténuation d'attaque DDoS ou à un fournisseur d'hébergement sécurisé. Deflect.ca peut vous aider en protégeant votre site d'attaques en ligne. CloudFlare peut également bloquer de nombreuses attaques répandues. Les fournisseurs d'hébergement sécurisé comme VirtualRoad/Qurium investissent beaucoup d'efforts dans la détection et la prévention de telles attaques.&nbsp;

Ne vous arrêtez pas là&nbsp;! Importantes mesures supplémentaires

_N'attendez pas de subir une attaque&nbsp;!_ Tous les services indiqués ci-dessous vous aideront rapidement pendant ou après une attaque mais vous pouvez vous protéger vous-même dès maintenant, avant qu'elle ne se produise&nbsp;! Ceci peut réduire le coût d'une attaque en diminuant votre usage de bande passante et en vous maintenant en ligne pendant la crise. Une fois que vous avez été attaqué, cela peut prendre jusqu'à trois jours pour qu'Internet vous «&nbsp;retrouve&nbsp;» à votre nouvelle adresse protégée. Il est donc dans presque tous les cas bien mieux d'_être préparé et de commencer tout de suite_.

1. Les fournisseurs d'hébergement sécurisé exigent que vous déplaciez complètement votre site sur leurs serveurs&nbsp;: vous changez d'hébergeur. Beaucoup d'entre eux peuvent vous y aider. Ce choix a pour avantage, entre autres, que la solution d'hébergement fournit souvent d'autres fonctionnalités de protection en plus de l'atténuation d'attaque DDoS. L'inconvénient peut être le coût (selon ce que vous payez actuellement) et le contrôle&nbsp;: vous devez pouvoir faire confiance à l'hébergeur de votre domaine car il dispose d'un pouvoir important sur votre site.&nbsp;
  - .Avantages&nbsp;:&nbsp;
    - .Fournit un service unique centralisé pour la plupart, voire la totalité, des besoins de votre site&nbsp;
    - .Fournit des services de protection contre les attaques DDoS, le piratage et le spam&nbsp;
    - .Comprend souvent de nombreuses options supplémentaires et des services de conseil, parfois même une certaine protection juridique limitée&nbsp;
    - .Des équipes d'assistance complète sont souvent disponibles pour vous aider.&nbsp;

  - .Inconvénients&nbsp;:&nbsp;
    - .Vous devez héberger votre site internet chez cette société.&nbsp;
    - .Vous devez faire confiance au service pour la gestion de votre site et la défense de vos droits.&nbsp;
    - .Ces services sont souvent beaucoup plus chers (mais vous n'avez plus besoin de payer d'autres services d'hébergement/de DNS&nbsp;!).&nbsp;

2. Les services d'atténuation d'attaque DDoS vous permettent de continuer à héberger votre site là où il est et ne font que changer la façon dont les autres utilisateurs d'Internet le trouvent et y accèdent&nbsp;: c'est souvent beaucoup plus facile à mettre en place. Ces services disposent de serveurs partout dans le monde qui, essentiellement, s'interposent devant votre site internet et absorbent ou ignorent le trafic malveillant. Ils font un «&nbsp;miroir&nbsp;» de votre site et diffusent des copies constamment mises à jour de votre site. Ces services sont faciles à mettre en place et vous conservez entièrement le contrôle de votre site et de la configuration d'hébergement. Les services proxy peuvent poser un problème pour les sites très complexes qui risquent de rencontrer des difficultés avec les connexions d'utilisateurs non administrateurs et les zones interactives/javascript complexes. Discutez-en avec votre webmaster et le service de proxy car la plupart du temps, ceci peut être résolu.&nbsp;
  - .Avantages&nbsp;:&nbsp;
    - .Coût moindre (souvent avec une offre gratuite)&nbsp;
    - .Rapide et facile à mettre en place&nbsp;
    - .Vous n'avez pas à changer d'hébergeur.&nbsp;
    - .Vous pouvez modifier ou quitter le service à tout moment.&nbsp;

  - .Inconvénients&nbsp;:&nbsp;
    - .Moins d'assistance&nbsp;
    - .Orienté surtout sur l'atténuation d'attaques DDoS&nbsp;: ne comprend pas nécessairement d'assistance contre le malware ou les spammeurs.&nbsp;
    - .Le trafic SSL (crypté) sera brièvement décrypté et ré-encrypté par le serveur proxy pour le transfert du proxy à votre serveur.&nbsp;

3. Choisissez un fournisseur spécifique&nbsp;: pour n'importe quel service, vous devez être à l'aise avec le fournisseur. C'est une question de confiance mais aussi de compréhension de son business model&nbsp;: s'agit-il d'une facturation à l'acte&nbsp;? S'il existe une version gratuite, reçoit-elle moins d'assistance qu'une version payante&nbsp;? Le service est-il financé par des gouvernements&nbsp;? Il vaut mieux obtenir le maximum de détails dès le début pour éviter des surprises plus tard.&nbsp;

Pour tous les services, posez-vous les questions suivantes&nbsp;:

- .Comment l'entreprise/l'organisation est-elle structurée et alimentée&nbsp;? Quels types de vérifications ou de signalements doit-elle éventuellement faire&nbsp;?&nbsp;
- .Examinez dans quel(s) pays elle a une présence légale et où elle serait tenue de se conformer à des requêtes policières ou judiciaires.&nbsp;
- .Quelles données sont enregistrées et combien de temps sont-elles disponibles&nbsp;?&nbsp;
- .Existe-t-il des restrictions concernant le type de contenu pour lequel le prestataire accepte d'être hébergeur/proxy et ces restrictions peuvent-elles avoir un impact pour votre site&nbsp;?&nbsp;
- .Existe-t-il des restrictions sur les pays dans lesquels le prestataire peut fournir le service&nbsp;?&nbsp;
- .Accepte-t-il un mode de paiement que vous pouvez utiliser&nbsp;? Pouvez-vous vous le permettre financièrement&nbsp;?&nbsp;
- .Communications sécurisées&nbsp;: vous devez pouvoir vous connecter de façon sécurisée et communiquer avec le prestataire de façon confidentielle.&nbsp;
- .L'option d'authentification à deux facteurs est-elle proposée, pour améliorer la sécurité des accès administrateur&nbsp;? Cette politique d'accès sécurisé ou d'autres similaires peut contribuer à réduire la menace d'autres formes d'attaques contre votre site internet.&nbsp;
- .À quel type d'assistance aurez-vous accès dans la durée&nbsp;? L'assistance entraîne-t-elle des frais supplémentaires et/ou recevrez-vous une assistance suffisante si vous utilisez le niveau «&nbsp;gratuit&nbsp;»&nbsp;?&nbsp;
- .Pouvez-vous faire une simulation de votre site avant le déménagement grâce à un site de qualification&nbsp;?&nbsp;

Questions pour les services d'hébergement sécurisé

- .Offrent-ils une assistance complète pour déménager votre site&nbsp;?&nbsp;
- .Les services sont-ils équivalents ou meilleurs que ceux de votre hébergeur actuel, au moins pour les outils ou services que vous utilisez&nbsp;? À vérifier en priorité&nbsp;:&nbsp;
  - .Les tableaux de bord de gestion comme cPanel&nbsp;
  - .Les comptes e-mail (combien, quotas, accès SMTP, IMAP)&nbsp;
  - .Les bases de données (combien, types, accès)&nbsp;
  - .Accès à distance par SFTP/SSH&nbsp;
  - .Assistance pour le langage de programmation (PHP, Perl, Ruby, accès cgi-bin...) ou CMS (Drupal, Joomla, Wordpress…) que votre site utilise.&nbsp;

Questions pour les services d'atténuation d'attaque DDoS&nbsp;:

- .Si vous utilisez SSL (également appelé HTTPS ou trafic web sécurisé), demandez comment ils gèrent SSL. Dans certaines configurations, il peut être plus simple de partager votre clé SSL privée. Si vous optez pour cette solution, vous devez avoir un très haut degré de confiance dans le prestataire de services car il peut «&nbsp;se faire passer pour&nbsp;» votre site (de fait, c'est ce que vous lui demandez de faire quand il vous fournit un proxy&nbsp;!)&nbsp;
- .Demandez comment les connexions et pages d'administration/de rédaction sont gérées.&nbsp;
- .Discutez de toutes les parties interactives de votre site (utilisateurs qui se connectent, commentaires, besoins des administrateurs/rédacteurs, pages interactives complexes/javascript/animations)&nbsp;: les différents services proxy gèrent ces aspects différemment. Vous aurez besoin de tester ces points avant le déménagement final.&nbsp;

Services spécifiques de réduction et d'atténuation

Les services spécifiques sont listés sur [https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-services](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-services) avec des commentaires développés. Veuillez noter que la liste de services fournie n'est pas exhaustive, il en existe beaucoup d'autres. Néanmoins, ces services représentent tous de bons points de départ, dans la mesure où ils ont été utilisés par d'autres membres des communautés des médias indépendants et de la défense des droits de l'homme et de la liberté d'expression. Pour une réponse immédiate, voici des options possibles&nbsp;:

- .Services d'hébergement sécurisé&nbsp;:&nbsp;
  - .Qurium (anciennement Virtual Road)&nbsp;
  - .The Positive Internet Company&nbsp;
  - .Greenhost&nbsp;

- .Services d'atténuation d'attaques DDoS&nbsp;:&nbsp;
  - .Deflect.ca&nbsp;
  - .Projet Shield de Google&nbsp;
  - .Projet Galileo de CloudFlare&nbsp;

Prenez des précautions supplémentaires contre les attaques

Même si vous n'avez pas connu d'attaque par déni de service, ce guide vous propose des mesures pour vous y préparer, dans l'espoir d'éviter toute indisponibilité du site. Reportez-vous directement à la section [Répondre à une attaque par déni de service](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#responding-to-a-denial-of-service-attack) pour inventorier les solutions répandues que vous pouvez mettre en œuvre tout de suite, avant d'être attaqué. Dans la section Ressources utiles, vous trouverez des guides permettant de maintenir votre site en vie.

- .Sauvegardes&nbsp;: Il est toujours bon de vous assurer que vous avez des sauvegardes (que vous stockez ailleurs que votre site internet&nbsp;!). De nombreux hébergeurs et plateformes de sites internet l'intègrent à leur service mais il est mieux de posséder aussi des sauvegardes supplémentaires, hors ligne.&nbsp;
- .Restez à jour&nbsp;: Si vous utilisez un système de gestion de contenu (CMS) comme WordPress ou Drupal, vérifiez que la technologie utilisée par votre site internet est à jour sur les dernières versions, particulièrement s'il y a eu des mises à jour de sécurité. Si vous utilisez un programme personnalisé, envisagez de passer à un CMS qui fait l'objet de mises à jour régulières.&nbsp;
- .Surveillance&nbsp;: Il existe de nombreux services qui peuvent vérifier en permanence votre site et vous envoyer un e-mail ou un SMS s'il est indisponible. Cet article de Mashabledonne les références de dix services appréciés. Soyez conscient que l'adresse électronique ou le numéro de téléphone que vous utilisez pour cette surveillance sera clairement associé à la gestion du site.&nbsp;

Menez l'enquête

Si vous avez été victime d'un _déni de service_ ou d'un _défacement_, il peut être précieux de comprendre pourquoi vous avez été attaqué et pourquoi maintenant.

**Pourquoi vous avez été attaqué et pourquoi maintenant** &nbsp;: Qui, d'après vous, pourrait trouver intérêt à s'attaquer à votre site internet ou à l'organisation dont vous faites partie&nbsp;? Avez-vous récemment publié un contenu controversé, cette menace pourrait-elle être liée à votre travail ou votre site internet reçoit-il beaucoup de visites et votre nom de domaine a expiré&nbsp;? Pourquoi maintenant&nbsp;? Est-ce qu'un changement récent dans votre site internet pourrait avoir fait de vous une cible pour des attaques par déni de service ou des défacements&nbsp;? La section Ressources utiles contient des liens vers des guides livrant des conseils et des trucs sur la prévention des urgences numériques et la proactivité en matière de sécurité informatique.

Ressources utiles&nbsp;:

- .Mon site est indisponible&nbsp;: https://github.com/OpenInternet/MyWebsiteIsDown&nbsp;
- .Maintenez votre site en vie&nbsp;: https://www.eff.org/keeping-your-site-alive&nbsp;
- .Security in a Box&nbsp;: https://securityinabox.org/en/chapter\_7\_2&nbsp;
- .Modélisation de menace, guide d'autodéfense contre la surveillance&nbsp;: https://ssd.eff.org/risk/threats&nbsp;

À propos du Kit de premiers secours numériques

Le Kit de premiers secours numériques est le produit d'une collaboration entre EFF, Global Voices, Hivos & the Digital Defenders Partnership, Front Line Defenders, Internews, Freedom House, Access, Qurium, CIRCL, IWPR, Open Technology Fund et des experts individuels en sécurité qui travaillent dans le domaine de la sécurité numérique et de l'intervention rapide. C'est un travail en cours d'élaboration et si des points doivent être ajoutés ou pour toute question ou commentaire concernant une des sections de ce document, rendez-vous sur [Github](https://github.com/RaReNet/DFAK).

Ce document est diffusé sous [licence Creative Commons Attribution – Partage dans les mêmes conditions 4.0 International](http://creativecommons.org/licenses/by-sa/4.0/).
