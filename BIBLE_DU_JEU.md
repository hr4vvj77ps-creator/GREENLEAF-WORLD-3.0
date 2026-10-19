GREENLEAF WORLD — BIBLE DU JEU
Version 1.0 — Document central de conception Projet : GreenLeaf World 3.1 Statut : document évolutif de référence pour le créateur et les IA de développement
 
⸻
 
1. OBJECTIF DE CETTE BIBLE
Cette Bible rassemble les idées, les règles de conception, les univers, les personnages, les quêtes, les missions, les récompenses et les systèmes que GreenLeaf World doit développer progressivement.
Elle sert à :
	•	conserver les idées du projet dans un document durable ;
	•	éviter que les futures IA oublient les décisions précédentes ;
	•	empêcher la création de fonctionnalités contradictoires ;
	•	faciliter l’ajout de nouvelles histoires, quêtes, personnages et mécanismes ;
	•	permettre à une IA de comprendre le projet avant de toucher au code ;
	•	distinguer les fonctions réellement développées des concepts encore à créer.
Règle fondamentale
Une idée documentée n’est pas nécessairement une fonction développée.
Chaque fonctionnalité doit être identifiée comme :
	•	Validée en conception : la règle a été décidée.
	•	À concevoir : le principe existe, mais ses détails restent à définir.
	•	À développer : la fonctionnalité n’est pas encore implémentée.
	•	En cours : le développement a commencé.
	•	À tester : le code existe, mais son fonctionnement n’est pas suffisamment vérifié.
	•	Validée techniquement : les tests prévus ont réussi et les résultats sont documentés.
Une IA ne doit jamais annoncer qu’une fonction est opérationnelle uniquement parce qu’elle a écrit du code ou créé une maquette.
 
⸻
 
PARTIE I — VISION DU MONDE
2. LE CONCEPT GREENLEAF WORLD
GreenLeaf World associe trois dimensions complémentaires.
2.1 Le monde réel
Une carte réelle permet de découvrir :
	•	producteurs locaux ;
	•	artisans et ateliers ;
	•	créateurs ;
	•	collectionneurs ;
	•	commerces et entreprises ;
	•	lieux de découverte ;
	•	partenaires commerciaux ;
	•	activités et événements autorisés.
Les participants peuvent présenter leur savoir-faire, leur histoire, leurs produits et leurs activités.
La présence sur la carte doit respecter la vie privée et les autorisations des personnes concernées.
2.2 Le monde fantastique
Les joueurs explorent un univers imaginaire composé de royaumes, de régions, de cités, de donjons, de lieux secrets et de civilisations.
Ils peuvent faire progresser leurs personnages, accomplir des missions, collecter des ressources virtuelles, fabriquer des objets, découvrir des trésors et construire des espaces persistants.
2.3 Le lien entre les deux mondes
Principe central :
« Le monde réel nourrit le monde virtuel. »
Des activités réelles autorisées peuvent débloquer des missions particulières, des découvertes ou des récompenses virtuelles. Mais le jeu doit également offrir une progression complète aux joueurs qui ne réalisent aucun achat.
Les actions réelles ne doivent être prises en compte que lorsque leur validation est possible et que le joueur a donné son consentement.
3. LES PRINCIPES NON NÉGOCIABLES
	1.	Le jeu doit pouvoir se développer progressivement, d’un petit monde vers une grande civilisation persistante.
	2.	Les constructions, personnages, ressources et progressions importantes doivent être sauvegardés durablement.
	3.	Le monde ne doit pas être réinitialisé automatiquement à chaque saison.
	4.	Les joueurs peuvent progresser sans dépenser d’argent réel.
	5.	Les récompenses rares ne doivent pas être exclusivement réservées aux joueurs payants.
	6.	Les achats ne doivent pas donner automatiquement de l’expérience simplement parce qu’une somme a été dépensée.
	7.	Les joueurs peuvent explorer, construire, collectionner, fabriquer et coopérer.
	8.	Les systèmes de jeu doivent être cohérents entre les personnages, les quêtes, les niveaux et les royaumes.
	9.	Les ressources virtuelles doivent être distinctes de l’argent réel.
	10.	Les activités commerciales doivent être transparentes et respecter les règles applicables.
	11.	Les fonctions sensibles doivent être sécurisées côté serveur.
	12.	Les idées nouvelles doivent enrichir le projet sans supprimer les fonctions existantes.
 
⸻
 
PARTIE II — LES DEUX UNIVERS
4. LE MONDE CLASSIQUE
Le Monde classique constitue l’univers fantastique principal.
Il comprend notamment :
	•	une carte d’exploration ;
	•	des personnages jouables ;
	•	des refuges ;
	•	des avant-postes ;
	•	des villes ;
	•	des royaumes ;
	•	des guildes et alliances ;
	•	des tavernes ;
	•	des quêtes et missions ;
	•	des compagnons ;
	•	des montures ;
	•	de la collecte ;
	•	de l’artisanat ;
	•	des fragments de cartes ;
	•	des coffres et artefacts ;
	•	des constructions persistantes.
Les joueurs doivent pouvoir suivre plusieurs voies de progression. Un joueur peut se concentrer sur l’exploration, un autre sur l’artisanat, un autre sur la construction ou la coopération.
Aucune voie ne doit être indispensable à tous les styles de jeu.
5. LE MONDE DE LA NUIT
Le Monde de la Nuit constitue un univers distinct, soumis à une autorisation d’accès.
Ses données sont séparées de celles du Monde classique :
	•	personnage ;
	•	carte ;
	•	inventaire ;
	•	points ;
	•	catalogue ;
	•	panier ;
	•	commandes ;
	•	historique ;
	•	progression spécifique ;
	•	autorisations.
Un compte non autorisé ne doit pas pouvoir découvrir les espaces privés depuis la carte classique ni accéder aux données protégées.
Les contrôles doivent être appliqués côté serveur, notamment par les permissions et les politiques Supabase RLS adaptées.
La révocation d’un accès bloque les accès futurs concernés sans supprimer automatiquement l’historique nécessaire.
Le prototype local ne constitue pas une sécurité réelle.
 
⸻
 
PARTIE III — ROYAUMES ET EXPLORATION
6. LES ROYAUMES ENVISAGÉS
Les royaumes suivants sont prévus comme pistes de conception. Leur carte complète, leur histoire et leurs conditions d’accès restent à développer.
6.1 La forêt ancienne
Un territoire de forêts profondes, de ruines recouvertes par la végétation, de créatures anciennes et de passages oubliés.
Idées de contenu :
	•	sentiers cachés ;
	•	arbres remarquables ;
	•	clairières ;
	•	ruines ;
	•	ressources naturelles virtuelles ;
	•	quêtes de découverte ;
	•	créatures gardiennes ;
	•	fragments de cartes.
6.2 Les terres enchantées
Un territoire de magie, de mystères, d’illusions et de phénomènes extraordinaires.
Idées :
	•	énigmes ;
	•	objets enchantés ;
	•	portes secrètes ;
	•	ateliers magiques ;
	•	missions de collecte ;
	•	personnages possédant des connaissances particulières.
6.3 Les Sept Mers
Un univers d’exploration maritime.
Idées :
	•	ports ;
	•	îles ;
	•	navires ;
	•	routes maritimes ;
	•	épaves fictives ;
	•	trésors ;
	•	cartes nautiques ;
	•	missions de navigation ;
	•	échanges entre communautés.
6.4 Le Royaume du Ciel
Un territoire aérien composé d’îles flottantes, de citadelles suspendues et de routes célestes.
Idées :
	•	ponts aériens ;
	•	montures volantes éventuelles ;
	•	tours d’observation ;
	•	missions de traversée ;
	•	fragments de cartes du ciel.
6.5 Les royaumes oubliés
Des territoires anciens dont l’histoire a disparu.
Idées :
	•	archives ;
	•	ruines ;
	•	inscriptions ;
	•	lignées anciennes ;
	•	reliques ;
	•	quêtes narratives à plusieurs étapes.
6.6 Les grottes de cristal
Un réseau souterrain avec des ressources virtuelles, des passages cachés et des phénomènes lumineux.
Idées :
	•	exploration souterraine ;
	•	collecte de cristaux virtuels ;
	•	outils d’extraction ;
	•	zones dangereuses ;
	•	énigmes ;
	•	ateliers spécialisés.
6.7 La cité engloutie
Une ancienne cité perdue sous les eaux.
Idées :
	•	quartiers submergés ;
	•	archives ;
	•	objets anciens ;
	•	chemins immergés ;
	•	histoires de l’ancienne civilisation.
6.8 Le Royaume lunaire secret
Un royaume caché, associé à des conditions d’accès particulières.
L’accès existant envisagé dans le projet comprend :
	•	l’appel de la nuit ;
	•	le niveau 20 ;
	•	1 000 points ;
	•	une autorisation de compte.
Ces conditions doivent être vérifiées dans le code actuel avant toute modification. Elles ne doivent pas être contournables par un simple changement d’interface.
6.9 Le désert des dragons
Un territoire de dunes, de ruines, de créatures mythiques et de lieux difficiles à atteindre.
Idées :
	•	oasis ;
	•	ruines ensevelies ;
	•	cavernes ;
	•	trésors ;
	•	quêtes de préparation ;
	•	artefacts liés aux dragons.
6.10 Les marais des sorcières
Un territoire mystérieux comprenant des chemins mouvants, des ruines, des plantes fictives et des personnages énigmatiques.
Idées :
	•	missions de collecte ;
	•	énigmes ;
	•	chemins cachés ;
	•	potions virtuelles ;
	•	histoires à embranchements.
