# Avis sur la certification CWES

Salut, comment ça va ? Je suis huupwn — c'est mon pseudo de hacker, mais mon vrai nom est Hữu. Je suis encore au lycée, et le CWES est en fait la toute première certification que j'ai obtenue.

L'année prochaine, mon objectif est de participer à un CTF, et j'ai décidé que la meilleure façon de m'y préparer était d'étudier et de passer la certification **CWES (Web Exploitation Specialist)** de Hack The Box (HTB). C'est un certificat relativement récent qui gagne en popularité, et qu'on compare souvent à l'eWPTX ou au BSCP. Voici l'intégralité de mon expérience : le cours, l'examen, le rapport.

## Introduction

Je suis arrivé dans la sécurité informatique presque par hasard — en jouant avec les modules gratuits de HTB Academy par curiosité, puis en me laissant happer par ce petit moment de révélation quand on trouve un exploit qui fonctionne. Je n'ai aucune certification antérieure, aucune expérience professionnelle, ni aucun réseau dans le domaine. Ce que j'ai, en revanche, c'est beaucoup de temps libre en tant qu'élève, et un véritable intérêt pour l'exploitation web.

J'aime les certifications parce qu'elles constituent une preuve tangible de compétences — un moyen de me prouver à moi-même (et éventuellement aux autres) que mes compétences sont réelles, même sans CV rempli d'expérience professionnelle.

Après quelques recherches, j'ai réduit mon choix à deux options : le **Certified Web Exploitation Specialist (CWES)** de HTB et le **Burp Suite Certified Practitioner (BSCP)** de PortSwigger. J'avais déjà testé quelques modules gratuits de HTB Academy pour le plaisir et j'avais aimé leur pédagogie, donc le CWES semblait être la suite logique — et une bonne étape vers le CTF de l'année prochaine.

Pour obtenir la certification, il faut :

1. Terminer tout le contenu de formation du parcours **Web Penetration Tester**.
2. Réussir l'examen avec un score minimum de 80/100.
3. Soumettre un rapport professionnel.

## Le cours de préparation

Il faut avoir terminé 100 % du contenu du cours et réussi l'évaluation de compétences à la fin de chaque module avant même que l'examen ne se débloque.

Le parcours compte environ 20 modules, allant d'un niveau facile à moyen. Tout est présenté sous forme de texte — pas de vidéos, pas de diapositives. Je suis resté bloqué sur plusieurs tâches, mais les indices de la communauté (en ligne et sur le Discord de HTB) m'ont sauvé plus d'une fois.

Rien à redire sur le contenu en lui-même — il est clair, concis et va droit au but. On sent que certains modules ont été rédigés par des personnes ayant une réelle expérience du pentest ; elles glissent parfois des anecdotes tirées du terrain, ce qui est un plus appréciable.

La liste complète des modules se trouve sur le site de HTB Academy, dans le parcours Web Penetration Tester.

### Le point faible de la préparation

Le plus grand manque, c'est la *pratique*. Certes, chaque module se termine par des exercices, mais on sait déjà exactement quelle classe de vulnérabilité on cherche — ce qui rend les choses bien plus faciles qu'elles ne le seraient en réalité.

Le véritable examen vous remet une application et rien d'autre ; c'est à vous de déterminer ce qu'il faut tester. Un grand laboratoire intégré combinant plusieurs applications — quelque chose qui simule réellement les conditions de l'examen — serait très utile. Une liste séparée de machines d'entraînement supplémentaires ne ferait pas de mal non plus. Globalement, j'ai eu l'impression que le cours ne prépare pas suffisamment sur le plan pratique.

## L'examen

Un gros avantage : aucune planification requise. Il suffit de se connecter et de démarrer dès qu'on est prêt. On dispose de **7 jours au total**, couvrant à la fois l'accès au laboratoire et la rédaction du rapport — aucun temps supplémentaire n'est accordé pour le rapport, donc il faut s'organiser en conséquence.

Vous devrez affronter plusieurs applications, chacune nécessitant un user flag et un root flag. Cela implique généralement l'exploitation d'une vulnérabilité, ou l'enchaînement de deux. Il y a souvent une astuce supplémentaire à découvrir par soi-même, même si certains flags étaient assez simples — comparables aux évaluations de compétences.

Honnêtement, certaines parties de l'examen étaient *bien* plus difficiles que tout ce qu'on trouve dans les modules — quelques défis m'ont poussé bien au-delà de ce que les évaluations de compétences avaient préparé. D'autres flags se rapprochaient davantage de la difficulté des modules, mais je ne dirais pas que l'examen est homogène de bout en bout ; attendez-vous à de vrais pics de difficulté. J'avais tous les flags dès le jour 4 et j'ai passé le reste du temps sur le rapport.

### Le point faible de l'examen

Sept jours, c'est long. J'ai fini par programmer le mien pendant les vacances d'été pour éviter de poser des congés au travail — pas exactement une manière reposante de passer ces vacances, et plutôt épuisant mentalement pendant que tout le monde se détend autour de soi. Je pense que la durée (et peut-être aussi le nombre de tâches) pourrait être réduite.

