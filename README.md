# Présentation d'un tableau de bord d'une entreprise de jouets

<img width="1428" height="802" alt="image" src="https://github.com/user-attachments/assets/ee19df9c-efb8-47cb-bad5-fa764c0688af" />

### Contexte

La base de données d'une entreprise de jouets répertorie les employés, les produits, les commandes et un peu plus encore.
Le souhait de la direction est d'avoir un tableau de bord dynamique qui pourrait être actualiser chaque matin pour obtenir les dernières informations afin de gérer l’entreprise.

#### > Schéma de la base de données

<img width="1880" height="1372" alt="image" src="https://github.com/user-attachments/assets/62432153-6328-4746-aaec-cd4f8a914baf" />

### Objectifs et enjeux

Fournir des indicateurs clés de performance (KPI) afin de présenter les données liées à la logistique.

📌 Logistique
* Stock des produits sous seuil critique : Identifier les stocks des produits les plus commandés.
* Durée moyenne de traitement des commandes : Mesurer l’efficacité opérationnelle en analysant le temps entre la date de commande et la date d’expédition.
* Valorisation des stocks : calculer la valeur du stock et identifier les 5 produits qui représentent la plus grosse valeur de ce stock.
* KPI supplémentaires au choix

L'enjeu est d'abord de **calculer les métriques en SQL** puis de **construire un dashboard dans Power BI**

#### > Détails des éléments mis en place

• Requête SQL : connaître le temps moyen de livraison par année

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/77b3c2eb-ce57-4196-93d1-caa39bbfc1ac" />

• Requête SQL : connaître les stocks des produits les plus commandés (par année)

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/1ebd6c2c-29f1-4d35-b12f-0e7dd73d104f" />

• Requête SQL : nombre de commandes en retard (par année)

<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/12b3a8f7-9f7c-4462-84b0-2068aca692a5" />

• Power BI : Tables de faits et de dimensions

<img width="1809" height="842" alt="image" src="https://github.com/user-attachments/assets/ddf5e716-82eb-4d18-b9b5-18c774b42438" />

### En résumé...

En 2024, dans le bandeau du dasbord...
<img width="1263" height="181" alt="image" src="https://github.com/user-attachments/assets/a828c1ff-82c0-422d-898b-87c952bca5de" />

* Le **premier indicateur** nous montre que 100% des commandes ont été livrées dans les temps depuis le début par rapport aux objectifs fixés. Il se base sur la comparaison de la date de livraison prévue avec la date de livraison réelle.
*	Le **deuxième indicateur** nous indique qu’actuellement les commandes sont livrées aux clients en moyenne en 3 jours. Il est possible de comparer ces indicateurs avec les valeurs des années précédentes grâce au segment en-dessous. Par exemple, en 2023 le taux de service logistique est également de 100% et que le temps de livraison moyen était de 3,5j. En 2022, le taux de service logistique était de 99% pour un temps de livraison moyen de 4,3j. Cela nous permet de constater une vraie évolution positive sur ces indicateurs clés.
*	Le **troisième indicateur** présente la valorisation du stock global. Il est actuellement de 3,05 millions d’euros. Ce KPI est intéressant mais il est peu exploitable en l’état puisqu’on ne peut pas le comparer à d’autres périodes par manque d’historique de données liés au stock. Mais il reste essentiel pour évaluer l’efficacité de la gestion des stocks et des ventes. (taux de rotation des stocks, coût moyen des stocks, valeur moyenne par période, etc.).

... dans le corps du dashboard...
<img width="1417" height="614" alt="image" src="https://github.com/user-attachments/assets/0575384b-1203-43f9-a876-42ca5fe2ccb9" />
*	Ici, on présente les **stocks des 5 produits les plus commandés** au cours des 3 dernières années. Les produits sont présentés par ordre décroissant de produit en stock et non par produits les plus vendus mais il est possible de connaître cette valeur en info-bulle.
*	En parallèle, on peut suivre ici les **5 produits qui représentent la plus grosse partie du stock valorisé**. On parcourt le donut dans le sens des aiguilles d’une montre pour aller du stock le plus important au stock le moins important. Il est possible de connaître le détail sur un produit en cliquant sur une part du donut. Elle s’affichera à droite. De cette façon, on peut notamment connaître la quantité en stock et le prix auquel il a été valorisé.
*	La visualisation du 'Cumul des commandes N' permet de connaître le nombre de commandes passées à date (actuellement au 20/02/2024) et de le comparer au nombre de commandes passées à la même période l’année dernière. On enregistre 21 commandes depuis le 01/01/2024. L'année dernière à la même période, au 20/02/2023, 14 commandes avaient été enregistrées. Ce qui représente une hausse des commandes de 50%.
*	Enfin le dernier graphique permet de dessiner la **tendance des ventes de la société** au cours des 3 dernières années. On note clairement une saisonnalité avec une très forte saison en fin d’année au moment des fêtes de Noël. On remarquera également une saison marquée, bien que moins importante, au début des vacances d’été, en juillet/août en zoomant sur le graphique, ce qui permettra d’anticiper la gestion des stocks pour répondre à ces rendez-vous.