7. STRUCTURE D’UNE RÉGION
Chaque région devra disposer progressivement d’une fiche contenant :
	•	nom ;
	•	description ;
	•	ambiance ;
	•	histoire ;
	•	carte ;
	•	lieux importants ;
	•	personnages présents ;
	•	ennemis ou dangers éventuels ;
	•	ressources virtuelles ;
	•	missions disponibles ;
	•	quêtes associées ;
	•	niveaux recommandés ;
	•	conditions d’accès ;
	•	récompenses possibles ;
	•	liens avec les autres régions ;
	•	état du développement.
Une région ne doit pas être considérée comme terminée si elle n’existe que sous la forme d’une image ou d’une carte décorative.
 
⸻
 
PARTIE IV — PERSONNAGES
8. CATALOGUE DES PERSONNAGES
Le projet prévoit 100 emplacements de personnages :
	•	50 personnages classiques ;
	•	50 personnages du Monde de la Nuit.
Cette répartition doit être vérifiée dans le code actuel avant d’être modifiée. Les emplacements existants et les personnages déjà développés doivent être conservés.
Un emplacement vide ou un nom provisoire ne doit pas être présenté comme un personnage entièrement développé.
9. FICHE STANDARD D’UN PERSONNAGE
Chaque personnage doit avoir une fiche structurée.
Identité
	•	identifiant unique ;
	•	nom ;
	•	univers ;
	•	titre éventuel ;
	•	description ;
	•	histoire personnelle ;
	•	origine ;
	•	apparence ;
	•	personnalité.
Profil de jeu
	•	rôle ;
	•	spécialités ;
	•	forces ;
	•	faiblesses ;
	•	compétences ;
	•	style de progression ;
	•	interactions possibles ;
	•	liens avec les royaumes.
Progression
	•	niveau ;
	•	expérience ;
	•	caractéristiques ;
	•	compétences débloquées ;
	•	équipement ;
	•	inventaire associé ;
	•	titres obtenus ;
	•	historique de progression.
Relations
	•	compagnons possibles ;
	•	personnages liés ;
	•	guildes ou factions ;
	•	relations narratives ;
	•	missions personnelles ;
	•	quêtes associées.
Technique
	•	identifiant stable ;
	•	état de disponibilité ;
	•	règles d’accès ;
	•	données sauvegardées ;
	•	tests réalisés ;
	•	éléments encore à développer.
10. ÉVOLUTION DES PERSONNAGES
Le projet comporte déjà une progression envisagée allant jusqu’au niveau 50. La logique exacte des niveaux, de l’expérience et des caractéristiques doit être auditée avant toute modification.
Les personnages doivent pouvoir évoluer différemment selon les activités habituelles du joueur.
Exemples de spécialisations possibles :
	•	explorateur ;
	•	artisan ;
	•	bâtisseur ;
	•	collectionneur ;
	•	protecteur ;
	•	navigateur ;
	•	érudit ;
	•	diplomate ;
	•	aventurier ;
	•	spécialiste des ressources virtuelles.
Ces spécialisations sont des pistes, pas des classes définitives.
Les compétences doivent avoir des conditions d’obtention explicites et ne doivent pas rendre obligatoire un achat réel.
11. PERSONNAGES CLASSIQUES ET PERSONNAGES DU MONDE DE LA NUIT
Les deux groupes peuvent avoir des histoires, apparences, équipements et quêtes distincts.
La conception doit préciser :
	•	les différences d’univers ;
	•	les compétences propres à chaque groupe ;
	•	les restrictions d’accès ;
	•	les éléments partagés autorisés ;
	•	les données qui doivent rester séparées.
Les personnages déjà existants ne doivent pas être renommés, remplacés ou réinitialisés sans vérification et accord explicite.
 
⸻
 
PARTIE V — QUÊTES ET HISTOIRES
12. OBJECTIF DU SYSTÈME DE QUÊTES
Les quêtes donnent une direction au joueur et relient les personnages, les royaumes, l’exploration, les missions et les récompenses.
Elles doivent offrir :
	•	une raison d’explorer ;
	•	une histoire à découvrir ;
	•	des objectifs compréhensibles ;
	•	des choix lorsque cela est prévu ;
	•	une progression mesurable ;
	•	des récompenses cohérentes ;
	•	des liens entre les régions.
13. TYPES DE QUÊTES
Quêtes principales
Elles racontent l’histoire générale du monde et peuvent ouvrir progressivement de nouveaux territoires.
Quêtes secondaires
Elles développent les histoires locales, les personnages et les lieux.
Quêtes personnelles
Elles concernent l’histoire ou l’évolution d’un personnage.
Quêtes d’exploration
Elles encouragent la découverte de lieux, de passages et de points remarquables.
Quêtes de collecte
Elles demandent de réunir des ressources virtuelles ou des objets définis.
Quêtes d’artisanat
Elles demandent de fabriquer, réparer ou améliorer des objets virtuels.
Quêtes communautaires
Elles récompensent la coopération, les échanges et les objectifs collectifs.
Quêtes de guilde
Elles contribuent à la progression d’un groupe, d’un refuge ou d’une construction commune.
Quêtes secrètes
Elles peuvent être découvertes par une exploration, une combinaison d’indices ou une condition particulière.
Quêtes légendaires
Elles représentent des objectifs importants et difficiles, composés de plusieurs étapes.
Une quête légendaire achevée doit attribuer au minimum un artefact légendaire.
Quêtes liées au monde réel
Elles peuvent inclure une visite volontaire, une découverte locale, une participation à un événement ou une action partenaire explicitement décrite.
Elles doivent proposer une méthode de validation adaptée et ne doivent pas imposer d’achat pour accéder à la progression générale.
14. FICHE STANDARD D’UNE QUÊTE
Chaque quête doit contenir :
	1.	Identifiant unique.
	2.	Titre.
	3.	Description.
	4.	Histoire et contexte.
	5.	Univers et région.
	6.	Personnage ou événement déclencheur.
	7.	Niveau conseillé ou requis.
	8.	Conditions d’accès.
	9.	Liste des missions.
	10.	Ordre des objectifs.
	11.	Conditions de validation.
	12.	Objectifs facultatifs éventuels.
	13.	Choix narratifs éventuels.
	14.	Récompenses.
	15.	Conditions d’échec ou d’interruption.
	16.	Conditions de reprise.
	17.	Règles contre les validations répétées.
	18.	Effets sur la progression du monde.
	19.	Tests nécessaires.
	20.	Statut de développement.
Les récompenses ne doivent pas être inventées par l’IA au moment de coder si elles contredisent les règles déjà définies.
15. EXEMPLE DE QUÊTE LÉGENDAIRE
Titre provisoire : Les Fragments du Premier Royaume
Concept narratif à développer :
Un ancien royaume a disparu de la mémoire du monde. Des fragments de cartes et des récits contradictoires permettent d’en retrouver progressivement les traces.
Étapes possibles :
	1.	Découvrir une inscription ancienne.
	2.	Interroger un personnage qui connaît une partie de l’histoire.
	3.	Explorer plusieurs régions.
	4.	Réunir des fragments de carte.
	5.	Résoudre une énigme.
	6.	Débloquer un lieu caché.
	7.	Accomplir une dernière mission.
	8.	Découvrir le trésor final.
Récompense obligatoire à la conception : au moins un artefact légendaire.
Le nombre exact de fragments, les régions concernées, les missions et les effets de l’artefact restent à définir. Cet exemple n’est pas une quête déjà implémentée.
16. CONTINUER À CRÉER DES QUÊTES
Les futures IA pourront proposer de nouvelles quêtes à condition de :
	•	consulter les quêtes déjà enregistrées ;
	•	éviter les doublons ;
	•	respecter les niveaux et conditions d’accès ;
	•	réutiliser les personnages et lieux pertinents ;
	•	donner à chaque mission un objectif mesurable ;
	•	prévoir des récompenses équilibrées ;
	•	préciser les dépendances techniques ;
	•	signaler les idées qui nécessitent une décision du créateur.
Chaque nouvelle quête validée doit être ajoutée à cette Bible ou à un catalogue de quêtes relié à celle-ci.
 
⸻
 
PARTIE VI — MISSIONS ET OBJECTIFS
17. DIFFÉRENCE ENTRE QUÊTE ET MISSION
Une quête est un ensemble narratif ou un objectif global.
Une mission est une tâche précise qui permet de progresser dans une quête ou d’accomplir une activité indépendante.
Une quête peut contenir plusieurs missions obligatoires et facultatives.
18. CATÉGORIES DE MISSIONS
Exploration
	•	découvrir une région ;
	•	atteindre un lieu ;
	•	ouvrir un passage ;
	•	trouver un point remarquable ;
	•	révéler une partie de carte.
Rencontre
	•	parler à un personnage ;
	•	découvrir son histoire ;
	•	obtenir un indice ;
	•	établir une relation narrative.
Collecte
	•	réunir une quantité définie de ressources virtuelles ;
	•	découvrir une ressource rare ;
	•	retrouver un objet perdu.
Artisanat
	•	fabriquer un objet ;
	•	améliorer un équipement ;
	•	réparer une construction ;
	•	contribuer à un atelier.
Trésors
	•	réunir des fragments ;
	•	résoudre une énigme ;
	•	trouver une clé ;
	•	ouvrir un coffre obtenu par progression.
Coopération
	•	aider un autre joueur ;
	•	contribuer à une construction collective ;
	•	accomplir un objectif de guilde ;
	•	participer à un événement commun.
Civilisation
	•	développer un refuge ;
	•	construire un avant-poste ;
	•	améliorer un bâtiment ;
	•	participer au développement d’une ville.
Monde réel
	•	découvrir un lieu autorisé ;
	•	participer à une activité ;
	•	visiter un producteur ou un artisan participant ;
	•	accomplir une mission partenaire clairement identifiée.