Il faut aussi être honnête : sans expérience sur des machines en dehors des modules officiels, l'examen est vraiment difficile. La théorie du cours seule ne suffit pas tout à fait.

### Le point fort de l'examen

L'environnement en lui-même était très solide — aucun lag, aucun crash, ce qui compte énormément sur une semaine d'examen. J'ai aussi vraiment apprécié la conception de plusieurs défis.

## Le cours suffit-il pour réussir ?

Réponse courte : en partie. Les techniques d'exploitation sont bien enseignées, mais comme mentionné, l'examen repose sur des « astuces » qui ne sont pas explicitement couvertes dans les modules. Attendez-vous à devoir en découvrir certaines par vous-même — ce qui, honnêtement, constitue un bon entraînement pour un environnement de CTF, où l'on n'a que rarement la main tenue.

## Rédiger le rapport

Capturer les flags ne suffit pas en soi — un rapport professionnel est obligatoire, et certaines personnes échouent pour en avoir rendu un trop faible. Ce n'est pas un simple walkthrough ; il faut une analyse complète pour chaque vulnérabilité : impact, notation CWE/CVSS, mesures d'atténuation, et une reproduction étape par étape. HTB fournit un modèle qui précise exactement ce qu'ils attendent.

J'ai utilisé **Sysreptor** pour rédiger le mien, et cela a grandement facilité le processus. L'outil met automatiquement en forme selon le style maison de HTB, génère une table des matières, et propose une section pré-structurée pour chaque découverte. Vous trouvez une injection SQL ? Cliquez sur « add new finding », choisissez SQLi dans la liste, et il génère un chapitre avec une description et des mesures d'atténuation pré-remplies — il ne reste plus qu'à ajouter vos propres étapes.

**Astuce :** la version cloud de Sysreptor est payante, mais vous pouvez l'auto-héberger gratuitement sur votre propre VM et y accéder via un panneau web depuis Kali ou votre machine hôte. Je recommande vivement de mettre cela en place *avant* le début de l'examen. Chez moi, ça refusait de tourner sur ma machine Kali, j'ai donc dû monter une Ubuntu à la place — environ 90 minutes que je n'avais pas envie de perdre en plein examen.

Rédiger le rapport m'a pris 5 à 6 heures. J'ai dormi dessus et tout relu le lendemain matin avec un regard neuf. Le délai de correction annoncé par HTB (SLA) est jusqu'à 20 jours ouvrés.

## Coût

Début 2026, il existe deux façons principales de payer :

- **Abonnement Silver Annual — 490 $.** Accès complet au parcours Web Penetration Tester plus un voucher d'examen. L'option la plus simple, à mettre en place une fois pour toutes.
- **Cubes (la monnaie interne de HTB).** Le parcours complet Web Penetration Tester coûte 1 410 cubes (environ 150 $ à ~100 $ les 1 000 cubes), plus un voucher d'examen séparé à 210 $ — soit environ **360 $ au total**. Plus économique si le CWES est votre seul objectif sur la plateforme.

Consultez la page de facturation de HTB pour connaître les tarifs actuels.

## Mes conseils

1. **Prenez des notes détaillées.** Non négociable. Les modules dissimulent souvent des petits détails ou extraits de code qui deviennent des indices directs pendant l'examen — documentez tout pour pouvoir le retrouver facilement plus tard.
2. **Refaites les évaluations de compétences avant l'examen.** Revenez sur les exercices finaux de chaque module et relisez rapidement le contenu pédagogique pour pouvoir vous y retrouver rapidement sous pression. Vous *devrez* absolument revenir consulter le contenu du cours pendant l'examen pour trouver des pistes.
3. **Entraînez-vous en dehors du cours.** Les modules seuls ne suffisent pas — le temps passé sur les machines de la plateforme principale de HTB est inestimable. Je n'ai pas moi-même terminé le parcours Bug Bounty Hunter, mais il semble offrir un excellent entraînement à l'exploitation manuelle, et l'exploitation manuelle est exactement la compétence qu'un CTF va tester.
4. **Soyez sélectif quant aux ressources complémentaires.** J'ai suivi une partie du parcours CPTS d'IppSec, et même si c'était de bonne qualité, ce n'était pas très pertinent ici. Cherchez des machines qui exigent une exploitation web manuelle, et non des exploits publics pour des logiciels obsolètes — c'est exactement l'ensemble de compétences que récompensent à la fois le CWES et le CTF de l'année prochaine.

***Note sur l'utilisation de l'IA :*** *J'ai écrit cet article moi-même. J'ai utilisé Claude (Anthropic) pour peaufiner significativement la grammaire, le choix des mots et la structure des phrases ; le contenu technique et toutes les affirmations sont miens.*

***Note :*** *Si vous souhaitez consulter une partie de mon write-up CWES, contactez-moi [ici](https://www.facebook.com/profile.php?id=61553341873402)*

*Date : 19-09-26*
