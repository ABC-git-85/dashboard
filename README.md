# Dashboard - Power BI
## Présentation d'un tableau de bord d'une entreprise de jouets

<img width="1430" height="804" alt="image" src="https://github.com/user-attachments/assets/626b257d-fe5a-49a1-a28c-e79c59168c3d" />

### Contexte

La base de données d'une entreprise de jouets répertorie les employés, les produits, les commandes et un peu plus encore.
Le souhait de la direction est d'avoir un tableau de bord dynamique qui pourrait être actualiser chaque matin pour obtenir les dernières informations afin de gérer l’entreprise.

#### > Schéma de la base de données

<img width="1880" height="1372" alt="image" src="https://github.com/user-attachments/assets/62432153-6328-4746-aaec-cd4f8a914baf" />

### Objectifs et enjeux

Fournir des indicateurs clés de performance (KPI) afin de présenter les données liées à la logistique.

📌 Logistique
• Stock des produits sous seuil critique : Identifier les stocks des produits les plus commandés.
• Durée moyenne de traitement des commandes : Mesurer l’efficacité opérationnelle en analysant le temps entre la date de commande et la date d’expédition.
• Valorisation des stocks : calculer la valeur du stock et identifier les 5 produits qui représentent la plus grosse valeur de ce stock.
• KPI supplémentaires au choix

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