Missions quotidiennes ou récurrentes
Elles peuvent encourager une participation régulière, sans obliger le joueur à se connecter à des horaires déraisonnables ni à payer.
Leur fréquence, leurs limites et leurs récompenses restent à équilibrer.

19. FICHE STANDARD D’UNE MISSION
Chaque mission doit préciser :
	•	identifiant unique ;
	•	nom ;
	•	description ;
	•	catégorie ;
	•	univers ;
	•	quête associée ;
	•	objectif exact ;
	•	conditions de départ ;
	•	méthode de validation ;
	•	nombre de répétitions autorisées ;
	•	récompenses ;
	•	conditions d’échec ;
	•	possibilité de reprise ;
	•	contrôles anti-fraude ;
	•	données à sauvegarder ;
	•	état d’implémentation ;
	•	tests nécessaires.
Une mission ne doit pas être validée simplement parce qu’un bouton a été pressé.
 
⸻
 
PARTIE VII — EXPÉRIENCE, NIVEAUX ET RÉCOMPENSES
20. EXPÉRIENCE ET PROGRESSION
La progression doit récompenser les activités réellement accomplies.
Sources possibles :
	•	quêtes ;
	•	exploration ;
	•	artisanat ;
	•	collecte virtuelle ;
	•	découverte ;
	•	coopération ;
	•	missions ;
	•	construction ;
	•	participation à des objectifs communautaires.
Les valeurs exactes d’expérience et les seuils de niveau doivent être documentés dans un système central afin d’éviter que chaque mission applique ses propres règles contradictoires.
21. RÉCOMPENSES POSSIBLES
	•	expérience ;
	•	titres ;
	•	objets de collection ;
	•	équipements virtuels ;
	•	recettes d’artisanat ;
	•	ressources virtuelles ;
	•	fragments de cartes ;
	•	clés ;
	•	accès à des lieux ;
	•	plans de construction ;
	•	décorations ;
	•	compagnons ;
	•	montures ;
	•	artefacts ;
	•	capacités spéciales ;
	•	éléments narratifs ;
	•	contributions à la progression d’une guilde ou d’une ville.
La rareté, les conditions d’obtention et les effets de chaque récompense doivent être documentés.
22. RÈGLES D’ÉQUITÉ
	•	Aucun achat réel ne doit être nécessaire pour obtenir de l’expérience.
	•	Les joueurs qui ne dépensent rien doivent pouvoir progresser durablement.
	•	Les récompenses légendaires doivent pouvoir être obtenues par des accomplissements prévus dans le jeu.
	•	Les avantages commerciaux ne doivent pas rendre automatiquement un personnage supérieur.
	•	Les probabilités, conditions et limites doivent être explicites lorsqu’un système aléatoire est utilisé.
	•	Aucun hasard payant ne doit être requis pour jouer.
	•	Les points de jeu ne doivent pas être convertibles automatiquement en argent réel.
23. RÉCOMPENSES RÉELLES
Des partenaires pourraient financer des produits, services ou bons d’achat.
Ces récompenses ne peuvent être proposées que si :
	•	leur financement est confirmé ;
	•	les quantités et conditions sont connues ;
	•	leur attribution est contrôlée ;
	•	les règles juridiques et fiscales ont été examinées ;
	•	le joueur est informé des conditions ;
	•	les données personnelles sont protégées.
Une récompense virtuelle et un bon d’achat réel sont deux objets différents et doivent être gérés séparément.
 
⸻
 
PARTIE VIII — COMPAGNONS, MONTURES ET ARTISANAT
24. COMPAGNONS
Les compagnons sont une piste de conception à développer.
Chaque compagnon pourrait disposer de :
	•	nom ;
	•	histoire ;
	•	apparence ;
	•	origine ;
	•	personnalité ;
	•	méthode d’obtention ;
	•	interactions ;
	•	compétences éventuelles ;
	•	évolution ;
	•	limites d’utilisation.
Les compagnons ne doivent pas tous être de simples bonus statistiques. Certains peuvent apporter une aide narrative, de l’exploration ou des interactions.
Le nombre de compagnons, leurs pouvoirs et leurs règles restent à définir.
25. MONTURES
Les montures peuvent être des récompenses d’exploration ou de progression.
Les fiches futures devront préciser :
	•	apparence ;
	•	univers ;
	•	conditions d’obtention ;
	•	déplacements autorisés ;
	•	régions compatibles ;
	•	progression éventuelle ;
	•	règles de sauvegarde.
Les déplacements spéciaux ne doivent pas contourner les conditions d’accès aux régions.
26. ARTISANAT ET FABRICATION
L’artisanat doit permettre de transformer des ressources virtuelles en objets utiles ou décoratifs.
Idées à étudier :
	•	ateliers ;
	•	recettes ;
	•	outils ;
	•	matériaux ;
	•	amélioration d’équipement ;
	•	réparation ;
	•	mobilier ;
	•	éléments de construction ;
	•	objets de collection ;
	•	objets nécessaires à certaines quêtes.
Chaque recette devra indiquer ses ingrédients, sa méthode, ses conditions et son résultat.
Les ressources consommées et les objets créés doivent être enregistrés de façon cohérente pour empêcher les doublons ou la duplication frauduleuse.
 
⸻
 
PARTIE IX — CONSTRUCTIONS ET CIVILISATION PERSISTANTE
27. REFUGES ET AVANT-POSTES
Les joueurs pourront développer progressivement des espaces personnels ou collectifs.
Idées :
	•	refuge ;
	•	atelier ;
	•	ferme virtuelle ;
	•	verger ;
	•	bibliothèque ;
	•	échoppe ;
	•	tour ;
	•	avant-poste ;
	•	fortification ;
	•	bâtiment spécialisé.
Les ressources nécessaires, les niveaux et les conditions de construction restent à définir.
28. VILLES, GUILDES ET ROYAUMES
À plus long terme, le monde pourra accueillir :
	•	guildes ;
	•	alliances ;
	•	villes ;
	•	communautés ;
	•	domaines ;
	•	royaumes de joueurs ;
	•	projets de construction collective.
Les règles de propriété, de gouvernance, de coopération, de résolution des conflits et de modération devront être conçues avant leur implémentation.
29. PERSISTANCE DU MONDE
Le monde doit évoluer sans réinitialisation automatique de l’ensemble des constructions à chaque saison.
À terme, le serveur devra sauvegarder :
	•	les constructions ;
	•	leur propriétaire ou groupe propriétaire ;
	•	leur emplacement ;
	•	leur état ;
	•	leurs améliorations ;
	•	leurs ressources ;
	•	leurs autorisations ;
	•	leur historique utile.
Les sauvegardes et la récupération après incident doivent être prévues.
Une construction visible uniquement sur l’appareil du joueur ne constitue pas une construction persistante partagée.
 
⸻
 
PARTIE X — CARTE RÉELLE, PRODUCTEURS ET PARTENAIRES
30. PROFILS RÉELS
Les producteurs, artisans, créateurs, collectionneurs et partenaires pourront disposer d’un profil adapté à leur activité.
Le profil pourra présenter :
	•	nom ou nom professionnel ;
	•	description ;
	•	origine et savoir-faire ;
	•	catalogue ;
	•	formats ;
	•	prix ;
	•	disponibilité ;
	•	localisation autorisée ;
	•	modalités de contact ;
	•	informations de livraison ;
	•	conditions de vente.
Les informations commerciales doivent être vérifiées selon leur nature. Une donnée non confirmée doit rester signalée comme telle.
31. ESPACES VIRTUELS POUR LES ACTEURS RÉELS
Un producteur peut, par exemple, avoir :
	•	une ferme virtuelle ;
	•	un verger ;
	•	un atelier ;
	•	une fromagerie ;
	•	une échoppe ;
	•	un bâtiment représentant son savoir-faire.
Les entreprises partenaires pourraient disposer d’un secteur ou d’une infrastructure virtuelle si cela est prévu par un partenariat réel.
La présence virtuelle est un élément du jeu ; elle ne constitue pas automatiquement un revenu ni une garantie commerciale.
32. PARTENARIATS ET RÉMUNÉRATION
Des partenariats pourraient rémunérer GreenLeaf pour des clients acquis, contrats confirmés, campagnes ou autres actions convenues.
Les entreprises mentionnées comme exemples ne doivent pas être présentées comme des partenaires tant qu’aucun accord n’est confirmé.
Le modèle envisagé est une commission sur les ventes effectivement réalisées. Un taux de 2 % ou 3 % a été évoqué, mais il reste à décider.
Les conditions devront préciser :
	•	la base de calcul ;
	•	les frais ;
	•	les annulations ;
	•	les remboursements ;
	•	les obligations de chaque partie ;
	•	la preuve de réalisation ;
	•	la protection des données.
Les récompenses réelles financées par les partenaires ne doivent jamais être promises avant confirmation de leur financement.
 
⸻
 
PARTIE XI — MONÉTISATION ET ÉCONOMIE DU JEU
33. SÉPARATION ENTRE VIRTUEL ET RÉEL
Il faut distinguer :
	•	XP ;
	•	niveaux ;
	•	ressources virtuelles ;
	•	objets de jeu ;
	•	prix des produits réels ;
	•	commissions ;
	•	frais ;
	•	bons d’achat ;
	•	remboursements.
Aucune conversion automatique ne doit transformer les ressources virtuelles en argent bancaire.
34. MINAGE VIRTUEL
Le minage initial désigne la collecte ou l’extraction de ressources fictives dans le jeu.
Il ne faut pas prétendre que le téléphone du joueur génère des revenus réels significatifs par le minage de cryptomonnaies.
Tout système financier ou crypto envisagé pour le Monde de la Nuit doit être traité séparément, avec une validation juridique, technique et opérationnelle préalable.
 
⸻
 
PARTIE XII — RÈGLES TECHNIQUES POUR LES FUTURES IA
35. AVANT DE DÉVELOPPER
Toute IA qui travaille sur GreenLeaf World doit :
	1.	Lire cette Bible.
	2.	Lire le cahier des charges existant.
	3.	Consulter l’état des fonctions et le suivi du projet.
	4.	Inspecter les fichiers concernés.
	5.	Identifier les fonctions déjà présentes.
	6.	Déterminer les dépendances.
	7.	Expliquer les fichiers qu’elle prévoit de modifier.
	8.	Sauvegarder avant une modification risquée.
	9.	Ne pas remplacer un module fonctionnel sans justification et autorisation.
	10.	Respecter les décisions validées et signaler les contradictions.
36. PENDANT LE DÉVELOPPEMENT
	•	Ne pas réécrire tout le projet lorsqu’une modification ciblée suffit.
	•	Ne pas supprimer les personnages, quêtes, données ou fonctions existants sans autorisation.
	•	Ne pas inventer des prix, des stocks, des fournisseurs ou des partenariats.
	•	Ne pas intégrer de secrets dans le code public.
	•	Ne pas confondre interface, prototype et fonction connectée.
	•	Ne pas utiliser le code client comme seule protection des accès.
	•	Garder les données privées séparées selon les permissions prévues.
	•	Documenter les migrations et leurs effets.
	•	Préserver les identifiants stables des personnages, quêtes, missions et objets.
37. APRÈS LE DÉVELOPPEMENT
L’IA doit :
	•	indiquer les fichiers modifiés ;
	•	résumer les changements réels ;
	•	fournir les tests réalisés ;
	•	signaler les tests non réalisés ;
	•	documenter les limites restantes ;
	•	mettre à jour l’état des fonctions ;
	•	mettre à jour cette Bible si une règle de conception a été validée ;
	•	ne jamais prétendre avoir modifié ou déployé un élément qu’elle n’a pas réellement modifié ou déployé.
38. TESTS MINIMAUX
Selon la fonctionnalité, vérifier :
	•	fonctionnement normal ;
	•	erreurs ;
	•	doublons ;
	•	permissions ;
	•	persistance ;
	•	reprise après actualisation ;
	•	reconnexion ;
	•	cohérence entre l’interface et la base de données ;
	•	sécurité des accès ;
	•	comportement en cas d’interruption réseau.
 
⸻
 
PARTIE XIII — ORGANISATION DES DOCUMENTS
39. STRUCTURE RECOMMANDÉE
Dans le dossier du projet, créer un dossier BIBLE_DU_JEU contenant progressivement :
	•	BIBLE_DU_JEU.md — vision et règles centrales ;
	•	PERSONNAGES.md — catalogue et fiches détaillées ;
	•	ROYAUMES_ET_CARTES.md — régions et lieux ;
	•	QUETES_ET_HISTOIRES.md — quêtes principales, secondaires et légendaires ;
	•	MISSIONS.md — missions détaillées et conditions de validation ;
	•	RECOMPENSES_ET_PROGRESSION.md — expérience, niveaux et objets ;
	•	COMPAGNONS_ET_ARTISANAT.md — compagnons, montures et fabrication ;
	•	CIVILISATION_ET_CONSTRUCTIONS.md — refuges, guildes, villes et royaumes ;
	•	MONDE_REEL_ET_PARTENAIRES.md — carte réelle et activités partenaires ;
	•	GUIDE_DEVELOPPEMENT_IA.md — règles de travail pour les IA ;
	•	IDEES_A_DEVELOPPER.md — idées futures et décisions en attente ;
	•	JOURNAL_DES_DECISIONS.md — décisions validées, datées et expliquées.
Cette structure est une recommandation. Les fichiers ne doivent être déclarés créés que lorsqu’ils existent réellement.
40. SYNCHRONISATION ENTRE LES VERSIONS
La Bible doit être conservée dans le dossier de travail principal et copiée dans une autre version uniquement après vérification.
Lorsqu’une nouvelle version du projet est créée :
	•	conserver la Bible ;
	•	conserver le cahier des charges ;
	•	conserver l’état des fonctions ;
	•	conserver les décisions validées ;
	•	vérifier les différences entre les versions ;
	•	éviter d’écraser des documents plus récents par une ancienne copie.
 
⸻
 
PARTIE XIV — IDÉES À DÉVELOPPER
41. PERSONNAGES
	•	Compléter les fiches des personnages existants.
	•	Vérifier les 50 emplacements classiques et les 50 emplacements du Monde de la Nuit.
	•	Identifier les noms provisoires.
	•	Définir progressivement les histoires, compétences, apparences et quêtes personnelles.
	•	Éviter de créer des personnages en double.
42. QUÊTES ET MISSIONS
	•	Créer un catalogue de quêtes principales.
	•	Développer des quêtes secondaires pour chaque région.
	•	Créer des missions d’exploration, de collecte et d’artisanat.
	•	Concevoir des quêtes légendaires.
	•	Définir des objectifs de guilde et de construction.
	•	Développer des quêtes secrètes.
	•	Définir des missions réelles facultatives et leurs méthodes de validation.
	•	Créer un système de suivi des missions.
	•	Tester la sauvegarde et empêcher les récompenses en double.
43. MONDE ET CIVILISATION
	•	Détailler les cartes des royaumes.
	•	Relier les régions aux quêtes.
	•	Concevoir les refuges et avant-postes.
	•	Définir les règles des guildes et alliances.
	•	Développer les constructions persistantes.
	•	Définir les règles de propriété et de gouvernance.
	•	Préparer les sauvegardes serveur.
44. PROGRESSION ET ÉCONOMIE
	•	Documenter les niveaux et l’expérience existants.
	•	Équilibrer les récompenses.
	•	Définir les ressources virtuelles.
	•	Concevoir l’artisanat.
	•	Distinguer les récompenses virtuelles des récompenses réelles.
	•	Définir les conditions de financement des récompenses partenaires.
45. MONDE RÉEL
	•	Concevoir les profils de producteurs et d’artisans.
	•	Définir les informations affichées sur la carte réelle.
	•	Définir les règles de consentement et de localisation.
	•	Concevoir les missions de visite.
	•	Définir les vérifications nécessaires.
	•	Documenter les conditions commerciales des partenaires.
 
⸻
GREENLEAF WORLD 3.1 — COMPLÉMENT GLOBAL À LA BIBLE

Histoire, sciences, religions, mythologies, fantasy, exploration, événements, sports et liberté créatrice

Statut : complément de conception à intégrer à la Bible existante.

Ce document rassemble les orientations définies pour enrichir GreenLeaf World 3.1. Il complète les travaux précédents sans les remplacer, sans figer les idées encore à développer et sans prétendre que les fonctionnalités décrites sont déjà codées.

⸻

1. VISION GÉNÉRALE DE GREENLEAF WORLD

GreenLeaf World est un univers d’exploration, de découverte, de connaissances, d’aventure, de fantasy, de sport et de création communautaire.

Le jeu relie le monde réel au monde virtuel : les lieux, les cultures, les histoires, les événements et les découvertes du monde réel nourrissent les aventures virtuelles. En retour, les aventures du jeu peuvent donner envie d’apprendre, de voyager, de découvrir des lieux et de mieux comprendre le monde.

Devise centrale :

« Le monde réel nourrit le monde virtuel. Le monde virtuel donne envie de découvrir le monde réel. »

GreenLeaf World doit permettre à chaque joueur de choisir sa façon de jouer. Certains voudront découvrir l’histoire et les sciences, d’autres explorer la carte, résoudre des mystères, pratiquer des activités sportives, développer leur personnage, créer des quêtes, participer à la vie communautaire ou simplement s’amuser.

Le jeu doit pouvoir accueillir aussi bien une enquête historique sérieuse qu’une aventure fantastique complètement absurde.

L’objectif n’est pas de prévoir toutes les aventures à l’avance, mais de construire un monde riche, cohérent et suffisamment ouvert pour que les joueurs puissent continuellement l’enrichir.

2. HISTOIRE, CIVILISATIONS ET PATRIMOINE

L’histoire réelle constitue un pilier important du jeu.

Les joueurs pourront découvrir des civilisations, des personnages historiques, des villes anciennes, des routes commerciales, des explorations, des inventions, des monuments, des sites archéologiques, des migrations et des événements qui ont marqué l’histoire humaine.

Exemples de pistes à développer :

	•	les routes de la soie et les échanges entre civilisations ;
	•	Alexandrie et l’histoire des savoirs dans l’Antiquité ;
	•	les voyages vikings et leurs itinéraires ;
	•	le mécanisme d’Anticythère et les connaissances techniques anciennes ;
	•	l’astronomie et les calendriers des civilisations mayas ;
	•	Pompéi et la vie quotidienne dans le monde romain ;
	•	les grandes routes maritimes, les explorations et les échanges culturels ;
	•	les monuments, les sites historiques et les traditions locales.

Ces pistes sont des idées de recherche, et non des scénarios déjà finalisés.

Chaque histoire doit être replacée dans son époque et son contexte géographique. Les frontières actuelles doivent être distinguées des territoires historiques. Les récits historiques doivent s’appuyer sur des sources adaptées et signaler les incertitudes lorsqu’elles existent.

Une aventure ne doit pas déplacer artificiellement un événement vers un lieu sans rapport avec son origine. Lorsqu’une quête est liée à un site réel, le jeu doit expliquer son importance historique et géographique.

Le patrimoine doit être abordé avec respect : aucune quête ne doit encourager la dégradation d’un monument, le prélèvement d’objets archéologiques, l’intrusion dans un site interdit ou la perturbation d’un lieu protégé.

3. SCIENCES ET GRANDES DÉCOUVERTES

La science constitue un autre pilier majeur de GreenLeaf World.

Les joueurs pourront explorer :

	•	Astronomie et cosmos : étoiles, galaxies, planètes, exoplanètes et exploration spatiale.
	•	Géologie : volcans, minéraux, reliefs, séismes et formation de la Terre.
	•	Paléontologie et évolution : fossiles, espèces disparues et évolution du vivant.
	•	Physique et chimie : matière, énergie, phénomènes naturels et expériences.
	•	Archéologie : méthodes de recherche, objets anciens, traces et interprétation des découvertes.
	•	Biodiversité : espèces animales et végétales, écosystèmes et interactions naturelles.
	•	Histoire des sciences : inventions, instruments, découvertes et évolution des connaissances.

Ces connaissances pourront être transformées en énigmes, missions, observations, expériences virtuelles, expéditions et aventures éducatives.

Le jeu doit distinguer :

	•	les faits scientifiques établis ;
	•	les hypothèses et modèles scientifiques ;
	•	les questions encore ouvertes ;
	•	les théories non démontrées ;
	•	les inventions fantastiques propres à GreenLeaf World.

Une hypothèse ne doit pas être présentée comme une certitude. Une question encore étudiée ne doit pas être présentée comme un mystère insoluble sans fondement.

Les expériences réelles proposées doivent être légales, sûres et adaptées au public concerné. Les expériences dangereuses doivent rester virtuelles ou être remplacées par des activités sans risque.

4. RELIGIONS, SPIRITUALITÉS ET TRADITIONS

GreenLeaf World pourra proposer la découverte des religions anciennes et vivantes, des traditions spirituelles, des textes, des lieux sacrés, des récits de création et de leur influence sur les sociétés.

L’objectif est de comprendre les cultures et les traditions, sans imposer de croyance ni établir de classement entre les religions.

Principes à respecter :

	•	présenter les traditions dans leur contexte historique et culturel ;
	•	distinguer les croyances, les doctrines, les traditions orales, les interprétations historiques et les faits scientifiques ;
	•	reconnaître qu’une même religion ou tradition peut comporter plusieurs courants et interprétations ;
	•	éviter les caricatures et les généralisations ;
	•	respecter les lieux sacrés, les pratiques et les communautés concernées ;
	•	ne pas présenter une croyance comme une preuve scientifique ni transformer un fait scientifique en doctrine religieuse.

Une grande saga sur l’origine de l’univers pourrait proposer plusieurs parcours complémentaires :

	1	Le parcours scientifique : formation de l’univers, étoiles, planètes et évolution des connaissances.
	2	Le parcours des traditions : récits de création et visions du monde présentés selon leurs cultures et leurs sources.
	3	Le parcours fantastique : une cosmogonie originale inventée pour GreenLeaf World.

Ces parcours peuvent coexister sans être confondus. Le joueur peut les explorer librement.

5. MYTHOLOGIES, LÉGENDES ET FOLKLORE

Les mythologies, les légendes, les contes, les traditions orales et les récits folkloriques peuvent inspirer des personnages, des royaumes, des créatures, des objets, des énigmes et des sagas.

Chaque tradition doit être replacée dans son contexte géographique et culturel. Les cultures d’un continent ne doivent pas être traitées comme si elles formaient un ensemble uniforme.

Lorsque plusieurs versions d’un récit existent, le jeu peut présenter les différences et expliquer d’où proviennent les variantes.

Pistes à étudier :

	•	l’Épopée de Gilgamesh ;
	•	les textes funéraires de l’Égypte ancienne, souvent désignés sous le titre moderne de Livre des morts ;
	•	la descente d’Inanna dans le monde souterrain ;
	•	le récit d’Orphée et Eurydice ;
	•	les traditions nordiques autour d’Yggdrasil et des différents mondes ;
	•	les créatures et traditions propres à différentes cultures du monde.

Ces exemples devront faire l’objet de recherches avant de devenir des contenus historiques ou culturels documentés.

Les légendes pourront également inspirer des aventures fantastiques originales. Le jeu devra alors distinguer le récit traditionnel de ce qui a été inventé spécialement pour GreenLeaf World.

6. MYSTÈRES, ENQUÊTES ET ÉNIGMES

GreenLeaf World doit accueillir des enquêtes historiques, scientifiques, archéologiques, culturelles et cryptographiques, mais aussi des mystères entièrement fictifs.

Le jeu doit distinguer cinq catégories :

	1	les faits établis ;
	2	les éléments incertains ou débattus ;
	3	les mystères populaires dont certaines explications sont déjà connues ;
	4	les théories et hypothèses des joueurs ;
	5	les mystères inventés pour l’histoire du jeu.

Une énigme fantastique peut rester mystérieuse aussi longtemps que nécessaire pour le récit. Une affirmation sur le monde réel, en revanche, doit être présentée avec le niveau de certitude approprié.

Les joueurs pourront découvrir des indices, proposer des hypothèses, comparer leurs interprétations et partager leurs découvertes.

Pistes possibles : le mécanisme d’Anticythère, certaines inscriptions anciennes, des énigmes cryptographiques et des jeux d’enquête historiques ou contemporains.

Le statut réel de chaque mystère devra être vérifié avant de le présenter comme non résolu.

7. ANCRAGE GÉOGRAPHIQUE DES HISTOIRES ET DES PERSONNAGES

La géographie est une composante fondamentale du jeu. Elle influence les histoires, les cultures, les déplacements, les conflits, les royaumes et les missions.

Pour chaque personnage ou récit lié au monde réel, prévoir, lorsque les informations sont disponibles :

	•	le continent, le pays et la région ;
	•	le lieu précis ou le site concerné ;
	•	la période historique ;
	•	la civilisation, la culture ou la tradition ;
	•	les déplacements historiques connus ;
	•	les sources et le niveau de certitude ;
	•	le statut du contenu : fait documenté, tradition, hypothèse ou fiction.

Si l’origine exacte d’un personnage ou d’un événement est inconnue, il faut le signaler plutôt que d’inventer une origine historique.

Les quêtes pourront proposer quatre modes :

	•	À distance : le joueur apprend, enquête ou résout une énigme depuis le jeu.
	•	Sur place : une visite réelle est nécessaire pour valider cette version de la quête.
	•	Hybride : une partie virtuelle et une partie réelle, clairement distinguées.
	•	Fantastique : toute l’action se déroule dans l’univers inventé.

Une quête qui exige réellement un déplacement ne doit pas prétendre avoir validé une visite lorsque le joueur a uniquement effectué la version virtuelle. Une alternative virtuelle peut néanmoins permettre de découvrir l’histoire sans voyager.

Aucune mission ne doit imposer une intrusion, une prise de risque, une entrée dans une propriété privée, une perturbation d’un site patrimonial ou un contact avec un inconnu.

8. FANTASY ET ROYAUMES ORIGINAUX

La fantasy est un pilier à part entière de GreenLeaf World. Elle ne doit pas être limitée à une décoration ajoutée sur la carte réelle.

Le jeu pourra développer des royaumes inventés, des peuples, des créatures, des pouvoirs, des portails, des conflits, des objets magiques et des histoires originales.

Concepts à approfondir, non définitifs :

Royaume des Terres Vivantes
Forêts changeantes, montagnes mystérieuses, cités cachées et territoires dont la géographie semble évoluer.

Royaume des Ombres
Portes qui disparaissent, lieux façonnés par les souvenirs et secrets oubliés.

Îles du Ciel
Îles flottantes, routes aériennes, cités suspendues et créatures capables de traverser les nuages.

Royaume Englouti
Civilisation imaginaire sous les eaux, cités submergées et secrets liés aux profondeurs.

Autres amorces narratives :

	•	les Sept Portes du Monde souterrain ;
	•	le Manuscrit des noms effacés ;
	•	la Forêt qui se souvient ;
	•	l’Observatoire de la dernière nuit.

Ces idées restent des pistes créatives à développer. Elles ne constituent pas des fonctionnalités déjà codées.

La carte, les royaumes, les histoires et les quêtes doivent être conçus ensemble : la géographie donne forme aux aventures, les histoires expliquent les conflits et les missions permettent aux joueurs d’explorer cet univers.

9. LA CARTE COMMUNE ET SES TROIS COUCHES

GreenLeaf World doit utiliser une carte commune sur laquelle plusieurs couches peuvent se superposer, et non trois cartes totalement séparées.

9.1 Couche du monde réel

Elle représente notamment les pays, les villes, les reliefs, les sites historiques, les lieux culturels, les sentiers autorisés et les événements réels.

9.2 Couche fantastique

Elle ajoute les royaumes inventés, les créatures, les portails, les arènes, les territoires imaginaires et les quêtes fantastiques.

9.3 Couche Fantôme / Monde de la Nuit

Elle contient des territoires cachés, des aventures nocturnes, des secrets et des contenus réservés aux joueurs autorisés.

Les joueurs doivent pouvoir comprendre ce qui appartient au monde réel et ce qui relève de la fiction.

L’accès à la couche Fantôme doit être protégé techniquement par le système d’autorisation du projet. Masquer simplement un bouton dans l’interface ne suffit pas : les données et les opérations réservées doivent être contrôlées côté serveur et par les règles d’accès appropriées.

L’autorisation technique d’accéder au contenu et la progression narrative dans ce contenu sont deux notions différentes.

La géolocalisation doit rester facultative, transparente et soumise au consentement du joueur. Sa position précise ne doit pas être publiée automatiquement.

10. ÉVÉNEMENTS DU MONDE RÉEL

La carte peut accueillir des événements liés à un lieu et à une date :

	•	fêtes nationales et célébrations culturelles ;
	•	fêtes de village, marchés et journées du patrimoine ;
	•	festivals, concerts et événements associatifs ;
	•	tournois, courses, randonnées organisées et initiations sportives ;
	•	quiz, soirées à thème et rencontres publiques ;
	•	événements proposés par des partenaires locaux.

Exemples d’inspiration : le 14 juillet en France, la Saint-Patrick en Irlande, les fêtes locales et les journées du patrimoine.

Les événements précis doivent être vérifiés avant d’être présentés comme confirmés. La fiche d’un événement doit indiquer, lorsque les informations sont disponibles, sa source, sa date, ses horaires, son lieu, ses conditions d’accès, ses éventuels frais et les informations d’accessibilité.

Un événement réel pourra inspirer une quête temporaire, faire apparaître un personnage, révéler un indice ou déclencher un événement fantastique. Le jeu ne doit pas laisser croire qu’un organisateur réel soutient une activité virtuelle sans accord explicite.

La participation ne doit pas imposer une dépense, un achat, une consommation d’alcool ou une activité sociale. Des alternatives gratuites ou virtuelles pourront être proposées lorsque cela est pertinent.

Les récompenses liées à ces événements peuvent être entièrement virtuelles : badges, objets, titres, expérience ou évolution temporaire d’un territoire.

11. SPORTS ET ACTIVITÉS PHYSIQUES

Le sport doit être une autre manière de jouer, de découvrir et de progresser, sans devenir une obligation. Les joueurs choisissent les activités qui leur plaisent et leur niveau de participation.

11.1 Familles d’activités

Football et sports collectifs : football, basket, volley, handball, rugby, badminton, tennis en double et autres disciplines collectives.

Yoga, respiration et équilibre : yoga, mobilité douce, étirements et exercices de respiration.

Arts martiaux et sports de combat : karaté, judo, taekwondo, boxe, lutte, jiu-jitsu et autres disciplines, avec découverte de leur histoire et de leurs principes.

Marche, randonnée et exploration : balades, sentiers autorisés, paysages, villages, monuments et sites naturels accessibles.

Vélo, course et endurance : cyclisme, jogging, course à pied, marche rapide et défis personnels facultatifs.

Danse, fitness et gymnastique : danse, coordination, souplesse, gymnastique et activités adaptées.

Natation et activités aquatiques : découverte des disciplines aquatiques et missions virtuelles liées aux océans, aux rivières et aux civilisations maritimes.

Musculation et préparation physique : renforcement musculaire, équilibre, mobilité et progression personnelle.

Sports fantastiques : courses de dragons, golf volcanique, courses d’escargots, tournois de chevaliers en pantoufles et autres disciplines inventées.

11.2 Formats de quêtes sportives

	•	Défi réel : activité pratiquée dans le monde réel.
	•	Défi virtuel : mini-jeu, quiz, simulation ou compétition imaginaire.
	•	Défi hybride : activité réelle facultative reliée à une aventure virtuelle.
	•	Défi communautaire : épreuve inventée par un joueur ou une équipe.

Exemples : découvrir l’histoire d’un art martial, participer à un match amical, explorer un sentier autorisé, apprendre une danse, organiser un tournoi fantastique ou accomplir une activité adaptée à son niveau.

Les défis réels doivent respecter la sécurité, la légalité et les capacités de chacun. Aucune récompense ne doit favoriser exclusivement la vitesse, la force ou l’endurance. Les alternatives virtuelles et les adaptations accessibles doivent pouvoir compter elles aussi.

Le jeu ne doit jamais encourager un défi dangereux, une intrusion ou l’utilisation du téléphone en regardant l’écran pendant une activité qui exige de l’attention.

11.3 Progression et récompenses sportives

Les récompenses peuvent comprendre :

	•	de l’expérience ;
	•	des titres et badges ;
	•	des équipements et tenues virtuels ;
	•	des décorations et améliorations de territoires ;
	•	des récompenses collectives pour les équipes ;
	•	des événements et quêtes débloqués.

Les données sportives personnelles et les habitudes de déplacement ne doivent pas être publiques par défaut.

12. LIBERTÉ CRÉATRICE DES JOUEURS

GreenLeaf World doit être un jeu vivant, pas une encyclopédie où chaque idée doit passer un examen avant d’exister.

Les joueurs peuvent inventer des quêtes sérieuses, humoristiques, absurdes, imprévisibles, spontanées ou complètement délirantes.

Principe central :

« La créativité des joueurs est libre dans le monde du jeu. Les règles protègent les personnes dans le monde réel, pas contre les idées farfelues. »

Une création fictive n’a pas besoin d’être vérifiée comme un fait historique. Elle doit simplement être identifiée comme une fiction ou une création de joueur et respecter les règles qui protègent les personnes.

Exemples de déconnage :

	•	aider un dragon à devenir président du Royaume des Champignons ;
	•	organiser une course d’escargots avec des dragons comme arbitres ;
	•	livrer une pizza à un dragon grincheux ;
	•	retrouver les chaussettes magiques d’un roi ;
	•	organiser un tournoi de chevaliers en pantoufles ;
	•	aider un sorcier qui a perdu ses pouvoirs après avoir oublié son mot de passe ;
	•	arbitrer un match de football contre un canard qui refuse de rendre le ballon.

Ces exemples ne sont pas des scénarios imposés. Ils illustrent le niveau de liberté créative souhaité.

Les joueurs doivent pouvoir inventer des idées encore plus étranges, les partager et leur donner une suite. L’humour et l’absurde font partie de l’identité du jeu.

13. CRÉATIONS COMMUNAUTAIRES ET CHAÎNES D’AVENTURES

Une découverte effectuée par un joueur peut déclencher une nouvelle quête pour d’autres joueurs.

Exemple de fonctionnement :

	1	Un joueur termine une quête et découvre un indice, un secret ou une idée.
	2	Il partage cette découverte dans le jeu.
	3	Il crée une quête ou une mission à partir de cette découverte.
	4	D’autres joueurs participent et apportent leurs propres éléments.
	5	Leurs découvertes peuvent donner naissance à de nouvelles quêtes.
	6	Une chaîne d’aventures peut ainsi se développer au fil de la communauté.

Les joueurs pourront proposer des énigmes, des personnages, des histoires, des défis, des pistes géographiques, des événements communautaires, des créations humoristiques et des règles de jeu originales.

Les créations pourront être proposées à des amis, à un groupe ou à la communauté. Les plus appréciées pourront inspirer d’autres joueurs ou être proposées pour devenir des quêtes officielles, avec crédit au créateur d’origine.

13.1 Statuts de contenu proposés

	•	Brouillon ou privé : visible par le créateur ou le groupe qu’il choisit.
	•	Création de joueur publiée : accessible à la communauté avec une indication claire de son origine.
	•	Création mise en avant : appréciée ou sélectionnée par la communauté.
	•	Contenu officiel : intégré ou adapté par l’équipe du jeu.
	•	Contenu factuel documenté : les affirmations présentées comme historiques, scientifiques ou géographiques disposent de sources adaptées.

Une création humoristique n’a pas besoin d’une validation historique. Lorsqu’une quête mêle fiction et faits réels, la différence doit rester compréhensible.

14. MODÉRATION : PROTÉGER LES PERSONNES SANS ÉTOUFFER L’IMAGINATION

La modération doit cibler les risques concrets :

	•	harcèlement et menaces ;
	•	divulgation d’informations privées ;
	•	incitation à des actes dangereux ou illégaux ;
	•	intrusions ou mises en danger de personnes ;
	•	contenu abusif visant des personnes ou des groupes ;
	•	autres contenus réellement nuisibles selon les règles du jeu.

Une idée ne doit pas être supprimée simplement parce qu’elle est étrange, irrévérencieuse, absurde ou décalée.

Les joueurs doivent disposer de mécanismes simples pour signaler les contenus nuisibles. La modération doit préserver la liberté de création tout en intervenant lorsque la sécurité, la vie privée ou les droits d’autrui sont réellement menacés.

La distinction fondamentale est la suivante : la liberté est grande dans le monde imaginaire ; les règles protègent les personnes dans le monde réel.

15. TON ET IDENTITÉ DE GREENLEAF WORLD

GreenLeaf World doit pouvoir passer naturellement entre plusieurs ambiances :

	•	sérieux et documenté pour l’histoire et les sciences ;
	•	respectueux pour les religions, les cultures et les traditions ;
	•	mystérieux pour les enquêtes et les secrets ;
	•	épique pour les sagas et les royaumes fantastiques ;
	•	convivial pour le sport et les événements ;
	•	absurde et imprévisible pour les créations humoristiques.

Le jeu peut proposer une enquête archéologique le matin et une élection présidentielle organisée par des champignons le soir.

Ce contraste fait partie de son identité. Il permet aux joueurs de choisir entre apprentissage, exploration, aventure, compétition, créativité et humour.

Le déconnage n’est pas seulement un décor : il peut produire des quêtes, des personnages, des objets, des événements temporaires, des compétitions et des sagas qui évoluent selon les décisions des joueurs.

16. ORGANISATION DOCUMENTAIRE PROPOSÉE POUR LA BIBLE

Les rubriques suivantes peuvent compléter l’organisation déjà existante, sans imposer de réorganiser les chapitres précédents :

	1	Histoires réelles et civilisations.
	2	Sciences et découvertes.
	3	Religions, spiritualités et traditions.
	4	Mythologies, légendes et folklore.
	5	Mystères, enquêtes et énigmes.
	6	Ancrage géographique des personnages et des récits.
	7	Royaumes, fantasy et univers originaux.
	8	Carte commune et couches du monde.
	9	Événements du monde réel.
	10	Sports et activités physiques.
	11	Quêtes et missions réelles, virtuelles et hybrides.
	12	Créations communautaires et chaînes de quêtes.
	13	Humour, absurdité et déconnage.
	14	Sources, statuts de contenu et règles de sécurité.

Il s’agit d’une proposition de classement. Chaque rubrique peut être placée là où elle s’intègre le mieux dans la Bible déjà commencée.

17. MODÈLE DE FICHE DE CONTENU

Titre :
Type : histoire réelle / science / religion ou tradition / mythe ou légende / mystère / fantasy originale / sport / événement / création de joueur
Origine géographique :
Période, date ou durée :
Culture, civilisation ou contexte :
Résumé :
Éléments établis :
Incertitudes ou variantes :
Partie fictive, si applicable :
Idée de quête ou de mission :
Mode : réel / virtuel / hybride / entièrement fictif
Conditions de sécurité et d’accessibilité :
Sources, si nécessaire :
Statut : brouillon / création de joueur / documenté / proposé comme contenu officiel
Créateur ou contributeur :

Pour une création purement humoristique, les champs de recherche historique peuvent être omis. Pour un événement réel, la date, le lieu et la source doivent être renseignés avant de le présenter comme confirmé. Pour un contenu scientifique ou historique présenté comme factuel, les sources et les incertitudes doivent être précisées.

18. PRINCIPES À CONSERVER POUR LES DÉVELOPPEMENTS FUTURS

	1	Compléter le travail existant sans le remplacer.
	2	Concevoir l’histoire, les royaumes et la carte ensemble.
	3	Distinguer clairement les faits, les traditions, les hypothèses et la fiction.
	4	Utiliser le monde réel comme source d’inspiration sans imposer de déplacements.
	5	Maintenir une carte commune avec des couches complémentaires.
	6	Protéger techniquement les contenus réservés, notamment la couche Fantôme.
	7	Permettre aux joueurs d’inventer librement des quêtes, y compris absurdes.
	8	Laisser les découvertes des joueurs déclencher de nouvelles aventures.
	9	Intégrer les sports et les événements sans en faire une obligation.
	10	Protéger les personnes sans censurer les idées farfelues.
	11	Ne pas présenter une idée de conception comme une fonctionnalité déjà codée.
	12	Développer progressivement les modules et les intégrer à l’architecture existante de GreenLeaf World 3.1.

GREENLEAF WORLD 3.1

COMPLÉMENT À LA BIBLE — MAPS INTERCONNECTÉES, CIVILISATIONS ET DIFFICULTÉ DES QUÊTES

Statut : spécification de conception à intégrer à la Bible du projet. Les fonctionnalités décrites sont des objectifs de développement et ne sont pas considérées comme déjà codées sans vérification.

⸻

1. CONCEPT GÉNÉRAL DES MAPS

GreenLeaf World possède un univers fantastique composé de plusieurs maps interconnectées.

La géographie réelle du monde sert de fondation à cet univers. Les continents, pays, régions, montagnes, fleuves, forêts, déserts, îles et villes inspirent la disposition des territoires. Les décors fantastiques, les civilisations anciennes, les créatures, les portails, les donjons, les royaumes cachés et les lieux mystérieux enrichissent cet environnement.

Il ne doit pas exister une carte réelle indépendante et une carte fantastique séparée. Le joueur explore des maps fantastiques fondées sur une géographie réelle, avec des représentations adaptées à chaque région, civilisation, époque ou aventure.

Les maps appartiennent toutes au même univers GreenLeaf World et peuvent être reliées par des quêtes, des personnages, des objets, des découvertes et des sagas.

Principe fondamental : une seule grande aventure, plusieurs maps, des mondes qui se dévoilent progressivement.

2. PROGRESSION ET DÉBLOCAGE DES MAPS

Les maps, régions et zones peuvent se débloquer progressivement en fonction :

	•	du niveau du joueur ;
	•	des quêtes accomplies ;
	•	des indices et découvertes ;
	•	des objets ou reliques obtenus ;
	•	des compétences acquises ;
	•	des énigmes résolues ;
	•	de la progression dans une saga ;
	•	de conditions particulières définies par certaines aventures.

Le niveau général d’une map représente sa place dans la progression globale, mais il ne détermine pas automatiquement la difficulté de toutes les quêtes qu’elle contient.

Plusieurs chemins de progression doivent être possibles. Le joueur peut privilégier l’histoire, l’exploration, les sciences, les mystères, les activités sportives, l’humour, les aventures fantastiques ou les missions communautaires.

Le jeu doit encourager la curiosité et l’exploration plutôt que d’imposer un parcours unique.

3. RETOUR LIBRE SUR LES ANCIENNES MAPS

Toute map déjà débloquée reste accessible au joueur, même lorsqu’il atteint des niveaux supérieurs.

Le joueur doit pouvoir revenir sur une ancienne map pour :

	•	terminer les quêtes qu’il n’a pas encore accomplies ;
	•	reprendre une mission interrompue ;
	•	retrouver des objets ou indices ;
	•	découvrir des passages secrets ;
	•	compléter son codex ;
	•	obtenir des récompenses encore disponibles ;
	•	utiliser des compétences nouvellement acquises ;
	•	découvrir des quêtes ou événements ajoutés ultérieurement.

La progression d’une map ne doit pas être effacée lorsqu’une autre map est débloquée.

Les conditions de progression doivent être enregistrées séparément pour chaque quête et chaque map : étapes validées, indices trouvés, objets obtenus, zones découvertes et récompenses récupérées.

Certaines zones peuvent nécessiter une clé, une quête préalable ou une condition narrative précise. Ces restrictions doivent être explicites et ne doivent pas empêcher arbitrairement le joueur de retourner explorer les anciennes maps.

4. DIFFICULTÉ MÉLANGÉE DANS TOUTES LES MAPS

Règle obligatoire : chaque map doit proposer un mélange de quêtes faciles, intermédiaires et difficiles.

Aucune map ne doit être constituée uniquement de quêtes difficiles sous prétexte qu’elle correspond à un niveau avancé. De même, une map de début de jeu peut proposer quelques défis exigeants, clairement identifiés, pour les joueurs qui souhaitent les tenter.

La difficulté dépend de chaque quête, et non uniquement du niveau général de la map.

4.1. Quêtes faciles

Exemples :

	•	découvrir un lieu ;
	•	observer un monument ou un paysage ;
	•	retrouver un objet ;
	•	rencontrer un personnage ;
	•	répondre à une question ;
	•	résoudre une énigme courte ;
	•	identifier un symbole ;
	•	accomplir une petite mission d’exploration.

Ces quêtes permettent de jouer rapidement, d’apprendre, de gagner de l’expérience et d’obtenir des récompenses utiles.

4.2. Quêtes intermédiaires

Exemples :

	•	relier plusieurs indices ;
	•	explorer plusieurs points d’une map ;
	•	résoudre une énigme en plusieurs étapes ;
	•	reconstituer un événement historique ;
	•	fabriquer ou retrouver un objet particulier ;
	•	combiner plusieurs compétences ;
	•	suivre une piste laissée par un personnage.

Ces quêtes offrent un défi plus développé sans exiger systématiquement une longue préparation.

4.3. Quêtes difficiles

Exemples :

	•	résoudre une enquête complexe ;
	•	accomplir une longue saga ;
	•	déchiffrer plusieurs énigmes liées ;
	•	réunir des objets rares ;
	•	affronter un défi stratégique ;
	•	coordonner plusieurs compétences ;
	•	participer à une aventure collective exigeante.

Ces quêtes peuvent offrir des récompenses rares ou ouvrir des parties importantes de l’histoire. Le joueur doit cependant pouvoir les mettre en attente et continuer à jouer ailleurs.

4.4. Quêtes secrètes

Certaines missions se révèlent après une découverte, une rencontre, la collecte d’un indice, l’obtention d’un objet ou l’accomplissement d’une autre quête.

Leur difficulté peut être facile, intermédiaire ou difficile. Une quête secrète n’est pas nécessairement une quête difficile.

4.5. Quêtes humoristiques et absurdes

GreenLeaf World peut proposer des missions amusantes, décalées ou volontairement absurdes.

Exemples :

	•	aider un personnage fictif à retrouver sa couronne perdue ;
	•	résoudre une énigme dont les indices sont volontairement loufoques ;
	•	participer à une compétition fantaisiste ;
	•	accomplir une mission parodique dans un royaume imaginaire.

La créativité et l’humour font partie intégrante du jeu. Les règles de sécurité s’appliquent aux actions réelles proposées, sans empêcher les idées absurdes dans l’univers virtuel.

4.6. Quêtes collectives et communautaires

Certaines missions peuvent être accomplies à plusieurs, nécessiter une coopération ou faire progresser une histoire commune.

Elles peuvent être faciles, intermédiaires ou difficiles. Les joueurs qui préfèrent jouer seuls doivent conserver suffisamment d’activités accessibles pour progresser.

4.7. Quêtes d’apprentissage et de découverte

Les quêtes peuvent porter sur :

	•	l’histoire et l’archéologie ;
	•	les sciences et les inventions ;
	•	la géographie et l’environnement ;
	•	les cultures et les traditions ;
	•	les mythologies et les légendes ;
	•	les langues, les arts et la philosophie ;
	•	les mystères, les enquêtes et les hypothèses ;
	•	les sports, les activités et les événements.

Le thème d’une quête ne fixe pas sa difficulté. Une quête scientifique peut être très simple ou extrêmement complexe.

5. LIBERTÉ DE JEU ET ABSENCE D’IMPASSE

Le joueur ne doit jamais être contraint de terminer immédiatement une quête difficile pour continuer à profiter de GreenLeaf World.

Il peut :

	1	tenter une quête ;
	2	la mettre en pause ;
	3	choisir une quête plus facile ;
	4	changer de map déjà débloquée ;
	5	gagner de l’expérience et découvrir de nouveaux éléments ;
	6	revenir plus tard à la quête initiale.

Le jeu conserve sa progression et les indices déjà obtenus.

Le système doit proposer plusieurs activités et plusieurs voies de progression afin qu’un joueur ne soit pas bloqué par une seule énigme, un seul combat, une seule saga ou une seule catégorie de missions.

Lorsque cela est compatible avec le scénario, des aides progressives peuvent être proposées : indice, explication, piste supplémentaire ou aide facultative. Ces aides ne doivent pas nécessairement supprimer toutes les récompenses.

6. EXEMPLE DE MIXITÉ DES QUÊTES SUR UNE MAP

Prenons la map de l’Égypte ancienne.

Le joueur peut y trouver simultanément :

	•	une quête facile d’observation de symboles ;
	•	une quête intermédiaire consistant à relier plusieurs indices ;
	•	une enquête historique difficile en plusieurs étapes ;
	•	une quête secrète révélée par une découverte ;
	•	une mission humoristique impliquant un personnage fictif ;
	•	une quête collective ;
	•	une quête de connaissance sur les sciences, les croyances ou l’histoire de l’Égypte ancienne.

Un joueur peut donc choisir une activité adaptée à son envie du moment, indépendamment de son niveau général ou de la difficulté des autres missions de cette map.

Le même principe s’applique à toutes les maps historiques, culturelles et fantastiques.

7. CIVILISATIONS ET MONDES À INTÉGRER

GreenLeaf World pourra intégrer progressivement différentes civilisations et périodes historiques, notamment :

	•	Mésopotamie et Sumériens : premières cités, écriture cunéiforme, temples et histoire des sociétés anciennes.
	•	Monde maya : cités, architecture, astronomie, calendriers et histoire des peuples mayas.
	•	Égypte ancienne : Nil, temples, monuments, savoirs, croyances et histoire.
	•	Empires perses : Perse antique, Persépolis, routes, administration et échanges culturels.
	•	Grèce antique : philosophie, sciences, cités, histoire et mythologie.
	•	Rome antique : routes, villes, ingénierie, monuments et histoire impériale.
	•	Civilisations andines et incas : Andes, architecture, agriculture et histoire.
	•	Civilisations africaines : royaumes, empires, villes, traditions et savoirs de différentes régions.
	•	Civilisations asiatiques : Chine ancienne, Inde historique, Japon et autres cultures.
	•	Cultures de l’Amazonie : peuples, territoires, savoirs et histoires propres aux régions amazoniennes.
	•	Autres civilisations et périodes historiques : ajoutées progressivement selon les contenus et les sources disponibles.
	•	Royaumes fantastiques originaux : territoires fictifs propres à GreenLeaf World.
	•	Mondes mystérieux et zones secrètes : régions à découvrir à travers des quêtes, des objets et des énigmes.

La liste reste ouverte et évolutive.

Les localisations doivent être historiquement et géographiquement cohérentes. Par exemple, la civilisation maya est associée à la Mésoamérique, notamment au sud-est du Mexique et à certaines régions d’Amérique centrale. Elle ne doit pas être confondue avec les cultures de l’Amazonie péruvienne.

8. ADAPTATION DES MAPS AUX QUÊTES

Lorsqu’une quête porte sur une civilisation ou une période, la map concernée peut faire apparaître des lieux, des décors, des personnages, des chemins et des points de mission adaptés à son contexte.

Une quête consacrée aux Perses peut, par exemple, ouvrir une région inspirée de la Perse antique et révéler des missions autour de Persépolis, des routes historiques ou des échanges culturels.

Les nouvelles découvertes enrichissent les maps existantes et peuvent aussi ouvrir des maps spécialisées reliées au monde principal.

Les maps doivent rester cohérentes avec la géographie, les périodes et les cultures concernées, tout en conservant l’identité fantastique de GreenLeaf World.

9. HISTOIRE, LÉGENDES ET FICTION

Les contenus doivent distinguer clairement :

	•	les faits historiques documentés ;
	•	les hypothèses historiques ou scientifiques ;
	•	les traditions culturelles et religieuses ;
	•	les mythes et légendes ;
	•	les théories ou interprétations proposées par les joueurs ;
	•	la fiction originale créée pour GreenLeaf World.

Les mythes, légendes et récits religieux sont présentés dans leur contexte, sans être automatiquement assimilés à des faits historiques démontrés.

La fiction peut enrichir une région historique, mais ne doit pas être présentée comme une découverte archéologique réelle ou un fait établi.

10. RÉCOMPENSES ET PROGRESSION

Les récompenses doivent être adaptées à la difficulté, au temps nécessaire, à la rareté et à la nature de la mission.

Les quêtes faciles peuvent fournir :

	•	de l’expérience ;
	•	des ressources courantes ;
	•	des indices ;
	•	des pages de codex ;
	•	des objets de collection ;
	•	des récompenses simples mais utiles.

Les quêtes intermédiaires et difficiles peuvent offrir :

	•	des objets plus rares ;
	•	de nouvelles compétences ;
	•	des titres et des succès ;
	•	des éléments de saga ;
	•	des accès à des zones secrètes ;
	•	des objets ayant une utilité particulière ;
	•	des récompenses communautaires.

Les quêtes faciles doivent rester intéressantes sans rendre les quêtes difficiles inutiles. Les quêtes difficiles doivent être gratifiantes sans être obligatoires pour profiter de l’ensemble du jeu.

Les éventuelles récompenses réelles — réductions, billets, objets, souvenirs, événements ou activités — doivent correspondre à des offres effectivement confirmées par des partenaires. Elles doivent indiquer leurs conditions, leur période de validité et leur lieu.

11. LIEN AVEC LE MONDE RÉEL

La carte fantastique est fondée sur la géographie réelle et peut être associée au GPS avec le consentement du joueur.

Le joueur doit aussi pouvoir choisir manuellement une région ou une destination lorsque cela est possible.

Certaines quêtes sont entièrement virtuelles ; d’autres peuvent demander une visite physique. Les conditions doivent être annoncées clairement. Une quête à distance ne doit pas être présentée comme une visite réelle, et une simple position GPS ne doit pas automatiquement suffire à valider une mission.

Les aventures physiques doivent rester sûres, légales, accessibles autant que possible et respectueuses des lieux, des personnes et de la vie privée. Aucune quête ne doit encourager une intrusion, une dégradation ou une activité dangereuse.

12. PRINCIPES OBLIGATOIRES POUR LE DÉVELOPPEMENT

	1	Une carte fantastique fondée sur la géographie réelle.
	2	Plusieurs maps appartenant au même univers et reliées entre elles.
	3	Un déblocage progressif selon la progression, les quêtes et les découvertes.
	4	La possibilité de revisiter les maps déjà débloquées.
	5	La sauvegarde de la progression propre à chaque map et à chaque quête.
	6	Un mélange obligatoire de quêtes faciles, intermédiaires et difficiles dans toutes les maps.
	7	Aucune difficulté uniforme imposée par le seul niveau général d’une map.
	8	La possibilité de mettre une quête difficile en pause et de continuer ailleurs.
	9	Plusieurs voies de progression et plusieurs styles de jeu.
	10	Des récompenses équilibrées, utiles et proportionnées au défi.
	11	Une distinction claire entre histoire documentée, hypothèses, traditions, légendes et fiction.
	12	Une connexion au monde physique fondée sur le consentement, la sécurité et des règles de validation adaptées.
	13	La conservation de l’existant lors de l’intégration : les nouvelles fonctionnalités doivent s’ajouter à l’architecture déjà développée, après vérification, sans supprimer arbitrairement le travail antérieur.

⸻

PRINCIPE DIRECTEUR

Chaque map est un terrain d’aventure complet. Chaque joueur peut y trouver plusieurs niveaux de difficulté et plusieurs façons de jouer. La progression ouvre de nouveaux horizons sans effacer les anciens, et aucune quête difficile ne doit enfermer le joueur dans une impasse.

CONCLUSION

GreenLeaf World 3.1 doit devenir un univers où l’on peut apprendre, enquêter, voyager, découvrir des cultures, comprendre les sciences, explorer des mythologies, vivre des aventures fantastiques, pratiquer ou découvrir des sports, participer à des événements et inventer des quêtes avec d’autres joueurs.

Il doit être assez structuré pour préserver la fiabilité des informations et la sécurité des personnes, mais assez libre pour que l’imagination ne soit pas enfermée dans un cadre rigide.

L’objectif n’est pas de prévoir toutes les aventures à l’avance. L’objectif est de construire un monde assez riche et des outils assez souples pour que les joueurs puissent continuellement en inventer de nouvelles.

Et si cela conduit à découvrir une civilisation antique, résoudre une énigme scientifique, partir en randonnée, rencontrer une nouvelle communauté ou aider un dragon à devenir président du Royaume des Champignons, alors GreenLeaf World aura rempli sa mission. 
46. RÈGLE FINALE
GreenLeaf World doit se développer comme un monde cohérent, durable et évolutif.
Chaque nouvelle idée doit enrichir l’ensemble sans casser le travail précédent. Chaque nouvelle quête doit respecter les personnages et les royaumes. Chaque récompense doit respecter les règles d’équité. Chaque fonction connectée doit être sécurisée et testée.
La Bible est la référence de conception ; le cahier des charges fixe les exigences ; le code implémente les fonctions ; les tests démontrent ce qui fonctionne réellement.
Les règles encore incertaines restent ouvertes jusqu’à validation explicite par le créateur.
